# Introduction to Sass and NPM

### SASS

Sass is a CSS preprocessor, an extension of CSS that adds power and elegance to the basic language.

#### Features of SASS

1. **Variables**: for resuable values for color, font-sizes, spacing etc
2. **Nesting**: nest selectors inside of one another, allowing us to write less code
3. **Operators**: mathematical operations right inside CSS.
4. **Partials and imports**: write CSS in different files and importing them all into one single file.
5. **Mixins**: resuable pieces of CSS code.
6. **Functions**: similar to mixins, with the difference that they produce a value that can be used.
7. **Extends**: to make different selectors inherit declarations that are common to all of them.
8. **Control directives**: for writing complex code using conditions and loops

# Sass - Variables, nesting, mixins, extends and functions

```css
/* without argument */
@mixin clearfix {
  &::after {
    content: "";
    clear: both;
    display: table;
  }
}

/* with argument */
@mixin style-link-text($color) {
  text-decoration: none;
  text-transform: uppercase;
  color: $color;
}

@function divide($a, $b) {
  @return $a/ $b;
}

element {
  @include clearfix;
  @include style-link-text($color-text-light);
  /* not practical */
  margin: divide(60, 2) * 1px;
}
```

# Responsive designing and layout types

# Mobile-First vs Desktop-First and Breakpoints

# Writing Media Queries

# Responsive images in HTML, CSS with browser supports
