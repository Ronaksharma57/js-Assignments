
# Day10Homework

This is a simple HTML and JavaScript code that changes the background color of the webpage when the button is clicked.

Hosted Link : https://ronaksharma57.github.io/js-Assignments/Day10Homework/

## Step-by-Step Explanation

### HTML Code

The HTML code consists of a `<div>` element that contains a button. The button has an `onclick` event listener that calls the `changeBackgroundColor()` function when clicked.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Day10Homework</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div>
        <button>Change BackGroundColor</button>
    </div>
    <script src="index.js">
    </script>
</body>
</html>
```

### JavaScript Code

The JavaScript code consists of a single function called `changeBackgroundColor()`. This function changes the background color of the webpage by setting the `backgroundColor` property of the `body` element.

```javascript
var Color = [
    "green",
    "cyan",
    "black",
    "voilet",
    "blue",
    "yellow",
    "purple",
    "orange",
    "lightgreen",
    "lemon",
  ];
  var index = 0 ;
  var div = document.querySelector("div");
  const button = document.querySelector("button");
  button.addEventListener("click", function() {
      if (index === Color.length) {
          index = 0;
    }
          div.style.backgroundColor = Color[index];
          index++;
  })
```

## Conclusion

This is a simple example of how to change the background color of a webpage using HTML and JavaScript. This code can be used as a starting point for more complex projects.
```
