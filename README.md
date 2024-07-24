<h1 style="font-size: 36px; font-weight: bold; text-align: center;">
    MongoDB Commands
</h1>
<hr style="border: 3px solid #6f42c1;">

<h2 style="font-size: 24px; margin-top: 20px;">Create Database</h2>
<pre>
<code>
use "Name of Database"
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">Create Collection</h2>
<pre>
<code>
db.createCollection("Name of Collection")
<small>For example:</small>
db.createCollection("StudentInfo")
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">InsertOne</h2>
<pre>
<code>
db.CollectionName.insertOne()
<small>For example:</small>
db.StudentInfo.insertOne({ Name: "Huy" })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">InsertMany</h2>
<pre>
<code>
db.CollectionName.insertMany()
<small>For example:</small>
db.StudentInfo.insertMany([{ Name: "Huy" }, { Name: "Minh" }])
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">Find</h2>
<pre>
<code>
db.CollectionName.find()
<small>For example:</small>
db.StudentInfo.find()
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">UpdateOne</h2>
<pre>
<code>
db.CollectionName.updateOne({ Name: "currentName" }, { $set: { Name: "newName" } })
<small>For example:</small>
db.StudentInfo.updateOne({ Name: "Huy" }, { $set: { Name: "Huy Tran" } })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">DeleteOne</h2>
<pre>
<code>
db.CollectionName.deleteOne({ Name: "nameToDelete" })
<small>For example:</small>
db.StudentInfo.deleteOne({ Name: "Huy" })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">Count Documents</h2>
<pre>
<code>
db.CollectionName.countDocuments()
<small>For example:</small>
db.StudentInfo.countDocuments()
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">Find with Condition</h2>
<pre>
<code>
db.CollectionName.find({ "field": "value" })
<small>For example:</small>
db.StudentInfo.find({ Name: "Huy" })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">Sort Results</h2>
<pre>
<code>
db.CollectionName.find().sort({ "field": 1 }) // 1 for ascending, -1 for descending
<small>For example:</small>
db.StudentInfo.find().sort({ Name: 1 })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">Limit Results</h2>
<pre>
<code>
db.CollectionName.find().limit(number)
<small>For example:</small>
db.StudentInfo.find().limit(5)
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">DeleteMany</h2>
<pre>
<code>
db.CollectionName.deleteMany({ "field": "value" })
<small>For example:</small>
db.StudentInfo.deleteMany({ Name: "Huy" })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">UpdateMany</h2>
<pre>
<code>
db.CollectionName.updateMany({ "field": "value" }, { $set: { "fieldToUpdate": "newValue" } })
<small>For example:</small>
db.StudentInfo.updateMany({ Name: "Huy" }, { $set: { Name: "Huy Tran" } })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">ReplaceOne</h2>
<pre>
<code>
db.CollectionName.replaceOne({ "field": "value" }, { "newDocument" })
<small>For example:</small>
db.StudentInfo.replaceOne({ Name: "Huy" }, { Name: "Huy Tran", Age: 22 })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px;">Import</h2>
<pre>
<code>
mongoimport --db Name_Database --collection Name_Collection --jsonArray --file "path to file json"
<small>For example:</small>
mongoimport --db sample_weatherdata --collection data --jsonArray --file "C:\Users\huypg\Desktop\Mongo\mongodb-sample-dataset\mongodb-sample-dataset\sample_weatherdata\data.json"
</code>
</pre>
