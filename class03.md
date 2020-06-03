[Table of Contents](https://github.com/logantscott/june2020_reading)

## Data Modeling & NoSQL Databases

### Reading, Research, and Discussion
1. **Why would a developer choose to make data models?**  
Data models help give structure and rules to the organization of your data and how it relates. 

1. **What purpose do CRUD operations serve?**  
Creation, reading, updating, and deleting of information. These are the four common database and RESTful operations (create/read/update/delete and post/get/put/delete). 

1. **What kind of database is Postgres? What kind of database is MongoDB?**  
Postgres is SQL (relational) and MongoDB is NoSQL.

1. **What is Mongoose and why do we need it?**  
Mongoose allows users to easily interact with MongoDB through NodeJS (object modeling). Mongoose provides type-casting, validation, and many other common operations.

1. **Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.**  
Customer, order, and inventory/item. An order contains a customer and one or more items. A customer can have one or more orders, but the customer table/document would only include customer information (name, shipping, billing, etc). An item can be on one or more orders going to one or more customers, but the item table/document would contain specific item information (title, price, etc). 


### Vocabulary
**database**  
A database is an organized collection of structured information, or data, typically stored electronically in a computer system.

**data model**  
Data model is a high level design which decides what can be present in the schema. It provides a database user with a conceptual framework in which we specify the database requirements of the database user and the structure of the database to fulfill these requirements.

**CRUD**  
Create, read, update, and delete are the four basic functions of persistent storage.

**schema**  
A database schema represents the logical configuration of all or part of a relational database. It can exist both as a visual representation and as a set of formulas known as integrity constraints that govern a database. These formulas are expressed in a data definition language, such as SQL. As part of a data dictionary, a database schema indicates how the entities that make up the database relate to one another, including tables, views, stored procedures, and more. 

**sanitize**  
The process of preventing code injection problems, utilizing secure input and output handling

**Structured Query Language (SQL)**  
Structured Query Language is a standard language for accessing and manipulating databases. According to ANSI (American National Standards Institute), it is the standard language for relational database management systems.

**Non SQL (NoSQL)**  
NoSQL databases (aka "not only SQL") are non tabular, and store data differently than relational tables. NoSQL databases come in a variety of types based on their data model. The main types are document, key-value, wide-column, and graph. They provide flexible schemas and scale easily with large amounts of data and high user loads.

**MongoDB**  
A cross-platform document-oriented database program. Classified as a NoSQL database program, MongoDB uses JSON-like documents with optional schemas.

**Mongoose**  
Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node.js. It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB.

**record**  
A record in a database is an object that can have one or more values (or like a row in a table).

**document**  
MongoDB Document is an entity in which zero or more ordered field-value pairs are stored. In comparison to Relational Databases, it is analogous to a record or row in table.

**Object Relation Mapping (ORM)**  
ORM in computer science is a programming technique for converting data between incompatible type systems using object-oriented programming languages. This creates, in effect, a "virtual object database" that can be used from within the programming language.
