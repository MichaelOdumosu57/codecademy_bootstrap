# Getting Started with Bootstrap
* Bootstrap simplifies the layout of a website using a grid system


## Intro to the Grid
bootstrap is based like this
```html
<div class="container">
  <div class="row">
    <div class="col">
      <!-- A column inside a row inside a container! -->
    </div>
  </div>
</div>
```


* uses classes to apply css rulesets
__container__ give a width relative to the user screen
__container-flud__ fillls the screen

* row will take up entire width of container
* columns are the immediate children of rows
* row will accomodate 12 columns

* use col-auto when the width of the parent should be determined by its children

## Bootstrap Breakpoints
Bootstrap categorizes screen sizes into 5 categories or as breakpoints: extra small, small, medium, large, and extra large. 
![1659280030115](image/README/1659280030115.png)

* so you can use col-sm-4, col-lg-6, to change the size at different breakpoints
* however breakpoints mean "on this screen size and greater"
* a row will make a child stretch to fill its parent column

# Bootstrap Utilities and Components
* bootstrap is more than just sizing

[Bootstrap color docs](https://getbootstrap.com/docs/4.2/utilities/colors/)

[Bootstrap font docs](https://getbootstrap.com/docs/4.2/utilities/text/#font-weight-and-italics)

* use nav and nav-link for navigation
* for button classes you always need "btn"

## Collapsing a Component
[refer to](bootstrap_collapse_html_accessibility.index.html) 
how toggle is done html
```html
    <button class="btn btn-link" aria-expanded="false" aria-controls="seedSpecial" data-target="#seedSpecial"  data-toggle="collapse">
      Gearing to Grow?
    </button>
    <p class="collapse" id="seedSpecial">
      Use promo code "GGarden" for additional 15% off your entire purchase!
    </p>
```

## Navbar
```html
  <nav class="navbar-light bg-light navbar navbar-expand-sm">
    <!-- Add the <a> below: -->
    <a class="navbar-brand">
      <img src="https://content.codecademy.com/courses/learn-bootstrap-components/logo.png" alt="Gloria's Gardening Logo" height="30">
    </a>
  
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <!-- Make the follow elements into a nav component: -->
      <ul class="navbar-nav">
        <li class="nav-item active">
          <a class ="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
        </li>
        <li class="nav-item">
          <a class ="nav-link" href="#">Weekly Specials</a>
        </li>
        <li class="nav-item">
          <a class ="nav-link" href="#">About</a>
        </li>
      </ul>
    </div>
  </nav>
```

## Bootstrap card
```html
        <div class="card">
          <img class="card-img-top" src="https://content.codecademy.com/courses/learn-bootstrap-components/flowers.png"/>
          <div class="card-header">
Planting in the spring          
          </div>
          <div class="card-body">
            <p class="card-text">
              It's almost spring time, get your seeds ready for planting!
            </p>
          </div>
        </div>
```

## Bootstrap carousel
refer to the garderning website section


