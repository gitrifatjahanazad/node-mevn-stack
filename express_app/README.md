# NPM Install
*npm init* to initialize the project. To save later installed packages use but currently only npm install do the save for you,
```
npmm install <package-name> --save
```

to save it globally,

```
npmm install <package-name> -g
```

# About Express
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

node mon is used to automatically run build on any change item and serve the changes to server.

[Check the structure](folder_structure.md)