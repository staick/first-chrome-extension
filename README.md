# How to create a chrome extension?
Reference: [How to Create Your Own Google Chrome Extension](https://www.freecodecamp.org/news/building-chrome-extension/)

As a chrome user, we often use some chrome extension, such as Tampermonkey, Office, etc.

But, how can we make our own chrome extension?

The chrome extension is just like a web page and is consist of HTML, CSS, JavaScript, etc.

Every extension has a JSON-formatted mainifest file, named `manifest.json`, that provides important information.

Then how to create a manifest  file?

You can refer to the [Manifest file format](https://developer.chrome.com/docs/extensions/mv3/manifest/).

Our `manifest.json` file is like this:
```json
{
    "name": "Covid-19 Stats UK",  // The name of the extension
    "version": "1.0.0",  // The version of the extension
    "description": "latest covid data of UK",  // The description of the extension
    "manifest_version": 3,  // The manifest version
    "author": "Staick",  // The name of the author
    "icons": {
        "48": "images/icons/icon48.png",
        "96": "images/icons/icon96.png"
    },  // The icons of the extension
    "action": {
        "default_popup": "index.html",
        "default_title": "Latest Covid Report"  // show in tooltip
    }
}
```
So far, the extension is finish, we can open the chrome browser, type `chrome://extensions/` in the address bar(or use other methods) to manage the chrome.

Then click the "Load unpacked" button, and select the folder.

Then you can use it!