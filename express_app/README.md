# NPM Install Notes
*npm init* to initialize the project. To save later installed packages use but currently only npm install do the save for you,
```
npmm install <package-name> --save
```

to save it globally,

```
npmm install <package-name> -g
```

### About Express
*npm install express* does not avail express command after 4 version release of express. Also youy need to install express-generator.
```
npm install express-generator
express <express scaffold location>
```

then you need to run npm install. As more new packages are added in package.json file.
```
"cookie-parser": "~1.4.3",
"debug": "~2.6.9",
"express": "~4.16.0",
"http-errors": "~1.6.2",
"jade": "~1.11.0",
"morgan": "~1.9.0"
```
[Check the structure](folder_structure.md)

### About nodemon package
nodemon is used to automatically run build on any change item and serve the changes to server.

### About "npm start" vs "node app.js"
the express template can be run from the app.js file. if there exists this line of code,
```js
app.listen(3000, function() { console.log('listening on 3000') })
```

but remember if in www file same sort of line like
```js
server.listen(port);
```
then it will clash with the app.js extra line added. The thing is this is used to run the server. If one command runs the server and occupy a port then another same command tries to do the same and the later run finds that the port is already in use.