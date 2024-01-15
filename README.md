# Coding Challenge - Carousel

## Goal

Using the HTML below, write a self-executing vanilla JavaScript function that cycles through the images (much like a carousel). Each image should be displayed for roughly 1 second before moving on to the next image.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Carousel</title>
        <style>
            .carousel img {
                display: none;
            }
        </style>
    </head>
    <body>
        <h1>My Carousel</h1>
        <div class="carousel">
            <img alt="First" src="https://placehold.co/350x200?text=1" />
            <img alt="Second" src="https://placehold.co/350x200?text=2" />
            <img alt="Third" src="https://placehold.co/350x200?text=3" />
            <img alt="Fourth" src="https://placehold.co/350x200?text=4" />
            <img alt="Fifth" src="https://placehold.co/350x200?text=5" />
        </div>
        <script>
            // Your Code
        </script>
    </body>
</html>
```

Your output should emulate the included animated gif:

`./carousel.gif`

### Bonus

If you were to use third-party tools to complete this challenge, what would you use? Write a sentence or two describing your reasoning.

## Guidelines

- All code should be written in ES6 JavaScript.
- No third-party libraries or plugins are allowed.
- Documentation and maintainability is a plus.

### Time Allotment

We respect your time and would prefer you not spend more than 3-5 hours. Feel free to include code comments to indicate any features you don't have time to implement.



## STEPS
npm init -y

npm install express

mkdir public
mv index.html public/
mv script.js public/


#server.js
// server.js
const express = require('express');
const app = express();
const path = require('path');

app.use(express.static(path.join(__dirname, 'public')));

const PORT = process.env.PORT || 3000;
app.listen(PORT, () => {
    console.log(`Server is running on http://localhost:${PORT}`);
});


#package json
"scripts": {
    "start": "node server.js"
},


#npm install

#npm start

