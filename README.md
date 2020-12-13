# DB-script
---

# set up

we need:

* `package.json`
* `server.js` or `index.js`

**package.json:** :pager:

```js
{
    "name": "-asdf",
    "version": "1.0.0",
    "description": "",
    "main": "server.js",
    "scripts": {
      "start": "node server.js"
    },
    "engines": {
      "node": "12.x"
    },
    "author": "",
    "license": "ISC",
    "dependencies": {
      "dbd.js": "^1.0.1"
    }
  }
```
**server.js:**

```js
const dbd = require("dbd.js")
 
const bot = new dbd.Bot({
token: "TOKEN", 
prefix: "PREFIX" 
})
 
bot.onMessage()
 
bot.command({
name: "ping", 
code: `Pong! \`$ping\`` 
})

```

---

# Stuff

**code:** :computer: 

```js
bot.command({
name: "NAME", 
code: `CODE` 
})
```

**variables:** :package:

```js
bot.variables({
  Name: "NAME",
  Name2: "VALUE"
})
```

**status:** :bulb:

```js
bot.status({
  text: "TEXT",
  type: "PLAYING",
  time: 12
})
```

# Reminder
---
* To install the package: `npm install dbd.js`
* To start it: `node .`

