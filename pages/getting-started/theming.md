
## Theming Bootstrap

#### Customize Bootstrap 4 with the new built-in Sass variables for global style preferences for easy theming and component changes.

<br>

### Introduction

<p>
  In Bootstrap 3, theming was largely driven by variable overrides in LESS,
  custom CSS, and a separate theme stylesheet that was included in the `dist`
  files. With some effort, one could completely redesign the look of Bootstrap
  3 without touching the core files. Bootstrap 4 provides a familiar, but
  slightly different approach.
</p>

<p>
  Now, theming is accomplished by Sass variables, Sass maps, and custom CSS.
  There’s no more dedicated theme stylesheet; instead, you can enable the
  built-in theme to add gradients, shadows, and more.
</p>

+++

### Importing

<p>
  In your `custom.scss`, you’ll import Bootstrap’s source Sass files. You have
  two options: include all of Bootstrap, or pick the parts you need. The latter
  is encourage, though be aware there are some requirements and dependencies
  across our components. You also will need to include some JavaScript for the
  plugins.
</p>

```scss
// Custom.scss
// Include all of Bootstrap

@import "bootstrap";
```

<p>
  With that setup in place, you can begin to modify any of the Sass variables
  and maps in your `custom.scss`.
</p>

+++

### Variable defaults

<p>
  Every Sass variable in Bootstrap 4 includes the `!default` flag allowing you
  to override the variable’s default value in your own Sass without modifying
  Bootstrap’s source code. Copy and paste variables as needed, modify their
  values, and remove the `!default` flag. If a variable has already been
  assigned, then it won’t be re-assigned by the default values in Bootstrap.
</p>

<p>
  You will find the complete list of Bootstrap’s variables in
  `scss/_variables.scss`.
</p>

<p>
  Variable overrides within the same Sass file can come before or after the
  default variables. However, when overriding across Sass files, your
  overrides must come before you import Bootstrap’s Sass files.
</p>

<p>
  Here’s an example that changes the `background-color` and `color` for the
  `<body>` when importing and compiling Bootstrap via RubyGems:
</p>

```scss
// Your variable overrides
$body-bg: #000;
$body-color: #111;

// Bootstrap and its default variables
@import "bootstrap";
```
