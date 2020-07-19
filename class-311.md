## [Intro to EJS in ExpressJS](https://www.youtube.com/playlist?list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)

### Getting Started

In the Terminal:
- npm init
- npm install --save express body-parser cors ejs

In Server.JS
-var express = require('express');
-var bodyParser = require('body-parser');
-var cors = require('cors');
-var path = require('path');

-var app = express();

-app.use(bodyParser());
-app.use(cors());

-app.set('views', path.join(__dirname, 'views'));
-app.set('view engine', 'ejs');

-app.get('/', function(request, response) {
  response.render('index');
})

-app.listen(8000, function() {
  console.log('heard on 8000);
})


**Path** is a core module of Node which joins two paths

***Then*** create a folder called 'views' containing a file called index.ejs

In Index.EJS

-Add test text such as `<h1>Hello World</h1>`

Last but not least, turn on the server!

---

### Evaluate an Injected Variable

response.render takes 3 parameters:
- string of the file name (view) 
- local variables
- callback

In Server.JS
- response.render('index', {
  foo: 'bar'
});

In Index.EJS
- `<h1>Hello <%= foo %></h1>`

Then turn on the server

<=% ejs %> works kind of like {{ handlebar }}
---

### Iterate/Loop Over an Array of Values

In Server.JS
- response.render('index', {
  people: [
    {name: 'dave'},
    {name: 'jerry'}
  ]
});

In Index.EJS
- `<ul>`
- `<% for(var person of people) { %>`
- `<li><% person.name %></li>`
- `<% } %>`
- `</ul>`

Turn on the browser and see both names render on the page in an UL

---

### If/Else Statements

In Index.EJS
- `<ul>`
- `<% for(var person of people) { %>`
- `<% if(person.name === 'dave') { %>`
- `<li><This is definitely <%= person.name %>!!!!</li>`
- `<% } else { %>`
- `<li><This is definitely not dave!!!  This is <%= person.name %></li>`
- `<% } %>`
- `<% } %>`
- `</ul>`

---

[Home](https://jchinzi.github.io/reading-notes/)