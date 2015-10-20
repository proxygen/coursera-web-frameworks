Coursera web frameworks 

### Viewport

* Ensures that the screen width is set to the device width and the content is rendered with this width in mind

```html
<meta name="viewport" content="width=device-width,initial-scale=1">
```

### Bootstrap Grid
* Four classes available: xs, sm, md and lg

|&nbsp;|Extra small (&lt;768px)|Small (&ge;768px)|Medium (&ge;992px)|Large (&ge;1200px)
|---|---|---|---|---
|Tipical device|Mobile phones|Tablets|Laptops|Desktops
|Grid Behavior|Horizontal|Collapsed to start, horizontal above vrekpoints|Collapsed to start, horizontal above vrekpoints|Collapsed to start, horizontal above vrekpoints
|Container width|None(auto)|750px|970px|1170px
|Class prefix|.col-xs-|.col-sm-|.col-md-|.col-lg-
|# of columns|12|12|12|12
|Column width|Auto|~62px|~81px|~97px
|Gutter width|30px (15px on each side)|30px (15px on each side)|30px (15px on each side)|30px (15px on each side)

* Each row in Bootstrap grid system is divided to 12 columns
* Use the classes .col-xs-*, .col-sm-*... for defining the layouts for the various screen sizes
* Specify how many columns each piece of content will occupy within a row, all adding up to 12 or a multiple thereof
* A small white margin between each piece of content, called "gutter"

```html
<div class="container">
    <div class="row">
        <div class="col-sm-5"></div>
        <div class="col-sm-7"></div>
    </div>
</div>
```
