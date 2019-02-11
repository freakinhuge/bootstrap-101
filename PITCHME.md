@title[Bootstrap 101]

## Bootstrap 101!

<div class="btn btn-primary">I am a button</div>

---

### Alerts

<p>
  Alerts are available for any length of text, as well as an optional dismiss
  button. For proper styling, use one of the eight required contextual classes
  (e.g., `.alert-success`).
</p>

<div class="alert alert-primary mx-4 text-left p-4 mb-3" role="alert">
  A simple primary alert—check it out!
</div>
<div class="alert alert-secondary mx-4 text-left p-4 mb-3" role="alert">
  A simple secondary alert—check it out!
</div>
<div class="alert alert-success mx-4 text-left p-4 mb-3" role="alert">
  A simple success alert—check it out!
</div>
<div class="alert alert-danger mx-4 text-left p-4 mb-3" role="alert">
  A simple danger alert—check it out!
</div>
<div class="alert alert-warning mx-4 text-left p-4 mb-3" role="alert">
  A simple warning alert—check it out!
</div>
<div class="alert alert-info mx-4 text-left p-4 mb-3" role="alert">
  A simple info alert—check it out!
</div>
<div class="alert alert-light mx-4 text-left p-4 mb-3" role="alert">
  A simple light alert—check it out!
</div>
<div class="alert alert-dark mx-4 text-left p-4 mb-3" role="alert">
  A simple dark alert—check it out!
</div>

+++

<div class="alert alert-primary mx-4 text-left p-4" role="alert">
  A simple primary alert—check it out!
</div>

```html
<div class="alert alert-primary" role="alert">
  A simple primary alert—check it out!
</div>
```

+++

### Link color

<p>
  Use the `.alert-link` utility class to quickly provide matching colored links
  within any alert.
</p>

<div class="alert alert-primary mx-4 text-left p-4" role="alert">
  A simple primary alert with <a href="#" class="alert-link">an example link</a>. Give it a click if you like.
</div>
<div class="alert alert-secondary mx-4 text-left p-4" role="alert">
  A simple secondary alert with <a href="#" class="alert-link">an example link</a>. Give it a click if you like.
</div>
<div class="alert alert-success mx-4 text-left p-4" role="alert">
  A simple success alert with <a href="#" class="alert-link">an example link</a>. Give it a click if you like.
</div>
<div class="alert alert-danger mx-4 text-left p-4" role="alert">
  A simple danger alert with <a href="#" class="alert-link">an example link</a>. Give it a click if you like.
</div>
<div class="alert alert-warning mx-4 text-left p-4" role="alert">
  A simple warning alert with <a href="#" class="alert-link">an example link</a>. Give it a click if you like.
</div>
<div class="alert alert-info mx-4 text-left p-4" role="alert">
  A simple info alert with <a href="#" class="alert-link">an example link</a>. Give it a click if you like.
</div>
<div class="alert alert-light mx-4 text-left p-4" role="alert">
  A simple light alert with <a href="#" class="alert-link">an example link</a>. Give it a click if you like.
</div>
<div class="alert alert-dark mx-4 text-left p-4" role="alert">
  A simple dark alert with <a href="#" class="alert-link">an example link</a>. Give it a click if you like.
</div>

+++

<div class="alert alert-primary" role="alert">
  A simple primary alert with <a href="#" class="alert-link">
  an example link</a>. Give it a click if you like.
</div>

```html
<div class="alert alert-primary" role="alert">
  A simple primary alert with <a href="#" class="alert-link">
  an example link</a>. Give it a click if you like.
</div>
```

+++

### Additional content

<p>
  Alerts can also contain additional HTML elements like headings, paragraphs
  and dividers.
</p>

<div class="alert alert-success mx-4 text-left p-4" role="alert">
  <h4 class="alert-heading">Well done!</h4>
  <p>
    Aww yeah, you successfully read this important alert message. This example
    text is going to run a bit longer so that you can see how spacing within
    an alert works with this kind of content.
  </p>
  <hr>
  <p class="mb-0">
    Whenever you need to, be sure to use margin utilities to keep things nice
    and tidy.
  </p>
</div>

```html
<div class="alert alert-success" role="alert">
  <h4 class="alert-heading">Well done!</h4>
  <p>
    Aww yeah, you successfully read this important alert message. This example
    text is going to run a bit longer so that you can see how spacing within
    an alert works with this kind of content.
  </p>
  <hr>
  <p class="mb-0">
    Whenever you need to, be sure to use margin utilities to keep things nice
    and tidy.
  </p>
</div>
```
