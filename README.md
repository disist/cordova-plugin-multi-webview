
# cordova-plugin-multi-webview
embeded webview for cordova app

This plugin is different with inappbrowser, You can load html page or external urls in the embeded webview, and control it directly.
It uses Crosswalk if available
Opens up to 6 inappBrowsers on screen

### Background
This plugin was originally commissioned by [ZeGenie Inc] [ze].

### Install
    cordova plugin add https://github.com/janpekarguru/cordova-plugin-multi-webview

### Method
  - cordova.EbWebview.open(n,url, param)
```sh    
app.webview = cordova.EbWebview.open(0,encodeURI('http://www.bing.com'), 'left='+app.left+',top='+app.top+',width=320,height=200');
```
n=browser number [0..5]
  - load(n,url)
  - show(n), hide(n)
  - setPosition(n,left, top)
  - setSize(n,width, height)
  - addEventListener(n,eventName, callback)
  - removeEventListenenr(n,eventName, callback)
  - executScript(n,injection, callback)

### Sample
[Here is sample javascript file] [sample]

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [sample]: <https://github.com/covernal/cordova-plugin-webview/blob/master/sample/index.js>
   [ze]: <http://www.zegenie.com>
