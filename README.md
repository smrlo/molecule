# Molecule
![GitHub release](https://img.shields.io/github/release/smrlo/molecule.svg)
![CSS gzip size](https://img.badgesize.io/smrlo/molecule/master/molecule.min.css?compression=gzip&label=CSS%20gzip%20size)

Molecule is a lightweight, responsive and mobile-first CSS framework which provides a very flexible solution for an easy to set up and fast development.

- Lightweight (~2KB gzipped)
- Easy to set up, flexbox based and mobile-first
- Responsive and flexible grid system: 12 columns with 1140px, 960px or Full-page width grid
- Basic typography, text utilities and some other basic layout elements



## Getting Started
To install Molecule, simply add the `molecule.min.css` file in your website &lt;head&gt;. For more cross-browser consistency of default styling, you can also add `normalize.min.css` before adding molecule.

```html
<!-- CSS Reset -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/normalize.css@8.0.1/normalize.min.css">

<!-- Molecule CSS minified -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/smrlo/molecule/molecule.min.css">
```



## The Grid
Molecule includes a 12 columns responsive, flexbox based and mobile first grid system with a default max width of 1140px, wich you can easily change to a 960px or full page width. You can of course also have a mix of different grids widths on the same page.

For the standard 1140px grid use the following code:
```html
<!-- default 12 columns - max width 1140px -->
<div class="container">
  <div class="row">
    ...
  </div>
</div>
```

For the 960px grid use the following code:
```html
<!-- max width 960px -->
<div class="container-960">
  <div class="row">
    ...
  </div>
</div>
```

For the full page width grid use the following code:
```html
<!-- full page width -->
<div class="container-full">
  <div class="row">
    ...
  </div>
</div>
```

To set up the columns use `col-*`, `col-s-*`, `col-m-*`, `col-l-*` and `col-x-*`. Note: `*` must be a number between 1 and 12 (e.g. `col-s-12`), or use `none` to hide the column (e.g. `col-s-none`).
| Class        | Applies      | CSS Media Query            | Example      |
| ------------ | ------------ | -------------------------- | ------------ |
| col-*        | < 576px      | Default                    | col-12       |
| col-s-*      | ≥ 576px      | @media (min-width: 576px)  | col-s-12     |
| col-m-*      | ≥ 768px      | @media (min-width: 768px)  | col-m-12     |
| col-l-*      | ≥ 992px      | @media (min-width: 992px)  | col-l-12     |
| col-x-*      | ≥ 1200px     | @media (min-width: 1200px) | col-x-12     |

Example:
```html
<div class="container">
  <div class="row">
    <div class="col-12 col-s-6 col-m-6 col-l-4 col-x-4">...</div>
    <div class="col-none col-s-3 col-m-3 col-l-4 col-x-4">...</div>
    <div class="col-none col-s-3 col-m-3 col-l-4 col-x-4">...</div>
  </div>
</div>
```


## Typography
Molecule includes some basic typography defaults for headings, text modifiers, paragraphs, blockquotes, lists and code elements. The base font size in Molecule is 1rem (usually 16px) with a line height of 1.5 (24px).

Read more on how to get started and what else you can do with Molecule [here](https://smrlo.github.io/molecule).



## Contributing
Did you find a &#x1f41e; or would like to make a feature request? Please [open a new issue](https://github.com/smrlo/molecule/issues).



## Copyright and license
Released under the [MIT License](https://github.com/smrlo/molecule/blob/master/LICENSE).
