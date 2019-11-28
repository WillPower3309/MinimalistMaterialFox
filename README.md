# WillPower3309 Fork Readme

![](minimalMaterialFoxDemo.gif)

Optimizations Include:
1. Close tab button replaces favicon on hover (saving tab space and allowing for longer tab titles)
2. Fullscreen content is limited to the browser container (allowing for a video to play alongside an application in the same workspace)
3. Buttons only appear on hover (giving a minimal aesthetic)

## Installation
Follow the steps below.

If desired, you may have fullscreen content limited to the browser container (allowing for a video to play alongside an application in the same workspace, recommended for tiling window manager users) by changing the following in [about:config]:
Set ```full-screen-api.ignore-widgets``` to ```true```

# MaterialFox: Original Readme
*A Material Design-inspired userChrome.css theme for Firefox*

![Preview](https://user-images.githubusercontent.com/5405629/45172944-21d91900-b24a-11e8-8bc5-03814121b0de.png)
This theme is powered by blood, sweat, and coffee. If you like it, please consider helping out to support its continued development.

[![Buy me a coffee](https://svgshare.com/i/8Yd.svg)](https://www.buymeacoffee.com/n4ho5QX2l)

## What this does
Inspired by Google's Material Design and their latest Google Chrome UI, this theme turns your Firefox into a Material-styled web browser. The aim was to style the browser as closely as possible to the latest Google Chrome dev builds, where practical.

This is a userChrome.css theme, which means you must manually add it to your Firefox profile. The theme overrides certain browser styles. Currently, only the main UI is affected (settings pages, etc. are not). More elements of the UI may be styled in the future.

## Installation
Some steps involve accessing the about:config page. You can get there by typing it into your urlbar.

### Mandatory instructions
1. Copy the chrome folder into your Firefox profile directory. To find your profile directory, go to about:support. Alternatively, you can symlink your chrome folder instead of copying.
2. [about:config] Set ```toolkit.legacyUserProfileCustomizations.stylesheets``` to ```true``` (default is ```false```).
3. [about:config] Set ```svg.context-properties.content.enabled``` to ```true``` (default is ```false```).
4. Restart Firefox.

### Recommended instructions
Add space above tab bar:
* Right click on toolbar -> Customize.
* Check Drag Space checkbox.

Replicate Chrome behaviour for clipped tabs:
* [about:config] Set ```browser.tabs.tabClipWidth``` to ```83``` (default is ```144```).

Allow tabs to shrink more; tabs in overflow will look the same as pinned tabs:
* [about:config] Add new entry ```materialFox.reduceTabOverflow``` with value ```true```.

Replicate Chrome's "Not Secure" text on HTTP:
* [about:config] Set ```security.insecure_connection_text.enabled``` to ```true```.

## Please note
* Linux is not frequently tested; last tested on 21/05/2019.
* Some customisation settings may no longer work (such as compact/touch density).
* Some custom themes may clash with address bar.
