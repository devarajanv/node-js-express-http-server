# Overview
A sample node js express http server which exposes REST methods like GET, POST, DELETE in a HTTP port

# Install Node.js 
Install Node.js from https://nodejs.org/en/download/ 
I have installed it using Windows Installer (.msi) 64-bit (https://nodejs.org/dist/v6.10.0/node-v6.10.0-x64.msi) for my windows desktop

# Open Node.js command prompt 
Open Node.js command prompt so that it picks up the node executable
start(windows) --> All Programs --> Node.js --> Node.js command prompt

# Checkout project from Github
You probably might be aware of Github, so you can ignore and goto next step
but if you are new to github,
To go to your workspace and checkout the project from github
$ cd C:\workspace\
$ git clone  https://github.com/devarajanv/node-js-express-http-server.git

# Install Express for http methods
$npm install express --save
 
# Edit/Run the javascript 
Edit/Run the javascript file(http-server.js). This creates a JSON document, inserts it into MarkLogic Database(Documents Database) by making a REST API interface call.
$ node http-server.js

# Output
Example app listening at http://:::8082
To Verify this output, please make a REST call in your browser or any REST Client(Like Postman, SoapUI) 
and goto 

GET http://localhost:8082/ 

Output will be 200 Success response code with this message below:
Hello GET

# FAQ or Frequently faced errors
If you have run this command $node http-server.js ahead of installing dependencies for node.js, then you'll get this error.
Error: Cannot find module 'express'
    at Function.Module._resolveFilename (module.js:469:15)
    at Function.Module._load (module.js:417:25)
    at Module.require (module.js:497:17)
    at require (internal/module.js:20:19)
    at Object.<anonymous> (C:\workspace\node-js-express-http-server\http-server.js:4:15)
    at Module._compile (module.js:570:32)
    at Object.Module._extensions..js (module.js:579:10)
    at Module.load (module.js:487:32)
    at tryModuleLoad (module.js:446:12)
    at Function.Module._load (module.js:438:3)


