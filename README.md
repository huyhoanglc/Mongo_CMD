
<h1 style="font-size: 36px; font-weight: bold; text-align: center; color: #007BFF;">
    MongoDB Commands
</h1>
<hr style="border: 3px solid #6f42c1;">

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">Create Database</h2>
<pre>
<code>
use "Name of Database"
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">Create Collection</h2>
<pre>
<code>
db.createCollection("Name of Collection")
<span style="color: #28a745;">For example:</span>
db.createCollection("StudentInfo")
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">InsertOne</h2>
<pre>
<code>
db.CollectionName.insertOne()
<span style="color: #28a745;">For example:</span>
db.StudentInfo.insertOne({ Name: "Huy" })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">InsertMany</h2>
<pre>
<code>
db.CollectionName.insertMany()
<span style="color: #28a745;">For example:</span>
db.StudentInfo.insertMany([{ Name: "Huy" }, { Name: "Minh" }])
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">Find</h2>
<pre>
<code>
db.CollectionName.find()
<span style="color: #28a745;">For example:</span>
db.StudentInfo.find()
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">UpdateOne</h2>
<pre>
<code>
db.CollectionName.updateOne({ Name: "currentName" }, { $set: { Name: "newName" } })
<span style="color: #28a745;">For example:</span>
db.StudentInfo.updateOne({ Name: "Huy" }, { $set: { Name: "Huy Tran" } })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">DeleteOne</h2>
<pre>
<code>
db.CollectionName.deleteOne({ Name: "nameToDelete" })
<span style="color: #28a745;">For example:</span>
db.StudentInfo.deleteOne({ Name: "Huy" })
</code>
</pre>

<h1 style="font-size: 36px; font-weight: bold; text-align: center; color: #007BFF;">
    MongoDB Commands
</h1>
<hr style="border: 3px solid #6f42c1;">

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">Create Database</h2>
<pre>
<code>
use "Name of Database"
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">Create Collection</h2>
<pre>
<code>
db.createCollection("Name of Collection")
<span style="color: #28a745;">For example:</span>
db.createCollection("StudentInfo")
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">InsertOne</h2>
<pre>
<code>
db.CollectionName.insertOne()
<span style="color: #28a745;">For example:</span>
db.StudentInfo.insertOne({ Name: "Huy" })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">InsertMany</h2>
<pre>
<code>
db.CollectionName.insertMany()
<span style="color: #28a745;">For example:</span>
db.StudentInfo.insertMany([{ Name: "Huy" }, { Name: "Minh" }])
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">Find</h2>
<pre>
<code>
db.CollectionName.find()
<span style="color: #28a745;">For example:</span>
db.StudentInfo.find()
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">UpdateOne</h2>
<pre>
<code>
db.CollectionName.updateOne({ Name: "currentName" }, { $set: { Name: "newName" } })
<span style="color: #28a745;">For example:</span>
db.StudentInfo.updateOne({ Name: "Huy" }, { $set: { Name: "Huy Tran" } })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">DeleteOne</h2>
<pre>
<code>
db.CollectionName.deleteOne({ Name: "nameToDelete" })
<span style="color: #28a745;">For example:</span>
db.StudentInfo.deleteOne({ Name: "Huy" })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">Count Documents</h2>
<pre>
<code>
db.CollectionName.countDocuments()
<span style="color: #28a745;">For example:</span>
db.StudentInfo.countDocuments()
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">Find with Condition</h2>
<pre>
<code>
db.CollectionName.find({ "field": "value" })
<span style="color: #28a745;">For example:</span>
db.StudentInfo.find({ Name: "Huy" })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">Sort Results</h2>
<pre>
<code>
db.CollectionName.find().sort({ "field": 1 }) // 1 for ascending, -1 for descending
<span style="color: #28a745;">For example:</span>
db.StudentInfo.find().sort({ Name: 1 })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">Limit Results</h2>
<pre>
<code>
db.CollectionName.find().limit(number)
<span style="color: #28a745;">For example:</span>
db.StudentInfo.find().limit(5)
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">DeleteMany</h2>
<pre>
<code>
db.CollectionName.deleteMany({ "field": "value" })
<span style="color: #28a745;">For example:</span>
db.StudentInfo.deleteMany({ Name: "Huy" })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">UpdateMany</h2>
<pre>
<code>
db.CollectionName.updateMany({ "field": "value" }, { $set: { "fieldToUpdate": "newValue" } })
<span style="color: #28a745;">For example:</span>
db.StudentInfo.updateMany({ Name: "Huy" }, { $set: { Name: "Huy Tran" } })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">ReplaceOne</h2>
<pre>
<code>
db.CollectionName.replaceOne({ "field": "value" }, { "newDocument" })
<span style="color: #28a745;">For example:</span>
db.StudentInfo.replaceOne({ Name: "Huy" }, { Name: "Huy Tran", Age: 22 })
</code>
</pre>
