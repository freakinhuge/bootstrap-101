
# Breadcrumb

##### Indicate the current page’s location within a navigational hierarchy that automatically adds separators via CSS.

+++

### Examples

<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item active" aria-current="page">Home</li>
  </ol>
</nav>

<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="#">Home</a></li>
    <li class="breadcrumb-item active" aria-current="page">Library</li>
  </ol>
</nav>

<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="#">Home</a></li>
    <li class="breadcrumb-item"><a href="#">Library</a></li>
    <li class="breadcrumb-item active" aria-current="page">Data</li>
  </ol>
</nav>

```html
<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item active" aria-current="page">Home</li>
  </ol>
</nav>

<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="#">Home</a></li>
    <li class="breadcrumb-item active" aria-current="page">Library</li>
  </ol>
</nav>

<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="#">Home</a></li>
    <li class="breadcrumb-item"><a href="#">Library</a></li>
    <li class="breadcrumb-item active" aria-current="page">Data</li>
  </ol>
</nav>
```

+++

### Changing the separator

<p>
  Separators are automatically added in CSS through `::before` and `content`.
  They can be changed by changing `$breadcrumb-divider`. The `quote` function
  is needed to generate the quotes around a string, so if you want `>` as
  separator, you can use this:
</p>

```scss
$breadcrumb-divider: quote(">");
```

<p>
  It’s also possible to use a <strong>base64 embedded SVG icon</strong>:
</p>

```scss
$breadcrumb-divider: url(data:image/svg+xml;base64,PHN...dmc+);
```

<p>
  The separator can be removed by setting `$breadcrumb-divider` to `none`:
</p>

```scss
$breadcrumb-divider: none;
```
