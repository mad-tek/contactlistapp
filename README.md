#### Setting up and getting started with the MEAN stack

This requires Node.js installed
Install dependencies in terminal:
```
$ npm install
```
Dependencies:
>"body-parser": "^1.13.1" (parse JSON)
>"mongojs": "^1.0.1" (Mongo management)
>"express": "^4.13.0" (server framework for node)
>"nodemon": "^1.3.7" (node monitor, auto reload on file change)

In the example, all the dependencies are included and called in server.js

Next, download MongoDB in the console
```
$ brew install mongodb
```
Then, create the folder "data" with the folder "db" inside at the root or another location
```
$ touch data/db/
```
Then run MongoDB to boot up the database
```
$ mongod
```
if data/db is not in the root directory
```
$ mongod --dbpath <whateverpath/data>
```
In another console check and create the database
```
$ mongo
> show dbs
//admin  (empty)
//local  0.078GB
> use <name a new database you will be using>
//switched to db <whatever name you put in>
```

That's it for the setup. The rest of the routing is in the server.js
