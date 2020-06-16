[Table of Contents](https://github.com/logantscott/june2020_reading)

## User Auth

### On bcrypt and hashes/salts
Plain text passwords are extremely vulnerable to hacking. One first solution is to hash the password with a commmon encryption algorithm (then which the server would compare hashes but never have the password), but this is vulnerable to certain kinds of attacks for commonly used passwords. The next solution is to salt the password before hashing, with a salt string, to make this list of passwords less generic to one algorithm potentially used by thousands of sites to just one. Even more secure is providing each user with their own salt on signup, so generating an attack list for one site is still not feasible.

#### bcrypt
Using bcrypt helps further by slowing down the encryption process using salt rounds. This makes generating a list of potential common passwords much, much slower in combination with having unique salts per user. It's the difference between some milliseconds and several seconds.

### On SPAs with APIs and tokens
