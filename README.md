
# cordova-plugin-multi-webview
embeded webview for cordova app

This plugin is different with inappbrowser, You can load html page or external urls in the embeded webview, and control it directly.
It uses Crosswalk if available
Opens up to 6 inappBrowsers on screen

### Background
This plugin was originally commissioned by [ZeGenie Inc] [ze].

### Install
    cordova plugin add https://github.com/janpekarguru/cordova-plugin-multi-webview
### Remove
    cordova plugin remove cordova-plugin-ebwebview

Add whis plugin so iOS will use WkWebView with this plugin
https://github.com/apache/cordova-plugin-wkwebview-engine

### Method
  - cordova.EbWebview.open(n,url, param)
```sh    
app.webview = cordova.EbWebview.open(0,encodeURI('http://webkam.com'), 'left=0,top=0,width=320,height=200');
```
n=browser number [0..5]
  - load(n,url)
  - show(n), hide(n)
  - setPosition(n,left, top)
  - setSize(n,width, height)
  - addEventListener(n,eventName, callback)
  - removeEventListenenr(n,eventName, callback)
  - executScript(n,injection, callback)
  - hasHistory: function (n,callback) 
  - goBack: function (n)
  - getScreenshot: function (n,quality, callback)
  - addEventListener: function (n,eventname,f)
  - removeEventListener: function(n,eventname, f)
  - executeScript: function(n,injectDetails, cb)
  - insertCSS: function(n,injectDetails, cb)
     
	




   
   
   [ze]: <http://www.zegenie.com>
