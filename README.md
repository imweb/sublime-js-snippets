# JavaScript Snippets for Sublime

## description

This is a JavaScript Snippets package for [IMWeb team](https://github.com/imweb), it unifies the js snippets for IMWeb team.<br>
The snippets of this package make a standard list in [Code Guide of IMWeb team](http://imweb.github.io/CodeGuide/#snippets)

## Install

To install through [Package Control](http://wbond.net/sublime_packages/package_control),
search for **JavaScript Snippets for IMWeb**. If you still don't have Package Control in Sublime Text, [go get it](http://wbond.net/sublime_packages/package_control/installation).
It's pure awesomeness.

If you prefer to install it manually, you can download the package and put it inside your `Packages` directory. It should work but will not update automatically.

## Console

### [cd] console.dir

```javascript
console.dir(${1:obj});
```

### [cl] console.log

```javascript
console.log(${1:obj});
```

## EJS

### [=fo] <% for %>

``` javascript
<% for (var ${1:i} = ${2:0}, ${3:l} = ${4:arr}.length; ${1:i} < ${3:l}; ++${1:i}) { %>
    ${5}
<% } %>
```

### [=if] <% if %>

``` javascript
<% if(${1:expr}) { %>
    ${2}
<% } %>
```

### [=] <%= %>

```javascript
<%${1:=} ${2:expr} %>
```

## For

### [fe] forEach

```javascript
${1:myArray}.forEach(function(${2:elem}, ${3:index}) {
    ${4}
});
```

### [fi] for...in

```javascript
for (${1:prop} in ${2:obj}) {
    if (${2:obj}.hasOwnProperty(${1:prop})) {
        ${3}
    }
}
```

### [fo] for

```javascript
for (var ${1:i} = ${2:0}, ${3:l} = ${4:arr}.length; ${1:i} < ${3:l}; ++${1:i}) {
    ${5}
}
```

## Function

### [fn] function

```javascript
function ${1:functionName}(${2:arguments}) {
    ${3:// body...}
}
```

### [afn] anonymous function

```javascript
function(${1:arguments}) {
    ${2:// body...}
}
```

### [apply] apply

```javascript
${1:functionName}.apply(${2:context}, [${3:arguments}]);
```

### [call] call

```javascript
${1:functionName}.call(${2:context}, ${3:arguments});
```

### [iif] immediately-invoked function expression

```javascript
(function(${2:win}) {
    ${3:// body...}
})(${1:window});
```

### [ofn] function as a property of an object

```javascript
${1:functionName}: function(${2:arguments}) {
    ${3:// body...}
},
```

## If

### [ife] if...else

```javascript
if (${1:expr}) {
    ${2:// if body...}
} else {
    ${3}
}
```

## Jquery

### [jvt] get $this

```javascript
var \$this = \$(this);
```

### [jve] get jquery element

```javascript
var \$${1} = \$('${2}');
```

### [jvd] get data

```javascript
var ${1:cid} = \$${2:this}.data('${3:cid}');
```

### [jext] $.extend

```javascript
\$.extend(${1});
```

### [jat] $.attr

```javascript
\$${1:this}.attr('${2}'${3});
```

### [jcss] $.css

```javascript
\$${1:this}.css({${2}});
```

### [jwi] $.width

```javascript
\$${1:this}.width(${2});
```

### [jhe] $.height

```javascript
\$${1:this}.height(${2});
```

### [jsh] $.show

```javascript
\$${1:this}.show();
```

### [jhi] $.hide

```javascript
\$${1:this}.hide();
```

### [jac] $.addClass

```javascript
\$${1:this}.addClass('${2}');
```

### [jrc] $.removeClass

```javascript
\$${1:this}.removeClass('${2}');
```

### [jon] $.on

```javascript
\$${1:this}.on('${2:click}', ${3}function(e${4}) {
    ${5:// body...}
});
```

### [jtri] $.trigger

```javascript
\$${1:doc}.trigger('${2:eventType}'${3});
```

## MISC

### [vs] save context

```javascript
var ${1:self} = this;
```

### [al] alert

```javascript
alert('${1:msg}');
```

### [de] debugger

```javascript
debugger;
```

### [ret] return

```javascript
return ${1:this};
```

### [ni] new Image

```javascript
new Image().src = '/${1}';
```

## Node

### [re] require

```javascript
require('${1:module}');
```

### [rea] require.async

```javascript
require.async(['${1:moduleName}'], function(${2:module}) {
    ${3:// body...}
});
```

### [me] module.exports

```javascript
module.exports = {${1}};
```

## Timer

### [st] setTimeout

```javascript
setTimeout(function() {
    ${2:// body...}
}, ${1:delay});
```

### [si] setInterval

```javascript
setInterval(function() {
    ${2:// body...}
}, ${1:delay});
```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

Check [Releases](https://github.com/imweb/sublime-js-snippets/releases) for detailed changelog.

