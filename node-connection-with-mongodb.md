# Node JS Connection with mongodb
##### Node
[Mongodb](https://www.mongodb.com/) is a cross-platform and open-source document-oriented database, it is kind of a NoSQL/Unstructure database. As a  Unstructure database it store data in the form of json object, Any field in Mongodb can be indexed.

##### Feature
- Ad hoc queries - supports search by field, regular expression searches, and range - queries.
- Indexing - any field in the BSON document can be indexed.
- Replication - provides high availability via replica sets which consists of two or more copies of the original data.
- Load balancing - sharding is the method used to allow MongoDB to scale horizontally, meaning that data will be distributed and split into ranges and then stored in different shards which can be located in different servers. Shard keys are used to determine how the data will be distributed.
- Aggregation - MapReduce can be applied to enable batch processing of data as well as perform aggregation operations.
- File storage - MongoDB can be used as file system which makes use of the above functions and acting in a distributed manner through sharding.

##### Mongodb Connection
-	Connection String 
    - `mongodb://[username:password@]host1[:port1][,host2[:port2],...[,hostN[:portN]]][/[database][?options]]` 
    - [Refference](https://docs.mongodb.com/manual/reference/connection-string/)
-	Mongoose: It is a npm module used for connecting `Mongodb` with nodejs.
-	Example:
	
-	    let mongoose = require('mongoose');
-	    mongoose.connect('<connection string>').then(connected => console.log(connected)).catch(error=> console.log(error))

###### Thank you
