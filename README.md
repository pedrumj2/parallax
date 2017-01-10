# parallax
a javascript plugin that will generate a parallax effect

#usage
Creates a sliding parallax effect.

1- assign an ID to the img tag

2- assign an ID to the parent div. This is div with the content that will slide over the image.

**Example:**
```html
<div id = "parallexWrapper">
    <img id = "parallex1" src = "mid3.jpg">

    </img>
</div>
```

3- Call the plugin as shown below once the window loads:
```javascript
  var parallex = new Parallax("mid3_wrapper", "parallex1");
```

4- If there are more than one image just call the line above for each one.

5- Call this on the onscroll event of the window:
```javascript
parallex.create_effect()
```

**Note:** Make sure image is properly aligned vertically. The top of the image should be above the top of its parent (with overflow:hidden). If this is not set propertly the image will always be below the bottom of the screen.
