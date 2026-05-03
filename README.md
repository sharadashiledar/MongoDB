Overview

MongoDB is a NoSQL database that stores data in a flexible, JSON-like format called documents. It is designed for scalability, high performance, and ease of development.

🚀 Features
Document-oriented database (stores data as JSON/BSON)
Schema-less (flexible structure)
High performance and scalability
Supports indexing, aggregation, and replication
Easy integration with modern applications
🛠️ Installation
1. Download MongoDB

Go to the official website:
👉 https://www.mongodb.com/try/download/community

2. Install MongoDB
Run the installer
Choose Complete Setup
Install MongoDB as a service (recommended)
3. Verify Installation

Open command prompt and run:

mongod --version
▶️ Starting MongoDB
Start MongoDB Server
mongod
Start MongoDB Shell
mongosh
📂 Basic MongoDB Commands
1. Show Databases
show dbs
2. Create / Switch Database
use myDatabase
3. Create Collection
db.createCollection("students")
4. Insert Data
db.students.insertOne({
  name: "Sharada",
  age: 20,
  course: "BCA"
})
5. Insert Multiple Documents
db.students.insertMany([
  { name: "Amit", age: 21 },
  { name: "Riya", age: 19 }
])
6. Find Data
db.students.find()
7. Find One Document
db.students.findOne({ name: "Sharada" })
8. Update Data
db.students.updateOne(
  { name: "Sharada" },
  { $set: { age: 21 } }
)
9. Delete Data
db.students.deleteOne({ name: "Amit" })
🔍 Query Operators
Comparison Operators
db.students.find({ age: { $gt: 20 } })
$gt → Greater than
$lt → Less than
$gte → Greater than or equal
$lte → Less than or equal
📊 Useful Commands
Show Collections
show collections
Drop Collection
db.students.drop()
Drop Database
db.dropDatabase()
📁 Project Structure Example
mongodb-project/
│── README.md
│── app.js
│── package.json
│── models/
│── routes/
│── config/
🔗 Use Cases
Web applications
Real-time analytics
Content management systems
E-commerce platforms
📚 Resources
Official Docs: https://www.mongodb.com/docs/
MongoDB University: https://university.mongodb.com/
✨ Conclusion

MongoDB is a powerful and flexible database that is widely used in modern application development. It is especially useful when working with dynamic or unstructured data.
