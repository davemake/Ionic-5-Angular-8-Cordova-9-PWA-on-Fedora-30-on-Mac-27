# Ionic-5-Angular-8-Cordova-9-PWA-on-Fedora-30-on-Mac-27
Getting a PWA to work on desktop did not work out-of-the box for my situation. This is how I got it to work! Good luck with your project!


# CONVERT MOBILE APP TO PWA DESKTOP APP

Ionic 5 Angular 8 Cordova 9 PWA on Fedora 30 on Mac 27

Why?
(1) Instant refresh on change, great for debugging in a hurry!
(2) Resources go from 50 mb to 18,000! If your app is crashing, this may help!
(3) Desktop will stay on all the time, while mobile goes to sleep at the most inconvenient times!

Fedora 30 on Mac 27 inch with 8 mb ram 500 mb drive

$ ionic info

Ionic:

   Ionic CLI                     : 5.4.5 (/home/dave/.nvm/versions/node/v10.15.0/lib/node_modules/ionic)
   Ionic Framework               : @ionic/angular 4.11.3
   @angular-devkit/build-angular : 0.801.3
   @angular-devkit/schematics    : 8.1.3
   @angular/cli                  : 8.3.20
   @ionic/angular-toolkit        : 2.0.0

Cordova:

   Cordova CLI       : 9.0.0 (cordova-lib@9.0.1)
   Cordova Platforms : android 8.1.0, browser 6.0.0
   Cordova Plugins   : cordova-plugin-ionic-keyboard 2.2.0, cordova-plugin-ionic-webview 4.1.3, (and 11 other plugins)

Utility:

   cordova-res : 0.5.2 (update available: 0.8.1)
   native-run  : 0.2.1 (update available: 0.3.0)

System:

   Android SDK Tools : 26.1.1 (/home/dave/Android/Sdk)
   NodeJS            : v10.15.0 (/home/dave/.nvm/versions/node/v10.15.0/bin/node)
   npm               : 6.13.2
   OS                : Linux 5.3

Caution! Do NOT try this on a non-linux computer or prepare spend days and nights tearing your hair out and getting nowhere!

Install chromium or chromium-vaapi or some other version of chrome that you can use just for debugging.

Add this extension to disable CORS permissions so we can connect to the api:
https://chrome.google.com/webstore/detail/moesif-orign-cors-changer/digfbfaphojjndkpccljibejjbppifbc

Run these commands from app:

$ npm uninstall -g @angular/cli

$ npm install -g @angular/cli

$ ng -v

$ ng add @angular/pwa --project app

$ ionic cordova platform add browser

$ ionic cordova run browser

$ cordova plugin add cordova-plugin-browsersync

Get this error? "Using "requireCordovaModule" to load non-cordova module "q" is not supported. Instead, add this module to your dependencies and use regular "require" to load it."



When browser pops open, copy url and move to chromium browser, turn on CORS disabling at upper right of window.

Press: control-shift-C to open debugging console

Press: control-shift-I to close debugging console

Note: If errors arise, copy them, search the internet for solutions and apply!

Take breaks every 25 minutes or suffer!

LONG LIVE LINUX----YOU MAKE LIFE FUN AGAIN----YOU NEVER TELL ME WHAT TO DO!
