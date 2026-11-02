# Modern Temperature Converter

A sleek, responsive, single-page Web application designed for converting temperature values across **Celsius (°C)**, **Fahrenheit (°F)**, and **Kelvin (K)** in real-time. Built with pure HTML, Tailwind CSS, and vanilla JavaScript, it features a glassmorphism dark-mode UI with absolute zero safety validations and dynamic formula explanations.

---

## 🌟 Key Features

* **Real-time Conversion**: Automatically calculates temperature values across all units as you type.
* **Absolute Zero Validation**: Prevents invalid temperature entries below absolute zero ($0\text{ K}$, $-273.15^\circ\text{C}$, $-459.67^\circ\text{F}$) with visual warning alerts.
* **Dynamic Formula Display**: Shows the exact mathematical conversion formulas applied to the user's input.
* **Modern Glassmorphism UI**: Built with Tailwind CSS, custom neon glowing background accents, and smooth gradient highlights.
* **Keyboard Shortcuts & Quick Actions**:
  * `Escape` key clears input fields when focused.
  * One-click input clear button ($\otimes$).
  * Master reset button to restore default UI state.
* **Quick Reference Guide**: Direct footer references for Absolute Zero, Water Freezing Point, and Water Boiling Point.

---

## 📐 Mathematical Formulas Applied

The converter standardizes calculations across the three scales using the following formulas:

### 1. From Celsius ($C$)
* **To Fahrenheit**:  
  $$F = \left(C \times \frac{9}{5}\right) + 32$$
* **To Kelvin**:  
  $$K = C + 273.15$$

---

### 2. From Fahrenheit ($F$)
* **To Celsius**:  
  $$C = (F - 32) \times \frac{5}{9}$$
* **To Kelvin**:  
  $$K = \left((F - 32) \times \frac{5}{9}\right) + 273.15$$

---

### 3. From Kelvin ($K$)
* **To Celsius**:  
  $$C = K - 273.15$$
* **To Fahrenheit**:  
  $$F = \left((K - 273.15) \times \frac{9}{5}\right) + 32$$

---

## 🚀 Getting Started

Since this project is contained within a standalone single HTML file, setup requires no build tools or package installation.

### Prerequisites

All external libraries (Tailwind CSS, Font Awesome, Google Fonts) are included via CDN:
* **Tailwind CSS CDN**
* **Font Awesome v6.4.0**
* **Google Fonts (Plus Jakarta Sans)**

### Running the Application

1. Save your project code as `index.html`.
2. Open `index.html` directly in any modern web browser (Google Chrome, Firefox, Safari, Edge).

---

## 🛠️ Project Structure

```text
├── index.html       # Single-file HTML application containing UI, Tailwind setup, and JavaScript logic
└── README.md        # Documentation file
```

---

## ⚙️ Technical Highlights

* **Input Sanitization & Regex Check**: Verifies valid numerical inputs matching `^-?\d*\.?\d*$`.
* **Dynamic Styling**: Active target unit card updates dynamically with custom border neon glows (`cyan`, `blue`, `purple`).
* **Zero Dependencies Setup**: Runs in any environment without needing Node.js or additional bundlers.