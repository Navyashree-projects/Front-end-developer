body {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: #f4f4f4;
    font-family: Arial, sans-serif;
    margin: 0;
}

.calculator {
    background-color: #333;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
    padding: 20px;
    width: 320px;
}

.calculator-display {
    width: calc(100% - 20px);
    background-color: #222;
    color: #0f0; /* Green display for retro feel */
    font-size: 2.5em;
    border: none;
    border-radius: 5px;
    padding: 10px;
    margin-bottom: 20px;
    text-align: right;
    box-sizing: border-box;
}

.calculator-buttons {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
}

.button {
    background-color: #555;
    color: #fff;
    border: none;
    border-radius: 5px;
    padding: 20px;
    font-size: 1.5em;
    cursor: pointer;
    transition: background-color 0.2s ease;
}

.button:hover {
    background-color: #666;
}

.button.operator {
    background-color: #f79234; /* Orange for operators */
}

.button.operator:hover {
    background-color: #ff9d4a;
}

.button.equals {
    background-color: #28a745; /* Green for equals */
    grid-column: span 2; /* Make equals button span two columns */
}

.button.equals:hover {
    background-color: #2fb94e;
}

.button.zero {
    grid-column: span 2; /* Make zero button span two columns */
}

.button.decimal {
    background-color: #555;
}
