### Sample Index

```
{
  "email": "abc@xyz.com",
  "employee-id": 10001
  "age": 32
  "name": Chandler Bing
}
```



### Sample mapping example:

```
{
  "my-index" : {
    "mappings" : {
      "properties" : {
        "age" : {
          "type" : "integer"
        },
        "email" : {
          "type" : "keyword"
        },
        "employee-id" : {
          "type" : "integer"
        },
        "name" : {
          "type" : "text"
        }
      }
    }
  }
}
```
