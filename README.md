# Mongo_CLI
**Connect to Db**

* To see all the dbs

```
show dbs

```

* Switch to a db(go in db)

```
use  <database_name> 

 ```

* See collections inside a db

 ``` 
 show collections

  ```

* Query Data in Collections of a DB

```
db.<collection_name>.find(<query>)

```

**CRUD**

* Insert (Create)
```
db.<collection_name>.insertOne({ field1: "value1", field2: "value2" })

db.<collection_name>.insertMany([
    { field1: "value1", field2: "value2" },
    { field1: "value3", field2: "value4" }
])

```
* Read( Query)

```
db.<collection_name>.find(<query>)

db.<collection_name>.findOne(<query>, ?<projection>)

```

* Update 
```
db.<collection_name>.updateOne(
    { field1: "value1" },
    { $set: { field2: "new_value" } }
)

db.<collection_name>.updateMany(
    { field1: "value1" },
    { $set: { field2: "new_value" } }
)


```

* Delete
```
db.<collection_name>.deleteOne({ field1: "value1" })

db.<collection_name>.deleteMany({ field1: "value1" })

```
