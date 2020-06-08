[Table of Contents](https://github.com/logantscott/june2020_reading)

## Readings: HTTP and REST

### HTTP
**H**yper **T**ext **T**ransfer **P**rotocol is a stateless application-
   level protocol for distributed, collaborative, hypertext information
   systems (per IETF). Foundation of the modern web.

### HTTP Requests
Standard request starts with HTTP method, URL, and version. This is followed by the request headers and a conditional request body.

### HTTP Response
Standard response starts with HTTP version and status code/message (e.g. 200 OK). This is followed by the response headers and an conditional response body.

### REST
Acronym for **RE**presentational **S**tate **T**ransfer. Operates on the state of a resource most commonly with CRUD operations:  

| REST Method | CRUD Operation | Request Body | Response Body | Idempotent | Safe | Cacheable | Function |
| :---    | :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| GET     | READ |  | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | Retrieve 1 or More Records |
| POST	  | CREATE	| :heavy_check_mark: | :heavy_check_mark: |  |  | :heavy_check_mark: | Create a new record |
| PUT	    | UPDATE	| :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |  |  | Update a record through replacement (Put it back) |
| PATCH	  | UPDATE  | :heavy_check_mark: | :heavy_check_mark: |  |  |  | Update a record (just the parts that changed) |
| DESTROY | DELETE  |  | :heavy_check_mark: | :heavy_check_mark: |  |  | Remove a record |

**CRUD**  
**C**reate **R**ead **U**pdate **D**elete  
**Safe**  
Only for information retrieval, not state change.  
**Idempotent**  
Two identical requests should get the same response.  
**Cacheable**  
The client should be able to cache the response.  

### REST Documentation
**Swagger/OpenAPI** - The OpenAPI Specification was donated to the Linux Foundation under the OpenAPI Initiative in 2015. The specification creates a RESTful interface for easily developing and consuming an API by effectively mapping all the resources and operations associated with it.

[Swagger.io](https://swagger.io/) - Can be used for easily generating documentation for RESTful APIs.
