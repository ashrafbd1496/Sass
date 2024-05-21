<h1 align="center">
  Sass Practice , folders and files organization
</h1>

_Just an example/recommendation of how to organize sass files_

[Here you can check out the demo](https://ashrafbd1496.github.io/)

## Table of Contents

1. [Base Estructure](#Base-Estructure)
2. [📄Index File](#Index-File)
3. [📂Components](src/SCSS/components)
4. [📄Footer](src/SCSS/components/footer.scss)
   1. [📄Using SVG Images from Mixins](src/SCSS/components/callingSVGimages.md)
5. [📄Header](src/SCSS/components/header.scss)
6. [📂Shared](src/SCSS/shared)
7. [📄mixins](src/SCSS/shared/_mixins.scss)
8. [📄variables](src/SCSS/shared/_variables.scss)
9. [📄global](src/SCSS/shared/global.scss)
10. [📄normalize](src/SCSS/shared/normalize.scss)

## Base Estructure

    .
    ├── SASS
      ├── styles
        ├── components
          ├── demo.scss
          ├── footer.scss
        ├── shared
          ├── _mixins.scss
          ├── _variables.scss
          ├── global.scss
          ├── index.scss
          ├── normalize.scss

## Index File

_This file contains general imports of main files_

```css
@import "global/normalize.scss";
@import "global/shared.scss";
@import "components/about.scss";
@import "components/cards.scss";
.
.
.
```

[Check the .index.scss file](src/SCSS/index.scss)
