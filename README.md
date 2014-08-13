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
___

```html
<!DOCTYPE html>
<html>
    <head>
    </head>
    <body>

        <a href="update.php" data-ajax>Load Ajax (without response)</a>

        <a href="file.php" data-ajax="#ajax-content">Load Ajax (load and view response)</a>

        <div id="ajax-content"></div>

        <script src="jquery.js"></script>
        <script src="jquery.ajax-helper.js"></script>
        <script>
            $('body').ajaxHelper();
        </script>
    </body>
</html>
```
