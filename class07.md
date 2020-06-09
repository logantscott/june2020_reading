[Table of Contents](https://github.com/logantscott/june2020_reading)

## Express

### Express Routing
```app.get('/thing', (req, res) => {})```

#### Request (req, ...)
id = 1234  
req.params.id = app.get('/thing/:id', ...) = app.get('/thing/1234', ...)  
req.query.id = http://localhost:7890/thing?id=1234

#### Response (..., res)
Sends data back to the client/browser (including status, headers, body)


### Express Middleware
Generally speaking, does stuff before it hits the route. Some uses:  
-Good for common tasks on a route(s)  
-Error Handling  
-Logging  
-Parsing


### CRUD Operations
| CRUD | Express |
| :--- | :--- |
| **C**reate | app.post('/resource') |
| **R**ead | app.get('/resource') |
| **U**pdate | app.put('/resource') |
| **D**elete | app.delete('/resource') |


### Testing
It's a good idea to use supertest or mock superagent to avoid affecting production, spinning up a server, and avoiding bad/slow data (when testing the interface)