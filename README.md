# Coursera web frameworks
##Bootstrap Grid system

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
## Bootstrap Buttons
### Colors
Default colors:
* primary - Dark blue
* success - Green
* info - Light blue
* warning - Orange
* danger - Red

For ex.: text-primary, btn-success, alert-danger, bg-info 

### Button Classes
Button classes can be applied to &lt;a>, &lt;button> and &lt;input>. All these will get the button appearance but only &lt;button> can be used in _nav_ and _navbar_.

Examples:
```html
<div class="row"> 
	<div class="col-md-5 col-md-offset-1"> 
	   <button type="button" class="btn btn-primary btn-lg">Large Primary</button> 
	   <button type="button" class="btn btn-default">Default</button> 
	   <button type="button" class="btn btn-success btn-sm">Small Success</button> 
	   <button type="button" class="btn btn-info btn-xs">Extra Small Info</button> 
	   <button type="button" class="btn btn-link">Link</button> 
	</div> 
	<div class="col-md-3"> 
	   <button type="button" class="btn btn-warning btn-block">Warning</button> 
	   <button type="button" class="btn btn-danger btn-block" disabled="disabled">Danger</button>
	</div>
</div>
```

### Button Groups and Toolbars
```html
<div class="col-md-5 col-md-offset-1">
  <div class="btn-toolbar" role="toolbar">
    <div class="btn-group btn-group-sm" role="group">
      <button type="button" class="btn btn-primary">Primary</button>
      <button type="button" class="btn btn-default">Default</button>
      <button type="button" class="btn btn-success">Success</button>
    </div>
    <div class="btn-group btn-group-lg" role="group">
      <button type="button" class="btn btn-info">Info</button>
      <button type="button" class="btn btn-warning">warning</button>
      <button type="button" class="btn btn-danger">Danger</button>
    </div>
  </div>
</div>
  <div class="col-md-3">
    <div class="btn-group-ver]cal" role="group">
      <button type="button" class="btn btn-info">Info</button>
      <button type="button" class="btn btn-warning">Warning</button>
      <button type="button" class="btn btn-danger">Danger</button>
    </div>
  </div>
</div>
```
### Bootstrap Forms
form-horizontal
```html
<form class="form-horizontal" role="form">
  <div class="form-group">
    <label for="firstname" class="col-sm-2 control-label">First Name</label>
    <div class="col-sm-10">
      <input type="text" class="form-control" id="firstname"
          name="firstname" placeholder="Enter First Name">
    </div>
  </div>
</form>
```
#### Inline Form
<img src="data:image/png;base64,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"/>


```html
<form class="form-inline">
  <div class="form-group">
    <label class="sr-only" for="email">Email address</label>
    <input type="email" class="form-control" id="email" placeholder="Email">
  </div>
  <div class="form-group">
    <label class="sr-only" for="password">Password</label>
    <input type="password" class="form-control" id="password" placeholder="Password">
  </div>
  <div class="checkbox">
    <label><input type="checkbox">Remember me</label>
  </div>
  <button type="submit" class="btn btn-default">Sign in</button>
</form>
```
#### Input Group with Addons

<img src="data:image/png;base64,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"/>

```html
<div class="input-group"> 
   <div class="input-group-addon">(</div> 
   <input type="tel" class="form-control"
       id="areacode" name="areacode" 
       placeholder="Area code"> 
   <div class="input-group-addon">)</div> 
</div>
```