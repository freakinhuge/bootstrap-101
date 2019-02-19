
## Layout

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
