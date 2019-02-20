
# Cards

#### Bootstrap’s cards provide a flexible and extensible content container with multiple variants and options.

<br>

### About

<p>
  A <strong>card</strong> is a flexible and extensible content container. It
  includes options for headers and footers, a wide variety of content,
  contextual background colors, and powerful display options. If you’re
  familiar with Bootstrap 3, cards replace our old panels, wells, and
  thumbnails. Similar functionality to those components is available as
  modifier classes for cards.
</p>

+++

### Examples

<p>
  Cards are built with as little markup and styles as possible, but still
  manage to deliver a ton of control and customization. Built with flexbox,
  they offer easy alignment and mix well with other Bootstrap components. They
  have no `margin` by default, so use spacing utilities as needed.
</p>

+++

<p>
  Below is an example of a basic card with mixed content and a fixed width.
  Cards have no fixed width to start, so they’ll naturally fill the full width
  of its parent element. This is easily customized with our various sizing
  options.
</p>

<div class="card w-25 mb-3">
  <img src="https://via.placeholder.com/286x180?text=Image%20cap"
    class="card-img-top">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">
      Some quick example text to build on the card title and make up the bulk
      of the card's content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

```html
<div class="card w-25">
  <img src="https://via.placeholder.com/286x180?text=Image%20cap" class="card-img-top">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">
      Some quick example text to build on the card title and make up the bulk
      of the card's content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```

+++

### Content types

<p>
  Cards support a wide variety of content, including images, text, list groups,
  links, and more. Below are examples of what’s supported.
</p>

<br>

#### Body

<p>
  The building block of a card is the `.card-body`. Use it whenever you need a
  padded section within a card.
</p>

<div class="card mb-3">
  <div class="card-body">
    This is some text within a card body.
  </div>
</div>

```html
<div class="card">
  <div class="card-body">
    This is some text within a card body.
  </div>
</div>
```

+++

#### Titles, text, and links

<p>
  Card titles are used by adding `.card-title` to a `<h*>` tag. In the same
  way, links are added and placed next to each other by adding `.card-link` to
  an `<a>` tag.
</p>

<p>
  Subtitles are used by adding a `.card-subtitle` to a `<h*>` tag. If the
  `.card-title` and the `.card-subtitle` items are placed in a `.card-body`
  item, the card title and subtitle are aligned nicely.
</p>

<div class="card w-25 mb-3">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <h6 class="card-subtitle mb-2 text-muted">Card subtitle</h6>
    <p class="card-text">
      Some quick example text to build on the card title and make up the bulk
      of the card's content.
    </p>
    <a href="#" class="card-link">Card link</a>
    <a href="#" class="card-link">Another link</a>
  </div>
</div>

```html
<div class="card w-25">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <h6 class="card-subtitle mb-2 text-muted">Card subtitle</h6>
    <p class="card-text">
      Some quick example text to build on the card title and make up the bulk
      of the card's content.
    </p>
    <a href="#" class="card-link">Card link</a>
    <a href="#" class="card-link">Another link</a>
  </div>
</div>
```

+++

#### Images

<p>
  `.card-img-top` places an image to the top of the card. With `.card-text`,
  text can be added to the card. Text within `.card-text` can also be styled
  with the standard HTML tags.
</p>

<div class="card mb-3 w-25">
  <img src="https://via.placeholder.com/286x180?text=Image%20cap"
    class="card-img-top">
  <div class="card-body">
    <p class="card-text">
      Some quick example text to build on the card title and make up the bulk
      of the card's content.
    </p>
  </div>
</div>

```html
<div class="card w-25">
  <img src="https://via.placeholder.com/286x180?text=Image%20cap" class="card-img-top">
  <div class="card-body">
    <p class="card-text">
      Some quick example text to build on the card title and make up the bulk
      of the card's content.
    </p>
  </div>
</div>
```

+++

#### List groups

<p>
  Create lists of content in a card with a flush list group.
</p>

<div class="card w-25 mb-3">
  <ul class="list-group list-group-flush">
    <li class="list-group-item">Cras justo odio</li>
    <li class="list-group-item">Dapibus ac facilisis in</li>
    <li class="list-group-item">Vestibulum at eros</li>
  </ul>
</div>

```html
<div class="card w-25">
  <ul class="list-group list-group-flush">
    <li class="list-group-item">Cras justo odio</li>
    <li class="list-group-item">Dapibus ac facilisis in</li>
    <li class="list-group-item">Vestibulum at eros</li>
  </ul>
</div>
```

+++

<div class="card w-25 mb-3">
  <div class="card-header">
    Featured
  </div>
  <ul class="list-group list-group-flush">
    <li class="list-group-item">Cras justo odio</li>
    <li class="list-group-item">Dapibus ac facilisis in</li>
    <li class="list-group-item">Vestibulum at eros</li>
  </ul>
</div>

```html
<div class="card w-25">
  <div class="card-header">
    Featured
  </div>
  <ul class="list-group list-group-flush">
    <li class="list-group-item">Cras justo odio</li>
    <li class="list-group-item">Dapibus ac facilisis in</li>
    <li class="list-group-item">Vestibulum at eros</li>
  </ul>
</div>
```

+++

#### Header and footer

<p>
  Add an optional header and/or footer within a card.
</p>

<div class="card mb-3">
  <div class="card-header">
    Featured
  </div>
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

```html
<div class="card">
  <div class="card-header">
    Featured
  </div>
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```

+++

<p>
  Card headers can be styled by adding `.card-header` to `<h*>` elements.
</p>

<div class="card mb-3">
  <h5 class="card-header">Featured</h5>
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

```html
<div class="card">
  <h5 class="card-header">Featured</h5>
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```

+++

<div class="card mb-3">
  <div class="card-header">
    Quote
  </div>
  <div class="card-body">
    <blockquote class="blockquote mb-0">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer
        posuere erat a ante.
      </p>
      <footer class="blockquote-footer">
        Someone famous in <cite title="Source Title">Source Title</cite>
      </footer>
    </blockquote>
  </div>
</div>

```html
<div class="card">
  <div class="card-header">
    Quote
  </div>
  <div class="card-body">
    <blockquote class="blockquote mb-0">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer
        posuere erat a ante.
      </p>
      <footer class="blockquote-footer">
        Someone famous in <cite title="Source Title">Source Title</cite>
      </footer>
    </blockquote>
  </div>
</div>
```

+++

<div class="card text-center mb-3">
  <div class="card-header">
    Featured
  </div>
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
  <div class="card-footer text-muted">
    2 days ago
  </div>
</div>

```html
<div class="card text-center">
  <div class="card-header">
    Featured
  </div>
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
  <div class="card-footer text-muted">
    2 days ago
  </div>
</div>
```

+++

### Sizing

<p>
  Cards assume no specific `width` to start, so they’ll be 100% wide unless
  otherwise stated. You can change this as needed with custom CSS, grid
  classes, grid Sass mixins, or utilities.
</p>

+++

#### Using grid markup

<p>
  Using the grid, wrap cards in columns and rows as needed.
</p>

<div class="row mb-3">
  <div class="col-sm-6">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">Special title treatment</h5>
        <p class="card-text">
          With supporting text below as a natural lead-in to additional
          content.
        </p>
        <a href="#" class="btn btn-primary">Go somewhere</a>
      </div>
    </div>
  </div>
  <div class="col-sm-6">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">Special title treatment</h5>
        <p class="card-text">
          With supporting text below as a natural lead-in to additional
          content.
        </p>
        <a href="#" class="btn btn-primary">Go somewhere</a>
      </div>
    </div>
  </div>
</div>

+++

```html
<div class="row">
  <div class="col-sm-6">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">Special title treatment</h5>
        <p class="card-text">
          With supporting text below as a natural lead-in to additional
          content.
        </p>
        <a href="#" class="btn btn-primary">Go somewhere</a>
      </div>
    </div>
  </div>
  <div class="col-sm-6">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">Special title treatment</h5>
        <p class="card-text">
          With supporting text below as a natural lead-in to additional
          content.
        </p>
        <a href="#" class="btn btn-primary">Go somewhere</a>
      </div>
    </div>
  </div>
</div>
```

+++

#### Using utilites

<p>
  Use one of the handful of available sizing utilities to quickly set a card’s
  width.
</p>

<div class="card w-75 mb-3">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional
      content.
    </p>
    <a href="#" class="btn btn-primary">Button</a>
  </div>
</div>

<div class="card w-50 mb-3">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional
      content.
    </p>
    <a href="#" class="btn btn-primary">Button</a>
  </div>
</div>

+++

```html
<div class="card w-75 mb-3">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional
      content.
    </p>
    <a href="#" class="btn btn-primary">Button</a>
  </div>
</div>

<div class="card w-50">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional
      content.
    </p>
    <a href="#" class="btn btn-primary">Button</a>
  </div>
</div>
```

+++

#### Using custom CSS

<p>
  Use custom CSS in your stylesheets or as inline styles to set a width.
</p>

<div class="card mb-3" style="width: 18rem;">
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional
      content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

```html
<div class="card" style="width: 18rem;">
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional
      content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```

+++

### Text alignment

<p>
  You can quickly change the text alignment of any card--in its entirety or
  specific parts—with the text align classes.
</p>

<div class="card mb-3 w-25">
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

<div class="card text-center mb-3 w-25">
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

<div class="card text-right w-25">
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

+++

```html
<div class="card mb-3 w-25">
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

<div class="card text-center mb-3 w-25">
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

<div class="card text-right w-25">
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```

+++

### Navigation

<p>
  Add some navigation to a card’s header (or block) with Bootstrap’s nav
  components.
</p>

<div class="card text-center">
  <div class="card-header">
    <ul class="nav nav-tabs card-header-tabs">
      <li class="nav-item">
        <a class="nav-link active" href="#">Active</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Link</a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link disabled"
          href="#"
          tabindex="-1"
          aria-disabled="true">
          Disabled
        </a>
      </li>
    </ul>
  </div>
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

+++

```html
<div class="card text-center">
  <div class="card-header">
    <ul class="nav nav-tabs card-header-tabs">
      <li class="nav-item">
        <a class="nav-link active" href="#">Active</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Link</a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link disabled"
          href="#"
          tabindex="-1"
          aria-disabled="true">
          Disabled
        </a>
      </li>
    </ul>
  </div>
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```

+++

<div class="card text-center">
  <div class="card-header">
    <ul class="nav nav-pills card-header-pills">
      <li class="nav-item">
        <a class="nav-link active" href="#">Active</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Link</a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link disabled"
          href="#"
          tabindex="-1"
          aria-disabled="true">
          Disabled
        </a>
      </li>
    </ul>
  </div>
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

+++

```html
<div class="card text-center">
  <div class="card-header">
    <ul class="nav nav-pills card-header-pills">
      <li class="nav-item">
        <a class="nav-link active" href="#">Active</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Link</a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link disabled"
          href="#"
          tabindex="-1"
          aria-disabled="true">
          Disabled
        </a>
      </li>
    </ul>
  </div>
  <div class="card-body">
    <h5 class="card-title">Special title treatment</h5>
    <p class="card-text">
      With supporting text below as a natural lead-in to additional content.
    </p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```
