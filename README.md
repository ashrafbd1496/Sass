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
    }

}
}
