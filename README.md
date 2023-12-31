 
# Calculator

This is a simple calculator built using HTML, CSS, and JavaScript.

## Getting Started

To get started, clone the repository and open the `index.html` file in a web browser.

## HTML

The HTML file contains the basic structure of the calculator. It includes a `<div>` element with the class `container` that contains all of the other elements. The container is divided into two rows, the first row contains the input field and the second row contains the buttons.

```html
<div class="container">
  <div class="row">
    <input type="text">
  </div>
  <div class="row">
    <button>C</button>
    <button>%</button>
    <button>*</button>
  </div>
</div>
```

## CSS

The CSS file contains the styles for the calculator. It includes styles for the container, the input field, and the buttons.

```css
.container {
  width: 300px;
  margin: 0 auto;
}

input {
  width: 100%;
  height: 50px;
  font-size: 20px;
}

button {
  width: 50px;
  height: 50px;
  margin: 0 5px;
}
```

## JavaScript

The JavaScript file contains the logic for the calculator. It includes functions for handling the button clicks and evaluating the input.

```javascript
const buttons = document.querySelectorAll('button');

buttons.forEach((button) => {
  button.addEventListener('click', (e) => {
    const input = document.querySelector('input');
    const value = e.target.innerHTML;

    if (value === '=') {
      input.value = eval(input.value);
    } else if (value === 'C') {
      input.value = '';
    } else {
      input.value += value;
    }
  });
});
```

## Conclusion

This is a simple calculator built using HTML, CSS, and JavaScript. It is a good example of how to use these technologies to create a simple user interface.

