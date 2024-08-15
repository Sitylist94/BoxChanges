🎨 Dynamic Box Styler
Welcome to Dynamic Box Styler—a simple yet powerful tool to explore the magic of CSS and JavaScript! Customize the style of a div element in real-time by just typing in your desired values. Perfect for web developers and designers who love experimenting with live styling!

🚀 Features
Live Styling: Modify the border-radius and background-color of a box dynamically with an input field.
Interactive UI: The responsive design allows you to see changes immediately as you type.
Flexible Design: Adjust the box's appearance with any valid CSS values.
🛠️ How It Works
This tool is powered by a combination of HTML, CSS, and JavaScript:

The div box is styled with a solid border and an initial size of 200x200 pixels.
An input field is provided to allow real-time customization.
As you type in the input field, the border-radius and background-color of the box are updated dynamically using JavaScript.
🧩 Code Overview
html
Copier le code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dynamic Box Styler</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="box"></div>
    <input type="text" placeholder="Enter border-radius or color..." />

    <script src="script.js"></script>
</body>
</html>
css
Copier le code
* {
    margin: 0;
    padding: 0;
    background: white;
}

body {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-top: 250px;
}

.box {
    height: 200px;
    width: 200px;
    border: 2px solid black;
    transition: all 0.4s ease;
}

input {
    background-color: white;
    height: 25px;
    width: 200px;
    margin-top: 10px;
    padding: 5px;
}
javascript
Copier le code
let box = document.querySelector(".box");
let input = document.querySelector("input");

input.addEventListener("input", () => {
    box.style.borderRadius = input.value;
    box.style.background = input.value;
});
✨ Try It Yourself!
Clone the repository or copy the code above.
Open the index.html file in your favorite browser.
Start typing CSS values like 50% for border-radius or red for background-color.
Watch as the box transforms instantly!
🌟 Customize and Extend
Feel free to customize this tool further:

Add more input fields to change other CSS properties like box-shadow or border.
Enhance the user experience by adding a color picker or slider.
Integrate with a larger project to create a live CSS editor.
💬 Feedback
We'd love to hear your thoughts and see how you've used Dynamic Box Styler in your projects! Share your feedback and ideas to improve this tool.
