# Class 12: Mongo and Mongoose

## [SQL vs NoSQL Database Differences Explained with few Example DB](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

- NoSQL databases are document based, key-value pairs, graph databases or wide-column stores. SQL databases represent data in form of tables.
- NoSQL databases have dynamic schema for unstructured data.
- SQL databases are scaled by increasing the horse-power of the hardware. NoSQL databases are scaled by increasing the databases servers in the pool of resources to reduce the load.
- SQL databases are good fit for the complex query intensive environment
- NoSQL database are highly preferred for large data sets
- Examples of DBs:
  - SQL Databases:
    - MySQL
    - MS SQL
    - Oracle
    - SQLite
    - PostgreSQL
  - NoSQL Databases:
    - MongoDB
    - CouchDB
    - Redis

## [NOSQL DATA MODELING TECHNIQUES](https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-techniques/)

- 

## [Mongoose Docs](https://mongoosejs.com/docs/api.html#Model)

- Mongoose is `elegant mongodb object modeling for node.js`
- What it looks like:

```javascript
const mongoose = require('mongoose');
mongoose.connect('mongodb://localhost:27017/test', {useNewUrlParser: true, useUnifiedTopology: true});

const Cat = mongoose.model('Cat', { name: String });

const kitty = new Cat({ name: 'Zildjian' });
kitty.save().then(() => console.log('meow'));
```

- See the models section in the docs, linked above, for more information on what building a model can look like.

## Video: [SQL vs NoSQL or MySQL vs MongoDB](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y&ab_channel=Academind)

-
