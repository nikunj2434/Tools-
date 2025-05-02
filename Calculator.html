<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Responsive Calculator</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f4f4;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 20px;
      transition: background 0.3s, color 0.3s;
    }
    .dark-mode {
      background: #121212;
      color: #fff;
    }
    .calculator {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
      width: 100%;
      max-width: 320px;
      transition: background 0.3s, color 0.3s;
    }
    .dark-mode .calculator {
      background: #1e1e1e;
      color: #fff;
    }
    input {
      width: 100%;
      height: 50px;
      font-size: 1.5em;
      text-align: right;
      margin-bottom: 10px;
      padding: 10px;
      box-sizing: border-box;
    }
    .buttons {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
    }
    .buttons button {
      width: 23%;
      height: 50px;
      font-size: 1.2em;
      margin: 1% 1%;
      border: none;
      cursor: pointer;
      flex: 1 0 21%;
      box-sizing: border-box;
    }
    .history {
      margin-top: 20px;
      width: 100%;
      max-width: 320px;
      background: #fff;
      border-radius: 10px;
      padding: 10px;
      max-height: 150px;
      overflow-y: auto;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
      transition: background 0.3s, color 0.3s;
    }
    .dark-mode .history {
      background: #1e1e1e;
      color: #fff;
    }
    .toggle {
      margin-bottom: 10px;
    }
    .clear-history {
      float: right;
      font-size: 0.8em;
      cursor: pointer;
      color: red;
    }

    @media (max-width: 400px) {
      .buttons button {
        font-size: 1em;
        height: 45px;
      }
      input {
        font-size: 1.2em;
      }
    }
  </style>
</head>
<body>

  <button class="toggle" onclick="toggleDarkMode()">Toggle Dark Mode</button>

  <div class="calculator">
    <input type="text" id="display" disabled />
    <div class="buttons">
      <button onclick="clearDisplay()">C</button>
      <button onclick="squareRoot()">√</button>
      <button onclick="square()">x²</button>
      <button onclick="reciprocal()">1/x</button>
      <button onclick="appendValue('7')">7</button>
      <button onclick="appendValue('8')">8</button>
      <button onclick="appendValue('9')">9</button>
      <button onclick="appendValue('/')">/</button>
      <button onclick="appendValue('4')">4</button>
      <button onclick="appendValue('5')">5</button>
      <button onclick="appendValue('6')">6</button>
      <button onclick="appendValue('*')">*</button>
      <button onclick="appendValue('1')">1</button>
      <button onclick="appendValue('2')">2</button>
      <button onclick="appendValue('3')">3</button>
      <button onclick="appendValue('-')">-</button>
      <button onclick="appendValue('0')">0</button>
      <button onclick="appendValue('.')">.</button>
      <button onclick="appendValue('%')">%</button>
      <button onclick="appendValue('+')">+</button>
      <button onclick="deleteLast()">←</button>
      <button onclick="calculate()" style="flex: 0 0 73%">=</button>
    </div>
  </div>

  <div class="history" id="history">
    <strong>History <span class="clear-history" onclick="clearHistory()">Clear</span></strong><br/>
    <div id="history-content"></div>
  </div>

  <script>
    const display = document.getElementById("display");
    const historyContent = document.getElementById("history-content");

    function appendValue(value) {
      display.value += value;
    }

    function clearDisplay() {
      display.value = '';
    }

    function deleteLast() {
      display.value = display.value.slice(0, -1);
    }

    function squareRoot() {
      try {
        const result = Math.sqrt(eval(display.value));
        addToHistory(`√(${display.value}) = ${result}`);
        display.value = result;
      } catch {
        display.value = 'Error';
      }
    }

    function square() {
      try {
        const result = Math.pow(eval(display.value), 2);
        addToHistory(`(${display.value})² = ${result}`);
        display.value = result;
      } catch {
        display.value = 'Error';
      }
    }

    function reciprocal() {
      try {
        const result = 1 / eval(display.value);
        addToHistory(`1/(${display.value}) = ${result}`);
        display.value = result;
      } catch {
        display.value = 'Error';
      }
    }

    function calculate() {
      try {
        const result = eval(display.value.replace('%', '/100'));
        addToHistory(`${display.value} = ${result}`);
        display.value = result;
      } catch {
        display.value = 'Error';
      }
    }

    function toggleDarkMode() {
      document.body.classList.toggle("dark-mode");
    }

    function addToHistory(entry) {
      const entries = JSON.parse(localStorage.getItem("calcHistory")) || [];
      entries.push(entry);
      localStorage.setItem("calcHistory", JSON.stringify(entries));
      renderHistory();
    }

    function renderHistory() {
      const entries = JSON.parse(localStorage.getItem("calcHistory")) || [];
      historyContent.innerHTML = entries.map(e => `<div>${e}</div>`).join('');
    }

    function clearHistory() {
      localStorage.removeItem("calcHistory");
      renderHistory();
    }

    document.addEventListener('keydown', function(e) {
      const key = e.key;
      if (!isNaN(key) || "+-*/.%".includes(key)) {
        appendValue(key);
      } else if (key === "Enter") {
        calculate();
      } else if (key === "Backspace") {
        deleteLast();
      }
    });

    window.onload = renderHistory;
  </script>

</body>
</html>
