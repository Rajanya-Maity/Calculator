# Calculator
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Calculator</title>
  <link rel="stylesheet" href="style.css"> <!-- Linking CSS -->
</head>
<body>
  <div class="calculator">
    <input type="text" id="display" readonly> <!-- Display area for result -->
    <div class="buttons">
      <!-- Calculator buttons -->
      <button onclick="clearDisplay()">C</button>
      <button onclick="appendToDisplay('7')">7</button>
      <button onclick="appendToDisplay('8')">8</button>
      <button onclick="appendToDisplay('9')">9</button>
      <button onclick="appendToDisplay('/')">÷</button>
      <button onclick="appendToDisplay('4')">4</button>
      <button onclick="appendToDisplay('5')">5</button>
      <button onclick="appendToDisplay('6')">6</button>
      <button onclick="appendToDisplay('*')">×</button>
      <button onclick="appendToDisplay('1')">1</button>
      <button onclick="appendToDisplay('2')">2</button>
      <button onclick="appendToDisplay('3')">3</button>
      <button onclick="appendToDisplay('-')">−</button>
      <button onclick="appendToDisplay('0')">0</button>
      <button onclick="appendToDisplay('.')">.</button>
      <button onclick="calculate()">=</button>
      <button onclick="appendToDisplay('+')">+</button>
    </div>
  </div>

  <script src="script.js"></script> <!-- Linking JS -->
</body>
</html>

body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: #f3f4f6;
  font-family: Arial, sans-serif;
  margin: 0;
}

.calculator {
  background-color: #fff;
  padding: 20px;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

#display {
  width: 100%;
  height: 50px;
  font-size: 1.5rem;
  margin-bottom: 10px;
  text-align: right;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 6px;
}

.buttons {
  display: grid;
  grid-template-columns: repeat(4, 60px);
  gap: 10px;
}

button {
  height: 60px;
  font-size: 1.2rem;
  border: none;
  border-radius: 8px;
  background-color: #e2e8f0;
  cursor: pointer;
  transition: background-color 0.4s;
}

button:hover {
  background-color: #cbd5e0;
}
