# fullcode
fullcode is one page codeing editor

# 
```js
//mode.pug.js
https://codemirror.net/mode/pug/index.html
var editor = CodeMirror.fromTextArea(document.getElementById("code"), {
mode: "pug",
lineNumbers: true
});
```
```js
//mode.css.js
https://codemirror.net/mode/css/index.html
var editor = CodeMirror.fromTextArea(document.getElementById("code"), {
mode :"css",
extraKeys: {"Ctrl-Space": "autocomplete"}
});
```
```js
//mode.js.js
https://codemirror.net/mode/javascript/index.html
var editor = CodeMirror.fromTextArea(document.getElementById("code"), {
mode:"js",

  lineNumbers: true,
  matchBrackets: true,
  continueComments: "Enter",
  extraKeys: {"Ctrl-Q": "toggleComment"}
});
```
