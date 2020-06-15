[Table of Contents](https://github.com/logantscott/june2020_reading)

## Authentication

### User Modeling
Whenever modeling your applications, make sure to split up sensitive information so it can be served separately and more securely than the more public data.

### Cryptography
Generally speaking, uses an algorith to encrypt your data, and needs a key to decrypt it.

### Hash Algorithms
A hash algorith is consistent, if you pass the same data to it, it will produce the same output. Data is hased -> sent to server -> compared to another hash to see if there is a match.

### Cypher Algorithms
Often used by apps/services to make them more secure, a token is generated for a user and encrypted, with a secret key on the server. The encrypted token is sent to the client to be sent back, which is decrypted by the server back into the token.

### Basic Authorization
User/pass are encoded and sent over HTTPS, an auth token/key is sent back and can be used by the client as already having logged in.
