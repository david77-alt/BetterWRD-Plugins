
# Creating & Sharing Plugins for BetterWRD
BetterWRD Plugins allow users to run scripts made by other users that enhance WeAreDevs even more by adding fresh new features!\
It's easy to create & share plugins! This tutorial will teach you everything you have to know.


### Getting Started
First things first, create a file named `plugin.bwrd.js`. You'll use this file to load the plugin on BetterWRD.\
This is how the script should look like:

```js
/*
    @name My First Plugin
    @version 1.0.0
    @description My cool plugin.
    @author You
    @source https://raw.githubusercontent.com/davve77/testing/main/firstPlugin.bwrd.js
*/


// Your plugin's script:
console.log("Hello!");
```

The `@source` is your plugin's update link. It has to be a raw GitHub URL.


&nbsp;
### Using BetterWRD's own Plugin API (optional)
The API currently has 5 simple but useful functions:
```js
bwrd.injectStyle("style");
bwrd.injectScript("script");
bwrd.getSettings(); // Returns the plugin's settings in JSON format.
bwrd.setSettings({"proeprty": "value"});
bwrd.getUser().then(info => console.log(info)); // Prints the user's name, avatar, reputation, join date etc.
```


&nbsp;
### Distributing your Plugin to the community
This file is work-in-progress.
