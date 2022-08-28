# ng-material-utility
Tailwind-like utility classes for Angular Material.
Example: `bg-accent-500`, `text-primary-200-contrast`

# Usage

```
npm i ng-material-utility
```

You can use the mixin `all($theme)` to include all color-based classes supported i.e `background-color`, `color`, `outline-color`, `border-color`, and `text-decoration-color`.

```scss
@use 'ng-material-utility' as ng-material-utility;

// Code defining your Material $theme.

@include ng-material-utility.all($theme-var);
```
You can choose to generate only classes that you need using the following functions:

```scss
@include ng-material-utility.color($theme-var);
@include ng-material-utility.background-color($theme-var);
@include ng-material-utility.border-color($theme-var);
@include ng-material-utility.text-decoration-color($theme-var);
@include ng-material-utility.outline-color($theme-var);
```

# Characteristics
- Adds about 43kB of Raw Size to the styles when all styles are used.
- Moves you one step further to having all your styles in CSS and not inlined by Angular at runtime.
