
# Buttons

##### Use Bootstrap’s custom button styles for actions in forms, dialogs, and more with support for multiple sizes, states, and more.

<br>

### Examples

<p>
  Bootstrap includes several predefined button styles, each serving its own
  semantic purpose, with a few extras thrown in for more control.
</p>

<div class="mb-3">
  <button type="button" class="btn btn-primary">Primary</button>
  <button type="button" class="btn btn-secondary">Secondary</button>
  <button type="button" class="btn btn-success">Success</button>
  <button type="button" class="btn btn-danger">Danger</button>
  <button type="button" class="btn btn-warning">Warning</button>
  <button type="button" class="btn btn-info">Info</button>
  <button type="button" class="btn btn-light">Light</button>
  <button type="button" class="btn btn-dark">Dark</button>
  <button type="button" class="btn btn-link">Link</button>
</div>

```html
<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-light">Light</button>
<button type="button" class="btn btn-dark">Dark</button>
<button type="button" class="btn btn-link">Link</button>
```

+++

### Button tags

<p>
  The `.btn` classes are designed to be used with the `<button>` element.
  However, you can also use these classes on `<a>` or `<input>` elements
  (though some browsers may apply a slightly different rendering).
<p/>

<p>
  When using button classes on `<a>` elements that are used to trigger in-page
  functionality (like collapsing content), rather than linking to new pages or
  sections within the current page, these links should be given a
  `role="button"` to appropriately convey their purpose to assistive
  technologies such as screen readers.
</p>

<div class="mb-3">
  <a class="btn btn-primary" href="#" role="button">Link</a>
  <button class="btn btn-primary" type="submit">Button</button>
  <input class="btn btn-primary" type="button" value="Input">
  <input class="btn btn-primary" type="submit" value="Submit">
  <input class="btn btn-primary" type="reset" value="Reset">
</div>

```html
<a class="btn btn-primary" href="#" role="button">Link</a>
<button class="btn btn-primary" type="submit">Button</button>
<input class="btn btn-primary" type="button" value="Input">
<input class="btn btn-primary" type="submit" value="Submit">
<input class="btn btn-primary" type="reset" value="Reset">
```

+++

### Outline buttons

<p>
  In need of a button, but not the hefty background colors they bring? Replace
  the default modifier classes with the `.btn-outline-*` ones to remove all
  background images and colors on any button.
</p>

<div class="mb-3">
  <button type="button" class="btn btn-outline-primary">Primary</button>
  <button type="button" class="btn btn-outline-secondary">Secondary</button>
  <button type="button" class="btn btn-outline-success">Success</button>
  <button type="button" class="btn btn-outline-danger">Danger</button>
  <button type="button" class="btn btn-outline-warning">Warning</button>
  <button type="button" class="btn btn-outline-info">Info</button>
  <button type="button" class="btn btn-outline-light">Light</button>
  <button type="button" class="btn btn-outline-dark">Dark</button>
</div>

```html
<button type="button" class="btn btn-outline-primary">Primary</button>
<button type="button" class="btn btn-outline-secondary">Secondary</button>
<button type="button" class="btn btn-outline-success">Success</button>
<button type="button" class="btn btn-outline-danger">Danger</button>
<button type="button" class="btn btn-outline-warning">Warning</button>
<button type="button" class="btn btn-outline-info">Info</button>
<button type="button" class="btn btn-outline-light">Light</button>
<button type="button" class="btn btn-outline-dark">Dark</button>
```

+++

### Sizes

<p>
  Fancy larger or smaller buttons? Add `.btn-lg` or `.btn-sm` for additional
  sizes.
</p>

<div class="mb-3">
  <button type="button" class="btn btn-primary btn-lg">Large button</button>
  <button type="button" class="btn btn-secondary btn-lg">Large button</button>
</div>

```html
<button type="button" class="btn btn-primary btn-lg">Large button</button>
<button type="button" class="btn btn-secondary btn-lg">Large button</button>
```

<div class="mb-3">
  <button type="button" class="btn btn-primary btn-sm">Small button</button>
  <button type="button" class="btn btn-secondary btn-sm">Small button</button>
</div>

```html
<button type="button" class="btn btn-primary btn-sm">Small button</button>
<button type="button" class="btn btn-secondary btn-sm">Small button</button>
```
<br>
<p>
  Create block level buttons—those that span the full width of a parent—by
  adding `.btn-block`.
</p>

<div class="mb-3">
  <button type="button" class="btn btn-primary btn-lg btn-block">
    Block level button
  </button>
  <button type="button" class="btn btn-secondary btn-lg btn-block">
    Block level button
  </button>
</div>

```html
<button type="button" class="btn btn-primary btn-lg btn-block">Block level button</button>
<button type="button" class="btn btn-secondary btn-lg btn-block">Block level button</button>
```

+++

### Active state

<p>
  Buttons will appear pressed (with a darker background, darker border, and
  inset shadow) when active. <strong>There’s no need to add a class to
  `<button>`s as they use a pseudo-class</strong>. However, you can still force
  the same active appearance with `.active` (and include the
  `aria-pressed="true"` attribute) should you need to replicate the state
  programmatically.
</p>

<a href="#" class="btn btn-primary btn-lg active" role="button" aria-pressed="true">Primary link</a>
<a href="#" class="btn btn-secondary btn-lg active" role="button" aria-pressed="true">Link</a>

```html
<a href="#" class="btn btn-primary btn-lg active" role="button" aria-pressed="true">Primary link</a>
<a href="#" class="btn btn-secondary btn-lg active" role="button" aria-pressed="true">Link</a>
```

+++

### Disabled state

<p>
  Make buttons look inactive by adding the `disabled` boolean attribute to any
  `<button>` element.
</p>

<div class="mb-3">
  <button type="button" class="btn btn-lg btn-primary" disabled>Primary button</button>
  <button type="button" class="btn btn-secondary btn-lg" disabled>Button</button>
</div>

```html
<button type="button" class="btn btn-lg btn-primary" disabled>Primary button</button>
<button type="button" class="btn btn-secondary btn-lg" disabled>Button</button>
```

+++

<p>
  Disabled buttons using the `<a>` element behave a bit different:
  <ul>
    <li>
      `<a>`s don’t support the disabled attribute, so you must add the
      `.disabled` class to make it visually appear disabled.
    </li>
    <li>
      Some future-friendly styles are included to disable all `pointer-events`
      on anchor buttons. In browsers which support that property, you won’t
      see the disabled cursor at all.
    </li>
    <li>
      Disabled buttons should include the `aria-disabled="true"` attribute to
      indicate the state of the element to assistive technologies.
    </li>
  </ul>
</p>

<a href="#" class="btn btn-primary btn-lg disabled" tabindex="-1" role="button" aria-disabled="true">Primary link</a>
<a href="#" class="btn btn-secondary btn-lg disabled" tabindex="-1" role="button" aria-disabled="true">Link</a>

```html
<a href="#" class="btn btn-primary btn-lg disabled" tabindex="-1" role="button" aria-disabled="true">
  Primary link
</a>
<a href="#" class="btn btn-secondary btn-lg disabled" tabindex="-1" role="button" aria-disabled="true">
  Link
</a>
```

+++

### Button plugin

<p>
  Do more with buttons. Control button states or create groups of buttons for
  more components like toolbars.
</p>

#### Toggle states

<p>
  Add `data-toggle="button"` to toggle a button’s `active` state. If you’re
  pre-toggling a button, you must manually add the `.active` class
  <strong>and</strong> `aria-pressed="true"` to the `<button>`.
</p>

<div class="mb-3">
  <button type="button" class="btn btn-primary" data-toggle="button" aria-pressed="false" autocomplete="off">
    Single toggle
  </button>
</div>

```html
<button type="button" class="btn btn-primary" data-toggle="button" aria-pressed="false" autocomplete="off">
  Single toggle
</button>
```

+++

#### Checkbox and radio buttons

<p>
  Bootstrap’s `.button` styles can be applied to other elements, such as
  `<label>`s, to provide checkbox or radio style button toggling. Add
  `data-toggle="buttons"` to a `.btn-group` containing those modified buttons
  to enable their toggling behavior via JavaScript and add `.btn-group-toggle`
  to style the `<input>`s within your buttons. <strong>Note that you can create single
  input-powered buttons or groups of them.</strong>
</p>

<p>
  The checked state for these buttons is <strong>only updated via `click`
  event</strong> on the button. If you use another method to update the
  input--e.g., with `<input type="reset">` or by manually applying the input’s
  `checked` property--you’ll need to toggle `.active` on the `<label>` manually.
</p>

<p>
  Note that pre-checked buttons require you to manually add the `.active` class
  to the input’s `<label>`.
</p>

+++

<div class="mb-3">
  <div class="btn-group-toggle" data-toggle="buttons">
    <label class="btn btn-secondary active">
      <input type="checkbox" checked autocomplete="off"> Checked
    </label>
  </div>
</div>

```html
<div class="btn-group-toggle" data-toggle="buttons">
  <label class="btn btn-secondary active">
    <input type="checkbox" checked autocomplete="off"> Checked
  </label>
</div>
```

<div class="mb-3">
  <div class="btn-group btn-group-toggle" data-toggle="buttons">
    <label class="btn btn-secondary active">
      <input type="radio" name="options" id="option1" autocomplete="off" checked> Active
    </label>
    <label class="btn btn-secondary">
      <input type="radio" name="options" id="option2" autocomplete="off"> Radio
    </label>
    <label class="btn btn-secondary">
      <input type="radio" name="options" id="option3" autocomplete="off"> Radio
    </label>
  </div>
</div>

```html
<div class="btn-group btn-group-toggle" data-toggle="buttons">
  <label class="btn btn-secondary active">
    <input type="radio" name="options" id="option1" autocomplete="off" checked> Active
  </label>
  <label class="btn btn-secondary">
    <input type="radio" name="options" id="option2" autocomplete="off"> Radio
  </label>
  <label class="btn btn-secondary">
    <input type="radio" name="options" id="option3" autocomplete="off"> Radio
  </label>
</div>
```
