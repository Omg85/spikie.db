<div align="center">

  <p>
    <a href="https://www.npmjs.com/package/spikie.db"><img src="https://img.shields.io/npm/v/spikie.db?maxAge=3600" alt="NPM version" /></a>
<a href="https://www.npmjs.com/package/spikie.db"><img src="https://img.shields.io/npm/dt/spikie.db?maxAge=3600" alt="NPM downloads" /></a>
  </p>
  
  <p>
    <a href="https://www.npmjs.com/package/spikie.db"><img src="https://nodei.co/npm/spikie.db.png?downloads=true&stars=true" alt="NPM Banner"></a>
  </p>
</div>

## Installation
```sh
$ npm install spikie.db
```

<h1>DISCORD.JS</h2>

## Example

# spikieDB
## 1. Importing the package 
 ```js 
 const { spikieDB } = require("spikie.db"); // or import { spikieDB } from "spikie.db"; 
 ``` 
## 2. Establishing and exporting spikieDB 
 ```js 
 const db = new spikieDB({ uri: "your mongodb connection string", }); module.exports = db; 
 ```
## 3. Example on using it 
```js 
const db = require("./db.js"); // replace db.js with your file path to the setup of spikieDB db.set("numbers", "123"); 
```
## Methods 
### .set 
```js 
// saves data to database db.set("key", "value"); 
```
### .get 
```js 
// gets value from key db.get("key"); // returns => value 
```
### .has 
```js 
// returns boolean db.has("key"); // returns => true 
``` 
### .delete 
```js 
// deletes data db.delete("key"); // checking for data db.has("key"); // returns => false 
```