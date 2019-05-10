# fullcode
fullcode is one page codeing editor

# module
```
https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.46.0/codemirror.min.css
https://gnjo.github.io/fullcode/show-hint.css

https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.46.0/codemirror.min.js
https://gnjo.github.io/fullcode/mode.css.js
https://gnjo.github.io/fullcode/mode.js.js
https://gnjo.github.io/fullcode/mode.pug.js
https://gnjo.github.io/fullcode/show-hint.js
https://gnjo.github.io/fullcode/css-hint.js
https://gnjo.github.io/fullcode/javascript-hint.js

https://gnjo.github.io/terminal/terminal.css

```

#
```js
//key action
editor.setOption("extraKeys", {
  "Ctrl-Enter": function(cm) {
    var spaces = Array(cm.getOption("indentUnit") + 1).join(" ");
    cm.replaceSelection(spaces);
  }
});
```
```js
//autocomplete
https://codemirror.net/demo/complete.html
var editor = CodeMirror.fromTextArea(document.getElementById("code"), {
  lineNumbers: true,
  extraKeys: {"Ctrl-Space": "autocomplete"},
  mode: {name: "javascript", globalVars: true}
});

<link rel="stylesheet" href="../lib/codemirror.css">
<link rel="stylesheet" href="../addon/hint/show-hint.css">
<script src="../lib/codemirror.js"></script>
<script src="../addon/hint/show-hint.js"></script>
<script src="../addon/hint/javascript-hint.js"></script>
<script src="../mode/javascript/javascript.js"></script>
<script src="../mode/markdown/markdown.js"></script>

https://codemirror.net/addon/hint/
../
anyword-hint.js                                    24-Jul-2018 09:33                1681
css-hint.js                                        24-Jul-2018 09:33                2166
html-hint.js                                       09-Jan-2019 07:10               11417
javascript-hint.js                                 24-Jul-2018 09:33                6574
show-hint.css                                      28-Jun-2016 09:13                 623
show-hint.js                                       25-Apr-2019 06:12               17327
sql-hint.js                                        20-Mar-2019 08:11                9599
xml-hint.js                                        22-Mar-2019 07:33                5185

```
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
