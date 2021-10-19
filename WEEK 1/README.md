# Basics of HTML with it's DOM structure

#### Simple reset using universal selector CSS

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* All will be inherited by the child elements */

body {
  font-family: "Lato", sans-serif;
  font-weight: 400;
  font-size: 16px;
  line-height: 1.7;
  color: #777;
}
```

#### CSS | Clip-path property

- Clip path maker: https://bennettfeely.com/clippy/

- Lets you crop the element using various methods like

```css
/* Direction: Top-Left, Top-Right, Bottom-Right, Bottom-Left */
/* clip-path: polygon (x y, x y, x y, x y) */
/* Triangle */
clip-path: polygon(50% 0, 100% 100%, 0 100%);
```

# Basics of CSS with overview of animations

- CSS animation is done using keyframes at-rule (`@keyframes`) and `animation` property.

## There a 2 types of animation in CSS

### Simple: Using `transition` property

The `transition` property has to be on the initial state

```css
.btn {
  transition: all 0.2s;
}

.btn:hover {
  transform: translateY(-3px);
  /* Offset in X, Offset in Y, Blur, color */
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
}

.btn:active {
  transform: translateY(-1px);
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
}
```

### Complex: Using `@keyframes`.

```css
.heading-primary-main {
  animation-name: moveInLeft;
  animation-duration: 1s;
  animation-delay: 3s;
  animation-iteration-count: 3;
  animation-timing-function: ease-out;
}

/* Animation shorthand */
.heading-primary-sub {
  animation: moveInRight 1s ease-out;
}

@keyframes moveInLeft {
  0% {
    opacity: 0;
    transform: translateX(-100px);
  }

  80% {
    transform: translateX(10px);
  }

  100% {
    opacity: 1;
    transform: translate(0);
  }
}
```

# How CSS is parsed - Cascading and specificity

# How CSS Renders a Website: The Visual Formatting Model

# CSS architecture, components and BEM

### Github Repo: https://github.com/jonasschmedtmann/advanced-css-course
