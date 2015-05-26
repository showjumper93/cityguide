# Plugins
When you want to add plugins for use in you designs remember that they need to be complied by the Koala App. Make sure you have Koala up and running and that the main.js and plugin.js files are set to auto compile.

## console-errors.js
To utilize the console-errors.js file add the following line of code to your plugins.js file.
// @koala-prepend "vendor/console-errors.js"

## scroll.js
To utilize the console-errors.js file add the following line of code to your plugins.js file .
// @koala-prepend "vendor/scroll.js"

## jellyfish.js
To utilize the jellyfish.js file add the following line of code to your plugins.js file.
// @koala-prepend "vendor/jellyfish.js"

You will also need to add the following lines of code to your main.js file.
// init jellyfish.js
jellyfish.init({
    icon: 'img/loading.svg', // Image to display when image is loading
    offset: 0, // How far below fold to begin loading images
    type: 'img', // Type of content to load ('img' or 'iframe')
    callbackBeforeIcons: function ( wrappers ) {}, // Function to run before icon is loaded
    callbackAfterIcons: function ( wrappers ) {}, // Function to run after icon is loaded
    callbackBeforeContent: function ( wrapper ) {}, // Function to run before content is loaded
    callbackAfterContent: function ( wrapper ) {} // Function to run after content is loaded
});

