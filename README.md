
# Creating & Sharing Plugins for BetterWRD
BetterWRD Plugins allow users to run scripts created by other users to enhance WeAreDevs even more by adding fresh new features!\
It's easy to create & share plugins. This tutorial will teach you everything you have to know.


### Getting Started
First things first, create a file named `plugin.bwrd.js`. You'll use this file to load the plugin on BetterWRD (name must end with `.bwrd.js`).\
This is how the script should look like:

```js
/*
    @name My First Plugin
    @version 1.0.0
    @description My cool plugin.
    @author You
    @source https://raw.githubusercontent.com/davve77/BetterWRD-Plugins/main/plugins/plugin.bwrd.js
*/


// Your plugin's script:
console.log("Hello!");
```

The `@source` is your plugin's update link. It has to be a raw GitHub URL.


&nbsp;
### Using BetterWRD's own Plugin API (optional)
The API currently has 6 simple but useful functions:
```js
bwrd.injectStyle("style");
bwrd.injectScript("script");
bwrd.getSettings(); // Returns the plugin's settings in JSON format.
bwrd.setSettings({"proeprty": "value"});
bwrd.getVersion(); // Returns the currently installed BetterWRD version number.
bwrd.getUser().then(info => console.log(info)); // Prints the user's name, avatar, reputation, join date etc.
```
Yes, this is more of a library than an API.


&nbsp;
### How do Plugins get updated?
BetterWRD periodically checks for plugin updates every 3 hours.\
If the `@version` number on GitHub is different than the one stored on the user's browser (and of course if the `@source` URL is valid), BetterWRD will automatically ask the the user to update the plugin with a fixed box at the bottom of the page.

![image](https://cdn.discordapp.com/attachments/800294579856605204/937412167966261248/unknown.png)

Or of course, you can do it manually on the Plugins page.

&nbsp;
### Distributing your Plugin to the community
This section is work-in-progress.
