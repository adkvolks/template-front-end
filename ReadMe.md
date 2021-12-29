# Front-end Start Kit

Starter kit is a set of NPM tools for front-end developers with some default CSS (using SASS) and JavaScript to get the project started. 

```git clone https://github.com/adkvolks/template-front-end```

## SASS/CSS

This uses the SASS/SCSS extension language for CSS. The ```src/scss``` is broken up into six folders for organizational purposes.  Create a new file within folder and then include the newly created file within the master ```.scss``` file within the folder. ```.scss``` files do not need to include extension where ```.css``` do need to. 

Example for html.scss: ```@import "html";```
Example for html.css:  ```@import "html.css";```

- ```src/scss/0-plugins``` Directory to put any framework and third-party plugins.
- ```src/scss/1-helpers``` Directory to put helper files like variables and configs.
- ```src/scss/2-base``` Directory to put base SCSS information like default HTML.
- ```src/scss/3-layout``` Directory to put global layout files like header and footer.
- ```src/scss/4-modules``` Directory to put modules like cards and smaller components.
- ```src/scss/5-templates``` Directory to put larger templates like call to actions. 

The SCSS files are all compiled into a single ```/assets/css/styles.min.css``` file where it is also minified. To compile the SCSS files, run the following command:

```npm run sass-compile```

You can also have a watch for everytime you modify a SCSS file.

```npm run watch```
(please note this also watches JS files)

## JavaScript

The ```src/js``` is broken up into four folders for organizational purposes. Create a new file within the folder and then include the newly created file within the master ```.js``` file of that folder. 

Example for scripts.js: ```// @import:(scripts.js)```

- ```src/js/0-plugins``` Directory to put any framework or third-party plugins.
- ```src/js/1-helpers``` Directory to put any helper files like variables and configs.
- ```src/js/2-base``` Directory to put any base JavaScript.
- ```src/js/3-modules``` Directo to put any JavaScript modules.

The JavaScript fliles are compiled into a single ```/assets/js/scripts.min.js``` file where it is also minified and mangled. To compile, run the following command:

```npm run js-compile```

You can also have a watch for everytime you modify a JS file.

```npm run watch```
(please note this also watches SCSS files)