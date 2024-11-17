# mongodb-learning


```
MySql    mongodb
Database Database
Table    Collection
Rows     Documents

less relation
data is stored together




brew services start mongodb-community@8.0
mongod --config /opt/homebrew/etc/mongod.conf --fork
brew services restart mongodb-community

mongosh


show dbs


for clear terminal
cls
ctrl+L


use latest_db

db.students.insertOne({ name: "Shyam", age: 13 })
db.students.find()


insertOne(data,options)
insertMany(data,options)

find(filter,option)
findOne(filter,options)



updateOne(filter,data,options)
updateMany(filter,data,options)
replaceOne(filter,data,options)

show collections

db.students.find({hobbies:"Cooking"})
db.students.find()


db.students.find({age:33})

db.students.find({age:{$gte:12}}).limit(2)
db.students.find({age:{$gte:12}})
db.students.find({age:{$gt:12}})

db.students.find().toArray()


use school

db.students.deleteMany({age:12})
db.student.deleteMany({})

db.students.find({},{name:1,_id:0,age:1})

db.dropDatabase()

db.products_new.drop()

db.createCollection(name, options)

```








