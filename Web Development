<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Temperature Converter</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 20px;
        }
        
        input, select, button {
            margin-bottom: 10px;
            padding: 8px;
            font-size: 16px;
        }
        
        #result {
            font-size: 18px;
            font-weight: bold;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <h2>Temperature Converter</h2>
    <input type="number" id="temperatureInput" placeholder="Enter temperature" required>
    
    <select id="unitSelector">
        <option value="celsius">Celsius</option>
        <option value="fahrenheit">Fahrenheit</option>
        <option value="kelvin">Kelvin</option>
    </select>
    
    <button onclick="convertTemperature()">Convert</button>
    
    <div id="result"></div>

    <script>
        function convertTemperature() {
            var temperatureInput = document.getElementById("temperatureInput").value;
            var unitSelector = document.getElementById("unitSelector").value;
            var resultDisplay = document.getElementById("result");
            
            if (isNaN(temperatureInput)) {
                resultDisplay.innerHTML = "Please enter a valid number.";
                return;
            }

            var convertedTemperature;
            
            if (unitSelector === "celsius") {
                convertedTemperature = (parseFloat(temperatureInput) - 32) * (5/9);
                resultDisplay.innerHTML = "Converted Temperature: " + convertedTemperature.toFixed(2) + " °C";
            } else if (unitSelector === "fahrenheit") {
                convertedTemperature = (parseFloat(temperatureInput) * 9/5) + 32;
                resultDisplay.innerHTML = "Converted Temperature: " + convertedTemperature.toFixed(2) + " °F";
            } else if (unitSelector === "kelvin") {
                convertedTemperature = parseFloat(temperatureInput) + 273.15;
                resultDisplay.innerHTML = "Converted Temperature: " + convertedTemperature.toFixed(2) + " K";
            }
        }
    </script>
</body>
</html>
