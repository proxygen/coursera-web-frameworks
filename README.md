# Coursera web frameworks

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

### Navbar
#### Normal Navbar Example:
```html
<nav class="navbar navbar-default" role="navigation">
  <div class="container">
    <div class="navbar-header">
      <a class="navbar-brand" href="#">Ristorante Con Fusion</a>
    </div>
    <ul class="nav navbar-nav">	
      <li class="ac9ve"><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Menu</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
    <ul class="nav navbar-nav navbar-right"
      <li><a href="#">Sign in</a></div>
      <li><a href="#">Contact</a></div>
    </ul>
  </div>
</nav>
```
#### Responsive Navbar Example:
```html
<nav class="navbar navbar-default" role="navigation">
  <div class="container">
    <div class="navbar-header">
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbardata" aria-expanded="false" aria-controls="navbar">
        <span class="sr-only">Toggle navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      ...
    </div>
    <div id="navbardata" class="navbar-collapse collapse">
      <ul class="nav navbar-nav">...</ul>
    </div>
  </div>
</nav>
```
#### Positioning Navbar:
* .navbar-fixed-top and .navbar-fixed-bottom<br>
Fixed to top/bottom of window and does not scroll
* .navbar-static-top<br>
Full-width navbar at the top that scrolls
* .navbar-inverse<br>
Dark navbar with light text (opposite to .navbar-default)

#### Dropdown
```html
<li class="dropdown">
  <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false"><span class="caret"></span></a>
  <ul class="dropdown-menu">
    <li><a href="#">Appetizers</a></li>
    <li><a href="#">Drinks</a></li>
    <li role="separator" class="divider"></li>
    <li class="dropdown-header">Specials</li>
    <li><a href="#">Lunch Buffet</a></li>
    <li><a href="#">Weekend Brunch</a></li>
  </ul>
</li>
```
### Icon Fonts
Icon fonts is set of symbols and glyphs and can be used just like regular fonts.
```html
<span class="glyphinco glyphicon-home" aria-hidden="true"></span> <!-- Glyphicons -->
<i class="fa fa-phone"> <!-- Font Awesome -->
<a class="btn btn-social-icon btn-facebook" href="http://www.facebook.com/profile.php?id="><i class="fa fa-facebook"></i></a> <!-- Bootstrap-social -->
```