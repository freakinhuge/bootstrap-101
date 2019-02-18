
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

<div class="card mb-3" style="width: 18rem;">
  <img src="https://via.placeholder.com/286x180?text=Image%20cap"
    class="card-img-top" alt="...">
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
<div class="card" style="width: 18rem;">
  <img src="https://via.placeholder.com/286x180?text=Image%20cap"
    class="card-img-top" alt="...">
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
