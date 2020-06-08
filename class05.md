[Table of Contents](https://github.com/logantscott/june2020_reading)

## Readings: HTTP and REST

### HTTP


### HTTP Requests


### HTTP Response


### REST
Acronym for **RE**presentational **S**tate **T**ransfer. Operates on the state of a resource most commonly with CRUD operations:

| REST Method | CRUD Operation | Req Body? | Res Body? | Idempotent | Safe | Function |
| :---    | :--- | :---: | :---: | :--- | :--- | :--- |
| GET     | READ |  | :heavy_check_mark: | Yes | Yes | Retrieve 1 or More Records |
| POST	  | CREATE	| :heavy_check_mark: | :heavy_check_mark: | No | No | Create a new record |
| PUT	    | UPDATE	| :heavy_check_mark: | :heavy_check_mark: | Yes | No | Update a record through replacement (Put it back) |
| PATCH	  | UPDATE  | :heavy_check_mark: | :heavy_check_mark: | No | No | Update a record (just the parts that changed) |
| DESTROY | DELETE  |  | :heavy_check_mark: | Yes | No | Remove a record |


### REST Documentation