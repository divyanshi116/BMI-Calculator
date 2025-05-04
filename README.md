# 🧮 BMI Calculator

The **BMI Calculator** is a simple, responsive web-based application that allows users to calculate their Body Mass Index (BMI). It provides immediate feedback on the BMI value and categorizes it (e.g., Underweight, Normal weight, Overweight, or Obese) based on standard BMI ranges. Designed with an intuitive interface, visual appeal, and a responsive layout, this calculator is perfect for personal use or educational demonstrations.

---

## 🌟 Features

- **Interactive BMI Calculation**: Users can input their height and weight to instantly calculate their BMI.
- **Clear BMI Categories**: The app categorizes the BMI into:
  - Underweight
  - Normal weight
  - Overweight
  - Obese
- **Responsive Design**: Works seamlessly on various devices, including desktops, tablets, and smartphones.
- **User-Friendly Interface**: Simple input fields and a visually appealing design for better usability.
- **Real-time Feedback**: Displays the calculated BMI and corresponding category immediately after input.

---

## 🛠️ Technologies Used

- **HTML**: For the structure and layout of the web page.
- **CSS**: To enhance the visual appearance and responsiveness of the application.
- **JavaScript**: For the BMI calculation logic and interactivity.

---

## 🚀 Getting Started

### Prerequisites

To run this project, you only need a modern web browser (e.g., Chrome, Firefox, Safari, Edge). No additional software installation is required.

---

### Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/divyanshi116/BMI-Calculator.git
   ```
2. Navigate to the project folder:
   ```bash
   cd BMI-Calculator
   ```
3. Open the `bmi.html` file in your browser:
   ```bash
   open bmi.html
   ```
   Alternatively, drag and drop the `bmi.html` file into your browser.

---

## 🖥️ Usage

1. Enter your **Height** (in centimeters) in the respective input field.
2. Enter your **Weight** (in kilograms) in the respective input field.
3. Click the **"Calculate"** button.
4. View your BMI result and category displayed below the button.

---

## 📂 Project Structure

This project is organized into three main files:

- **`bmi.html`**: The main HTML file containing the structure of the application.
- **`style.css`**: The CSS file for styling and responsive design.
- **`script.js`**: The JavaScript file containing the logic for BMI calculation and real-time feedback.

---

## 🎯 Example

### Input:
- Height: 170 cm
- Weight: 70 kg

### Output:
- BMI: 24.22
- Category: Normal weight

---

## 📝 Code Overview

### BMI Calculation Logic

The BMI is calculated using the formula:
\[ \text{BMI} = \frac{\text{Weight (kg)}}{\left(\frac{\text{Height (cm)}}{100}\right)^2} \]

**Example Code Snippet from `script.js`:**
```javascript
var bmi = weight / ((height / 100) ** 2);
var category = "";
if (bmi < 18.5) {
  category = "Underweight";
} else if (bmi < 25) {
  category = "Normal weight";
} else if (bmi < 30) {
  category = "Overweight";
} else {
  category = "Obese";
}
resultDiv.innerHTML = "Your BMI is " + bmi.toFixed(2) + " (" + category + ")";
```

### Styling Highlights

The app uses **Google Fonts** for typography and provides hover effects for buttons and containers for a modern and dynamic experience. It includes responsive design to adapt to small screens.

**Example Code Snippet from `style.css`:**
```css
.container {
    max-width: 400px;
    padding: 30px;
    background-color: #ffffff;
    border-radius: 10px;
    box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1);
    text-align: center;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.container:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
}
```

---

## 📋 Features Breakdown

### Input Fields
- **Height**: Accepts numerical input for height in centimeters.
- **Weight**: Accepts numerical input for weight in kilograms.

### Button
- **Calculate**: Triggers the BMI calculation and displays the result.

### Result
- Displays the calculated BMI value with two decimal places.
- Indicates the BMI category (e.g., Normal weight).

---

## 📱 Responsive Design

The application is fully responsive and adjusts seamlessly for different screen sizes. Media queries are used to provide a better user experience on smaller devices.

**Example Code Snippet from `style.css`:**
```css
@media (max-width: 480px) {
    .container {
        padding: 20px;
        margin: 10px;
    }
    h1 {
        font-size: 22px;
    }
    input[type="number"], button {
        font-size: 14px;
        padding: 10px;
    }
    #result {
        font-size: 16px;
    }
}
```

---

## 🔧 Possible Enhancements

- Add **imperial units** (feet, inches, pounds) for height and weight inputs.
- Include **health tips** based on the BMI category.
- Allow **keyboard shortcuts** for better accessibility.
- Integrate **graphical representation** of BMI ranges.
- Provide **local storage** to save previous BMI calculations.

---

## 🤝 Contributing

Contributions are always welcome! If you have ideas for improvements or find a bug, feel free to fork the repository and create a pull request.

### Steps to Contribute:

1. Fork the repository.
2. Create a new branch for your feature/bugfix:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add new feature or fix"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request and describe your changes.

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 📧 Contact

For questions, suggestions, or feedback, feel free to reach out to [divyanshi116](https://github.com/divyanshi116). 🚀
