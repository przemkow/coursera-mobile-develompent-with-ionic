# Multiplatform Mobile App Development with Web Technologies
 by The Hong Kong University of Science and Technology
 
 Mobile app development with Ionic framework course. Provided by Coursera.


### About
conFusion is an application which allow you to check information of your favourite restauran! Application give you possibility to check restaurant's menu, contact information and cheefs who are working for us. Moreover you have posibility to save or delete your favourite dishes in your personal favourite list.

### Features
* Simply REST API server with [json-server](https://github.com/typicode/json-server)
* Chosing profile picture during registration using build-in camera or android gallery
* Local notification, toast notification, vibration

### How to start
Using npm install all required modules:

    npm install gulp-cli -g
    npm install bower -g
    npm install cordova ionic -g
    npm install json-server -g


To start json-server go to /json-server directory and type:

    json-server --watch db.json

For *ionic server* you need to disable non compatible plugins. You can do that going to *app.js* and setting constant *DEVELOPMENT* to *true*

    5.  var DEVELOPMENT = true;

>Remember to set this option to *false* before deploying your application to real device, otherwise there will be no access to platform features like camera and galery.

### Server address configuration 
In *services.js* set proper address of your REST API. Using *json-server* it will be address of your local machine with port 3000.

    4.    .constant("baseURL","http://192.168.0.XXX:3000/")

### Run app
Start ionic server

    ionic serve --lab

or deploy application to real device. 
For android:

    ionic platform add android
    ionic build android
    ionic run android

### Used tools and technologies:
* HTML5
* CSS
* JavaScript
* Ionic Framework
* AngularJS
* SCSS
* Gulp
* Json-server
* Cordova
* ngCordova
