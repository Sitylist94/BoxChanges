# 🎨 Dynamic Box Styler
Welcome to Dynamic Box Styler! This project is a simple yet effective tool for real-time CSS styling. Customize a div element's border-radius and background-color dynamically using an input field. Perfect for learning and experimenting with HTML, CSS, and JavaScript.

# 🚀 Features
Live CSS Styling: Adjust the border-radius and background-color in real-time.
Interactive UI: Immediate visual feedback as you type.
Lightweight & Flexible: Easy to integrate into any project.
# 🛠️ Installation
To get started with this project, simply clone the repository:

bash
Copier le code
git clone https://github.com/YourUsername/DynamicBoxStyler.git
Navigate into the project directory:

bash
Copier le code
cd DynamicBoxStyler
Then, open the index.html file in your favorite web browser to see the tool in action.

# 🧩 Code Overview
# HTML
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
CSS
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
JavaScript
javascript
Copier le code
let box = document.querySelector(".box");
let input = document.querySelector("input");

input.addEventListener("input", () => {
    box.style.borderRadius = input.value;
    box.style.background = input.value;
});
# ✨ Usage
Clone the repository or copy the code above.
Open the index.html file in your web browser.
Start typing CSS values like 50% for border-radius or red for background-color.
Watch the box transform instantly!
# 🌟 Customization
Feel free to customize and extend this project:

Add more input fields to change other CSS properties like box-shadow or border.
Enhance the UI with additional controls like sliders or color pickers.
Integrate this with a larger project as a live CSS editor.
# 💬 Contributing
Contributions are welcome! If you have suggestions for improvements, feel free to open an issue or submit a pull request.

# 📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
