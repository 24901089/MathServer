# Ex.05 Design a Website for Server Side Processing
## Date:08-11-2025

## AIM:
 To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side. 


## FORMULA:
P = I<sup>2</sup>R
<br> P --> Power (in watts)
<br> I --> Intensity
<br> R --> Resistance

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Lamp Filament Power Calculator</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin-top: 50px;
    }
    h1 {
      font-size: 28px;
    }
    .input-box {
      margin: 15px 0;
    }
    label {
      display: inline-block;
      width: 200px;
      text-align: right;
      margin-right: 10px;
    }
    input {
      padding: 6px;
      font-size: 16px;
      width: 120px;
    }
    button {
      padding: 8px 20px;
      font-size: 16px;
      margin-top: 15px;
      cursor: pointer;
    }
    #result {
      margin-top: 30px;
      font-size: 24px;
      font-weight: bold;
      border: 2px solid black;
      padding: 15px;
      display: inline-block;
      min-width: 200px;
    }
  </style>
</head>
<body>
  <h1>Lamp Filament Power Calculator</h1>
  <p>Use the formula: P = I²R</p>

  <div class="input-box">
    <label for="current">Current (I) in Amperes:</label>
    <input type="number" id="current" placeholder="Enter current">
  </div>

  <div class="input-box">
    <label for="resistance">Resistance (R) in Ohms:</label>
    <input type="number" id="resistance" placeholder="Enter resistance">
  </div>

  <button onclick="calculatePower()">Calculate Power</button>

  <div id="result">Power = ? W</div>

  <script>
    function calculatePower() {
      let I = parseFloat(document.getElementById("current").value);
      let R = parseFloat(document.getElementById("resistance").value);

      if (isNaN(I) || isNaN(R)) {
        document.getElementById("result").innerText = "Please enter valid numbers!";
        return;
      }

      let P = I * I * R;  // P = I²R
      document.getElementById("result").innerText = "Power = " + P + " W";
    }
  </script>
</body>
</html>
```


## SERVER SIDE PROCESSING:
![alt text](<Screenshot 2025-11-08 182029.png>)


## HOMEPAGE:


## RESULT:
The program for performing server side processing is completed successfully.
