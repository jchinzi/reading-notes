### Questions:

**Why would you want to run JavaScript code outside of a browser?**

Many reasons - node.js allows you to use JavaScript outside of the browser by building a node app. 

**What is the difference between a module and a package?**

A **package** is a file or directory described by a package.json
A **module** is a file or directory in the node_modules directory that can be loaded by the Node.js require() function.

All packages are also modules. However, because a module *may* have a package.json, a module can be a package, but not *all* modules are packages.

**What does the node package manager do?**

The node package manager puts modules in place so that node can find them, and manages dependency conflicts intelligently

**Provide code snippets showing 3 different ways to export a function from a node module**

Export Function
```
module.exports = function (content) { 
    console.log(content);
};
```
Export Function as a Class
```
module.exports = function (var1, var2) {
    this.var1 = var1;
    this.var2 = var2;
    this.allData = function () { 
        return this.var1 + ' ' + this.var2;
    }
}
```
Load Module from a Folder
```
var example = require('./folder/file.js');
```

(Adapted from https://www.tutorialsteacher.com/nodejs/nodejs-module-exports)

### Definitions

|Term|Definition|
|:--|--:|
|ecosystem|A managed lifecycle and dependency injection for your application components  (https://www.npmjs.com/package/ecosystem)|
|Node.js|An open source server environment (https://www.w3schools.com/nodejs/nodejs_intro.asp)|
|V8 Engine|Google's open source high-performance JavaScript and WebAssembly engine - used in Chrome and Node.js (https://v8.dev/)|
|module|Any file or directory in the node_modules directory that can be loaded by the Node.js require() function|
|package|A file or directory that is described by a package.json|
|node package manager(npm)|World's largest software registry - a way to reuse code from other developers and to share your code with other developers|
|server|A device that accepts and responds to requests made over a network - the server serves the *client* (https://www.computerhope.com/jargon/s/server.htm)|
|environment|The state of a computer, determined by a combination of software, basic hardware, and which programs are running (https://www.computerhope.com/jargon/e/environm.htm#:~:text=The%20term%20environment%20refers%20to,utilizing%20the%20Windows%20operating%20system.)|
|interpreter|A method of converting source code into machine code - interpreters translate programs one statement at a time and do not generate intermediate object code.  They are memory efficient, but comparatively slower than compilers (https://www.programiz.com/article/difference-compiler-interpreter)|
|compiler|A method of converting source code into machine code - compilers translate programs as a whole after scanning the entire program.  They do generate intermediate object code, making them less memory efficient, but comparatively faster than interpreters|

---

[Home](https://jchinzi.github.io/reading-notes/)