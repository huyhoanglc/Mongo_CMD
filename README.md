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
// For example:
db.createCollection("StudentInfo")
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">InsertOne</h2>
<pre>
<code>
db.CollectionName.insertOne()
// For example:
db.StudentInfo.insertOne({ Name: "Huy" })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">InsertMany</h2>
<pre>
<code>
db.CollectionName.insertMany({Type: "Value of type"})
// For example:
db.StudentInfo.insertMany([{ Name: "Huy" }, { Name: "Minh" }])
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">Find</h2>
<pre>
<code>
db.CollectionName.find()
// For example:
db.StudentInfo.find()
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">UpdateOne</h2>
<pre>
<code>
db.CollectionName.updateOne({Type: "current Value of type" }, { $set: {Type: "new Value of type" } })
// For example:
db.StudentInfo.updateOne({ Name: "Huy" }, { $set: { Name: "Huy Tran" } })
</code>
</pre>

<h2 style="font-size: 24px; margin-top: 20px; color: #007BFF;">DeleteOne</h2>
<pre>
<code>
db.CollectionName.deleteOne({Type: "Value of type To Delete" })
// For example:
db.StudentInfo.deleteOne({ Name: "Huy" })
</code>
</pre>
