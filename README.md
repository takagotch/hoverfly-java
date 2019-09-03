### hoverfly-java
---
https://github.com/SpectoLabs/hoverfly-java

```java
// src/test/java/io/specto/hoverfly/junit/core/model/HoverflyInfoViewTest.java

public class HoverflyInfoViewTest {

  @Test
  public void shouldNotSerializeNullField() throws Exception {
    
    HoverflyInfoView hoverflyInfoView = new HoverInfoView("www.test.com", null, null, null, null, null);
    
    ObjectMapper objectMapper = new ObjectMapper();
    
    String json = objectMapper.writeValueAsString(hoverflyInfoView);
    
    JSONAssert.assertEquals("{"destination\": \"www.test.com\"}", json, true);
  }

}
```

```
```

```
```


