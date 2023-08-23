
This is a simple HTML, CSS, and JavaScript code that allows a user to add paragraphs to a webpage. 

### Step-by-Step Explanation

#### HTML 

The HTML code creates a simple webpage with a text input, a button, and a div to hold the paragraphs.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
<div>
    <input type="text" id="text">
    <button id="addButton">Add</button>
    <div id="paragraph"></div>
</div>
    <script src="index.js"></script>
</body>
</html>
```

#### JavaScript

The JavaScript code adds a new paragraph to the webpage when the "Add" button is clicked.

```javascript
const Button = document.getElementById('addButton');
const text = document.getElementById('text');
const paragraph = document.getElementById('paragraph');

Button.addEventListener('click', () => {
        const newText = text.value;
        const newParagraph = document.createElement('p');
        newParagraph.textContent = newText;
        paragraph.appendChild(newParagraph);
        text.value = '';
});

