
## Introduction

##### Get started with Bootstrap, the world’s most popular framework for building responsive, mobile-first sites, with BootstrapCDN and a template starter page.

<br>

### CSS

<p>
  Copy-paste the stylesheet `<link>` into your `<head>` before all other
  stylesheets to load the CSS.
</p>

```html
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.2.1/css/bootstrap.min.css">
```

+++

### JS

<p>
  Many of the components require the use of JavaScript to function.
  Specifically, they require jQuery, Popper.js, and the Bootstrap specific
  JavaScript plugins. Place the following `<script>`s near the end of your
  pages, right before the closing `</body>` tag, to enable them. jQuery must
  come first, then Popper.js, and then the Bootstrap JavaScript plugins.
</p>

```html
<script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.6/umd/popper.min.js"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.2.1/js/bootstrap.min.js"></script>
```

<p>
  Here is a list of components that explicitly require jQuery, Bootstrap JS,
  and Popper.js.
  <ul>
    <li>
      Alerts for dismissing
    </li>
    <li>
      Buttons for toggling states and checkbox/radio functionality
    </li>
    <li>
      Carousel for all slide behaviors, controls, and indicators
    </li>
    <li>
      Collapse for toggling visibility of content
    </li>
    <li>
      Dropdowns for displaying and positioning (also requires Popper.js)
    </li>
    <li>
      Modals for displaying, positioning, and scroll behavior
    </li>
    <li>
      Navbar for extending our Collapse plugin to implement responsive behavior
    </li>
    <li>
      Tooltips and popovers for displaying and positioning (also requires
      Popper.js)
    </li>
    <li>
      Scrollspy for scroll behavior and navigation updates
    </li>
  </ul>
</p>

+++

### Starter template

<p>
  Be sure to have your pages set up with the latest design and development
  standards. That means using an HTML5 doctype and including a viewport meta
  tag for proper responsive behaviors. Put it all together and your pages
  should look like this:
</p>

```html
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.2.1/css/bootstrap.min.css">

    <title>Hello, world!</title>
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.6/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.2.1/js/bootstrap.min.js"></script>
  </body>
</html>
```

+++

### Important globals

<p>
  Bootstrap employs a handful of important global styles and settings that
  you’ll need to be aware of when using it, all of which are almost
  exclusively geared towards the normalization of cross browser styles. Let’s
  break those down.
</p>

#### HTML5 doctype

<p>
  Bootstrap requires the use of the HTML5 doctype. Without it, you’ll see some
  funky incomplete styling, but including it shouldn’t cause any considerable
  hiccups.
</p>

```html
<!doctype html>
<html lang="en">
  ...
</html>
```

+++

#### Responsive meta tag

<p>
  Bootstrap is developed <em>mobile first</em>, a strategy in which code is
  optimized for mobile devices first and then scale up components as necessary
  using CSS media queries. To ensure proper rendering and touch zooming for
  all devices, <strong>add the responsive viewport meta tag</strong> to your
  `<head>`.
</p>

```html
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
```

+++

#### Box-sizing

<p>
  For more straightforward sizing in CSS, the global `box-sizing` value is
  switched from `content-box` to `border-box`. This ensures `padding` does not
  affect the final computed width of an element, but it can cause problems
  with some third party software like Google Maps and Google Custom Search
  Engine.
</p>

<p>
  On the rare occasion you need to override it, use something like the
  following:
</p>

```html
.selector-for-some-widget {
  box-sizing: content-box;
}
```

<p>
  With the above snippet, nested elements--including generated content via
  `::before` and `::after`--will all inherit the specified `box-sizing` for
  that `.selector-for-some-widget`.
</p>

+++

#### Reboot

<p>
  For improved cross-browser rendering, Reboot is used to correct
  inconsistencies across browsers and devices while providing slightly more
  opinionated resets to common HTML elements.
</p>
