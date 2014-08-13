JQuery Ajax Helper
===========

JQuery Plugin to use ajax from html attributes, without write javascript code.

Usage
---

Include the javascript files and init de plugin:

```html
<!DOCTYPE html>
<html>
    <head>
    </head>
    <body>
        <script src="jquery.js"></script>
        <script src="jquery.ajax-helper.js"></script>
        <script>
            $('body').ajaxHelper();
        </script>
    </body>
</html>
```

Load Ajax Content
---

```html
<a href="update.php" data-ajax>Load Ajax (without response)</a>

<a href="file.php" data-ajax="#ajax-content">Load Ajax (load and view response)</a>

<div id="ajax-content"></div>
```

Submit Ajax Forms
---

```html
<form data-ajax="#ajax-content" method="post" action="post.php">
<input type="text" name="form[name]" />
<input type="submit" value="Send" />
</form>

<div id="ajax-content"></div>
```

Options
===

*   **data-ajax**: markup for handle the plugin, the value is optional, and if setted, is used as selector for show response in these element.
*   **data-before**: (optional) a plugin function called before execute ajax (arguments: element, event, container), if this method return false, de ajax is not called.
*   **data-after**: (optional) a plugin function called after execute ajax (arguments: response, element, container).
*   **data-url**: (optional) if the element is not a link, this value is used for get the url.
