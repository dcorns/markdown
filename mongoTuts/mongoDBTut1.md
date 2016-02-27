#MongoDB Basics
##Welcome to no SQL
MongoDB is known a 'no sql' database. Since Structured Query Language databases have dominated the scene for quite some time, it makes since to distinguish newer database technologies as 'no sql' databases...I guess. That is just the way it is. But that only tells that it is not an sql database; not very useful information. Tell me more, you say? MongoDB is what is also known as a document based database(dbds). Let's take a moment to contrast document based databases from sql databases. One, dbds do not require structured query language. Two, dbds do not require tables and columns, do not require predefined data types prior to adding data.

###Database Design


###Creating a Mongo Database and adding some data
Using Mongo shell:
use *database name*

create collection and insert data in one step:

db.prizes.insert({name:"Redbox Movies for a Year", value: 78, available: 1750, tickets:{required: 4, partList:["N559A",2, "N560B", 1, "N561C", 2, "N562D", 0],winner:"N562D"}})
Inserted 1 record(s) in 14ms
WriteResult({
  "nInserted": 1
})

find a document in a collection
db.prizes.find({name:"Home Makeover"})


Updating Data
Add new field and data to all documents in a collection
*multi parameter must be set to true*
db.prizes.update({},{$set:{lastAvailabilityUpdate:"Fri Feb 26 2016 00:00:00 GMT-0800 (PST)"}},{multi:true} )
Updated 28 existing record(s) in 2ms
WriteResult({
  "nMatched": 28,
  "nUpserted": 0,
  "nModified": 28
})

Remove field and data from all documents

Update specific document

