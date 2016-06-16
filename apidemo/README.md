# API调用示例

##java示例
```java
      package soma.api.demo;

      import java.security.MessageDigest;

      import org.apache.http.HttpEntity;
      import org.apache.http.HttpResponse;
      import org.apache.http.HttpStatus;
      import org.apache.http.client.methods.HttpPost;
      import org.apache.http.entity.StringEntity;
      import org.apache.http.impl.client.CloseableHttpClient;
      import org.apache.http.impl.client.HttpClientBuilder;
      import org.apache.http.util.EntityUtils;

      import com.google.gson.JsonObject;
      import com.google.gson.JsonParser;

      import soma.api.Constants;

      public class SoMaApiDemo {

          public static final int RESPONSE_CODE_SUCCESS = 0;

          public static final int RESPONSE_CODE_FAILED = 1;

          public static final int RESPONSE_CODE_PART_SUCCESS = 2;

          public static final int RESPONSE_CODE_SESSION_OVERTIME = 3;

          public static final int RESPONSE_CODE_PART_FAILED = 4;

          public static final int RESPONSE_CODE_TIMEOUT = 99;

          public static final String LOGIN_URL = "http://soma.yonyou.com/soma/rest/system/login";

          public static final String USER_JSON = "{\"name\":\"%s\",\"password\":\"%s\"}";

          public static final String DC_URL = "http://soma.yonyou.com/soma/rest/datacenter/listbypage";

          public static final String QC_JSON = "{\"pageSize\":%d,\"pageIndex\":%d}";

          public static void main(String arg[]) throws Exception {

              // login
              String user = "caipingxin";
              String pwd = crypt("password");
              String param = String.format(USER_JSON, user, pwd);
              String ret = doPost(LOGIN_URL, param);
              JsonParser parser = new JsonParser();
              JsonObject res = parser.parse(ret).getAsJsonObject();
              int code = res.get("code").getAsInt();
              String sessionId = null;
              if (Constants.RESPONSE_CODE_SUCCESS == code) {
                  sessionId = res.get("data").getAsJsonObject().get("sessionId").getAsString();
              } else {
                  System.out.println("login failed!");
              }

              if (sessionId == null) {
                  return;
              }

              // query datacenter
              param = String.format(QC_JSON, 10, 1);

              ret = doPost(DC_URL, param, sessionId);
              res = parser.parse(ret).getAsJsonObject();
              code = res.get("code").getAsInt();

              if (Constants.RESPONSE_CODE_SUCCESS == code) {
                  System.out.println(res.get("data"));
              }

          }

          public static String doPost(String url, String param) {
              return doPost(url, param, null);
          }

          public static String doPost(String url, String param, String sessionId) {
              HttpPost post = new HttpPost(url);
              try {
                  StringEntity s = new StringEntity(param);
                  s.setContentEncoding("UTF-8");
                  s.setContentType("application/json");
                  if (sessionId != null) {
                      post.addHeader("sessionid", sessionId);
                  }
                  post.setEntity(s);
                  CloseableHttpClient client = HttpClientBuilder.create().build();
                  HttpResponse res = client.execute(post);
                  if (res.getStatusLine().getStatusCode() == HttpStatus.SC_OK) {
                      HttpEntity entity = res.getEntity();
                      String result = EntityUtils.toString(entity);
                      return result;
                  }
              } catch (Exception e) {
                  throw new RuntimeException(e);
              }
              return param;

          }

          protected static String crypt(String s) throws Exception {
              MessageDigest md = MessageDigest.getInstance("MD5");
              byte[] digest = md.digest(s.getBytes("utf-8"));
              StringBuffer hex = new StringBuffer();
              for (int i = 0; i < digest.length; i++) {
                  int val = ((int) digest[i]) & 0xff;
                  if (val < 16)
                      hex.append("0");
                  hex.append(Integer.toHexString(val));
              }
              return hex.toString();
          }

      }
```
