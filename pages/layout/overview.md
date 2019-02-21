
# Layout

#### Components and options for laying out your Bootstrap project, including wrapping containers, a powerful grid system, a flexible media object, and responsive utility classes.

+++

### Containers

<p>
  Containers are the most basic layout element in Bootstrap and are
  <strong>required when using our default grid system</strong>. Choose from a
  responsive, fixed-width container (meaning its `max-width` changes at each
  breakpoint) or fluid-width (meaning it’s `100%` wide all the time).
</p>

+++

<p>
  While containers <em>can</em> be nested, most layouts do not require a
  nested container.
</p>

<div class="row justify-content-center mb-3 mx-0" style="height: 300px;">
  <div class="col-2 h-25"></div>
  <div class="col-8 h-25 pb-3 px-0">
    <div class="bg-success rounded h-100"></div>
  </div>
  <div class="col-2 h-25"></div>
  <div class="col-2 h-75"></div>
  <div class="col-2 h-75 pl-0 pr-3">
    <div class="bg-primary rounded h-100"></div>
  </div>
  <div class="col-6 h-75 px-0">
    <div class="bg-secondary rounded h-100"></div>
  </div>
  <div class="col-2 h-75"></div>
</div>

```html
<div class="container">
  <!-- Content here -->
</div>
```

+++

<p>
  Use `.container-fluid` for a full width container, spanning the entire width
  of the viewport.
</p>

<div class="row justify-content-center mb-3 mx-0" style="height: 300px;">
  <div class="col-12 h-25 pb-3 px-0">
    <div class="bg-success rounded h-100"></div>
  </div>
  <div class="col-2 h-75 pl-0 pr-3">
    <div class="bg-primary rounded h-100"></div>
  </div>
  <div class="col-10 h-75 px-0">
    <div class="bg-secondary rounded h-100"></div>
  </div>
</div>

```html
<div class="container-fluid">
  ...
</div>
```

+++

### Responsive breakpoints

<p>
  Since Bootstrap is developed to be mobile first, a handful of media queries
  are used to create sensible breakpoints for the layouts and interfaces.
  These breakpoints are mostly based on minimum viewport widths and allow us
  to scale up elements as the viewport changes.
</p>

<p>
  Bootstrap primarily uses the following media query ranges--or breakpoints--
  in the source Sass files for the layout, grid system, and components.
</p>

```scss
// Extra small devices (portrait phones, less than 576px)
// No media query for `xs` since this is the default in Bootstrap

// Small devices (landscape phones, 576px and up)
@media (min-width: 576px) { ... }

// Medium devices (tablets, 768px and up)
@media (min-width: 768px) { ... }

// Large devices (desktops, 992px and up)
@media (min-width: 992px) { ... }

// Extra large devices (large desktops, 1200px and up)
@media (min-width: 1200px) { ... }
```

+++

<p>
  Since the source CSS is writen in Sass, all the media queries are available
  via Sass mixins:
</p>

```scss
// No media query necessary for xs breakpoint as it's effectively `@media (min-width: 0) { ... }`
@include media-breakpoint-up(sm) { ... }
@include media-breakpoint-up(md) { ... }
@include media-breakpoint-up(lg) { ... }
@include media-breakpoint-up(xl) { ... }

// Example: Hide starting at `min-width: 0`, and then show at the `sm` breakpoint
.custom-class {
  display: none;
}
@include media-breakpoint-up(sm) {
  .custom-class {
    display: block;
  }
}
```

+++

<p>
  Occasionally you could use media queries that go in the other direction
  (the given screen size or smaller):
</p>

```scss
// Extra small devices (portrait phones, less than 576px)
@media (max-width: 575.98px) { ... }

// Small devices (landscape phones, less than 768px)
@media (max-width: 767.98px) { ... }

// Medium devices (tablets, less than 992px)
@media (max-width: 991.98px) { ... }

// Large devices (desktops, less than 1200px)
@media (max-width: 1199.98px) { ... }

// Extra large devices (large desktops)
// No media query since the extra-large breakpoint has no upper bound on its width
```

+++

<p>
  Once again, these media queries are also available via Sass mixins:
</p>

```scss
@include media-breakpoint-down(xs) { ... }
@include media-breakpoint-down(sm) { ... }
@include media-breakpoint-down(md) { ... }
@include media-breakpoint-down(lg) { ... }
// No media query necessary for xl breakpoint as it has no upper bound on its width

// Example: Style from medium breakpoint and down
@include media-breakpoint-down(md) {
  .custom-class {
    display: block;
  }
}
```

+++

<p>
  There are also media queries and mixins for targeting a single segment of
  screen sizes using the minimum and maximum breakpoint widths.
</p>

```scss
// Extra small devices (portrait phones, less than 576px)
@media (max-width: 575.98px) { ... }

// Small devices (landscape phones, 576px and up)
@media (min-width: 576px) and (max-width: 767.98px) { ... }

// Medium devices (tablets, 768px and up)
@media (min-width: 768px) and (max-width: 991.98px) { ... }

// Large devices (desktops, 992px and up)
@media (min-width: 992px) and (max-width: 1199.98px) { ... }

// Extra large devices (large desktops, 1200px and up)
@media (min-width: 1200px) { ... }
```

+++

<p>
  These media queries are also available via Sass mixins:
</p>

```scss
@include media-breakpoint-only(xs) { ... }
@include media-breakpoint-only(sm) { ... }
@include media-breakpoint-only(md) { ... }
@include media-breakpoint-only(lg) { ... }
@include media-breakpoint-only(xl) { ... }
```

<p>
  Similarly, media queries may span multiple breakpoint widths:
</p>

```scss
// Example
// Apply styles starting from medium devices and up to extra large devices
@media (min-width: 768px) and (max-width: 1199.98px) { ... }
```

<p>
  The Sass mixin for targeting the same screen size range would be:
</p>

```scss
@include media-breakpoint-between(md, xl) { ... }
```

+++

### Z-index

<p>
  Several Bootstrap components utilize `z-index`, the CSS property that helps
  control layout by providing a third axis to arrange content. A default
  z-index scale is utilized in Bootstrap that’s been designed to properly
  layer navigation, tooltips and popovers, modals, and more.
</p>

<p>
  It's not encouraged to customize these individual values; should you change
  one, you likely need to change them all.
</p>

```scss
$zindex-dropdown:          1000 !default;
$zindex-sticky:            1020 !default;
$zindex-fixed:             1030 !default;
$zindex-modal-backdrop:    1040 !default;
$zindex-modal:             1050 !default;
$zindex-popover:           1060 !default;
$zindex-tooltip:           1070 !default;
```

<p>
  To handle overlapping borders within components (e.g., buttons and inputs
  in input groups), a low single digit z-index values of `1`, `2`, and `3` are
  used for default, hover, and active states. On hover/focus/active, a
  particular element is brought to the forefront with a higher z-index value to
  show their border over the sibling elements.
</p>
