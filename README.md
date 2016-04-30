# Mafia

Mafia is built on an Ionic foundation. The structure of the project was generated by Ionic's build functions. We populated the necessary files with the functionality that was desired for the app. Within the ./mafiaApp/www directory exists files that are responsible for the execution of the app. Within his directory, ./lib contains all Ionic-generated code that acts as the default for the project. The img folder contains images used within the app. Our written code for this project is found within the templates and js directories. 

The files that we built followed the MVC design architecture. The Model may be found in ./mafiaApp/www/js/services.js. The Controllers may be found in ./mafiaApp/www/js/controllers.js. The Views are all found within the templates directory, one per page in the app. 

# Installation and Execution

In order to run our app, the Ionic framework and its dependencies must be installed. To do so, make sure you first have Node.js installed on your machine and then run the following lines from your command line:

$ sudo npm install -g cordova <br>
$ sudo npm install -g ionic

Now you should have Ionic and its dependencies installed on your machine. In order to run the app, run the following line from within the mafiaApp directory found in this folder:

$ ionic serve -l

This will emulate the app within your internet browser. You will see two versions of the app, one for iOS and one for Android. Both work in the same way. Refreshing the page acts in the same way as closing out of the app on your mobile device. Enjoy playing Mafia!

# Testing

Our testing suite is built on the Karma and Jasmine frameworks. You will have to install Karma and its dependencies in order to run our test suite. Our test suite can be found in mafiaApp/tests/unit-tests/services/serviceTests.js. Karma is the test Runner and Jasmine is the testing framework. Install Karma by running the following commands within the mafiaApp directory in this folder:

$ sudo npm install karma --save-dev <br>
$ sudo npm install karma-jasmine --save-dev <br>
$ sudo npm install -g karma-cli

If you encounter the error "Cannot find module: 'jasmine-core'", run the following line:

$ sudo npm install -g jasmine-core

Now you should be able to run the test suite. To do so, go to ./tests and run the following command:

$ karma start  unit-tests.conf.js

Refer to this link if you encounter errors, but be weary of overwriting project code:
http://gonehybrid.com/how-to-write-automated-tests-for-your-ionic-app-part-2/

If the testing suite still doesn't work, check the screenshots in the testingImages folder at the root of the project. 

Enjoy the testing!
