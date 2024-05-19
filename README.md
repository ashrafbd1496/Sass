# Sass Nesting

    .container {
    display: flex;

    .content {
    text-align: center;

    h1 {
      font-size: 2em;
      color: $primary-color;
    }

    p {
      font-size: 1em;
      color: $secondary-color;
    }

    a {
      text-decoration: none;
      color: $link-color;

      &:hover {
        color: $link-hover-color;
      }
      &:nth-child(1){ ... }
    }

}
}

# Menu Nesting

    nav {
    ul {
      margin: 0;
      padding: 0;
      list-style: none;
    }

    li { display: inline-block; }

    a {
      display: block;
      padding: 6px 12px;
      text-decoration: none;
    }
    }


# Partials
    // _base.sass
    $font-stack: Helvetica, sans-serif
    $primary-color: #333

    body
      font: 100% $font-stack
      color: $primary-color

      // styles.sass
      @use 'base'

      .inverse
        background-color: base.$primary-color
        color: white

    SCSS
    Sass
    CSS

# Mixin
    @mixin theme($theme: DarkGray)
      background: $theme
      box-shadow: 0 0 1px rgba($theme, .25)
      color: #fff

    .info
      @include theme

    .alert
      @include theme($theme: DarkRed)

    .success
      @include theme($theme: DarkGreen)


