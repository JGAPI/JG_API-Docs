# Getting Started
---
```java
public class Bot {
    static JG_API jg_api;

    public static void main(String[] args) {
        try {
            jg_api = new JG_API.ClientBuilder()
                    .setToken("gapi_token-here")
                    .addListenerAdapter(new EventHandler())
                    .build();

            jg_api.login();
            jg_api.start();
        } catch (Exception e) {
            e.printStackTrace();
        }

    }
}
```