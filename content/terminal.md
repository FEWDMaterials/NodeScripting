# Terminal JS

## Setting up the environment

* Download iTerm2 (if you prefer terminal, that's ok too)
* Install nodejs (everyone should have this done already)

## Getting Started

What is NodeJS?
```bash
>> 'Hello, (Node) Wrold'
```

How dependency imports work in node

```javascript
var Module = require('./someModule');

// ^^^ but what does that even MEAN??
```

Node Package Manager, or npm
```json
{
  "name": "statik",
  "version": "1.0.0",
  "description": "simple static site generator",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "Mottaqui Karim",
  "license": "ISC",
  "dependencies": {
    "colors": "^1.1.2",
    "commander": "^2.8.1",
    "marked": "^0.3.5",
    "q": "^1.4.1",
    "underscore": "^1.8.3",
    "watch": "^0.16.0"
  }
}
```

```bash
>> npm init
>> npm install
```

## File I/O

Read file
```javascript
var fs = require('fs');

fs.readFile('./index.html', function(err, data) {
    console.log( data );
});
```
Exercise: write file
```javascript
var fs = require('fs');

// how do we write a file in Node?
```

How do we write and run code in Node?
```bash
>> node [file_name]
```

## Command Line

How do we create simple command line scripts with NodeJS?

```javascript
#! /usr/bin/env node

var fs = require('fs');

/*
    code here to copy a file
*/

function copyFile( file1Name, file2Name ) {
    // implement code here
}
```

```bash
>> node copy.js file1 file2
```
