[Table of Contents](https://github.com/logantscott/june2020_reading)

## Mongoose Methods

### Instance & Static Methods
Just like ES6 classes, static methods apply to models and instance methods apply to documents. 
```Instance: [schemaName].methods.[methodName] = function(callback) {}```
```Static: [schemaName].statics.[staticName] = function(var) {}```

### Mongoose Middleware
Mongoose has 4 types of middleware that can be used pre and post of the functions being called. The 4 types and their functions:

| Document | Query | Aggregate | Model |
| :--- | :--- | :--- | :--- |
| [validate](https://mongoosejs.com/docs/api/document.html#document_Document-validate) | [count](https://mongoosejs.com/docs/api.html#query_Query-count) | [aggregate](https://mongoosejs.com/docs/api.html#model_Model.aggregate) | [insertMany](https://mongoosejs.com/docs/api.html#model_Model.insertMany) |
| [save](https://mongoosejs.com/docs/api/model.html#model_Model-save) | [deleteMany]() | | |
| [remove](https://mongoosejs.com/docs/api/model.html#model_Model-remove) | [find]() | | |
| [updateOne](https://mongoosejs.com/docs/api/document.html#document_Document-updateOne) | [findOne]() | | |
| [deleteOne](https://mongoosejs.com/docs/api/model.html#model_Model-deleteOne) | [findOneAndDelete]() | | |
| [init*](https://mongoosejs.com/docs/api/document.html#document_Document-init) | [findOneAndRemove]() | | |
| | [findOneAndUpdate](https://mongoosejs.com/docs/api.html#query_Query-findOneAndUpdate) | | |
| | [remove](https://mongoosejs.com/docs/api.html#model_Model.remove) | | |
| | [update](https://mongoosejs.com/docs/api.html#query_Query-update) | | |
| | [updateOne](https://mongoosejs.com/docs/api.html#query_Query-updateOne) | | |
| | [updateMany](https://mongoosejs.com/docs/api.html#query_Query-updateMany) | | |