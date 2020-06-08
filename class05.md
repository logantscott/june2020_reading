[Table of Contents](https://github.com/logantscott/june2020_reading)

## Readings: HTTP and REST

### HTTP


### HTTP Requests


### HTTP Response


### REST
Acronym for **RE**presentational **S**tate **T**ransfer. Operates on the state of a resource most commonly with CRUD operations:

| REST Method | CRUD Operation | Request Body | Response Body | Idempotent | Safe | Cacheable | Function |
| :---    | :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| GET     | READ |  | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | Retrieve 1 or More Records |
| POST	  | CREATE	| :heavy_check_mark: | :heavy_check_mark: |  |  | :heavy_check_mark: | Create a new record |
| PUT	    | UPDATE	| :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |  |  | Update a record through replacement (Put it back) |
| PATCH	  | UPDATE  | :heavy_check_mark: | :heavy_check_mark: |  |  |  | Update a record (just the parts that changed) |
| DESTROY | DELETE  |  | :heavy_check_mark: | :heavy_check_mark: |  |  | Remove a record |

**Safe**
Only for information retrieval, not state change.
**Idempotent**
Two identical requests should get the same response.
**Cacheable**
The client should be able to cache the response.

### REST Documentation