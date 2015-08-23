# download-svg

A script to download a SVG image (e.g. a d3 visualization) embeding related css stylessheets

 It is not interesting to include every stylesheets in the SVG so **only** stylesheets with ``title="embed-svg"`` will be used. 

```html
<link rel="stylesheet" href="needed-stylesheet.css" title="embed-svg">
```

### Example of use

```javascript
var downloadSVG = require("download-svg");   // I use webpack, but not needed
var svg = document.getElementById("MySVG");
downloadSVG(svg);
```

----

Based on https://github.com/NYTimes/svg-crowbar
