
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

<div class="row justify-content-center mb-3" style="height: 300px;">
  <div class="col-8 bg-success rounded mb-3"></div>
  <div class="col-2 bg-primary rounded mr-3"></div>
  <div class="col-6 bg-secondary rounded"></div>
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

<div class="row justify-content-center mb-3" style="height: 300px;">
  <div class="col-11 bg-success rounded mb-3"></div>
  <div class="col-2 bg-primary rounded mr-3"></div>
  <div class="col-9 bg-secondary rounded"></div>
</div>

```html
<div class="container-fluid">
  ...
</div>
```
