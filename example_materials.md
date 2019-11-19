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

### Sample settings examples:

```
{
    "settings" : {
        "number_of_shards" : 1
    },
    "mappings" : {
        "properties" : {
            "field1" : { "type" : "text" }
        }
    }
}
```


### index with settings and mappings:

```
PUT employees
{
  "settings": {
    "number_of_shards": 2,
    "number_of_replicas": 1
  },
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
```
