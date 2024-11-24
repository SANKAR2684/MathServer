# Ex.05 Design a Website for Server Side Processing
## Date:24/11/24

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
<html>
<head>
    <title>Power Calculater</title>
    <script>
        function calculate() {
            const Intesity = parseFloat(document.getElementById('t1').value);
            const Resistance = parseFloat(document.getElementById('t2').value);
           
            if (isNaN(Intesity) || isNaN(Resistance)) {
                alert("Please enter valid numbers.");
                return;
            }

            const Power = (Intesity * Intesity ) * Resistance;
            document.getElementById('t3').innerText = "The power of the bulb : " + Power+ " watts";
        }
    </script>
</head>
<body align="center" bgcolor="cyan">
    
    <h1>The Power of the lamb </h1>

    <label for="Intensity">Intensity:</label>
  
    <input type="number" id="t1" placeholder="Enter the Intensity value"> <label for="Intensity"> A</label><br><br>
    
    <label for="Resistance">Resistance:</label>
    
    <input type="number" id="t2" placeholder="Enter the Resistance value"><label for="Resistance">Ohm</label><br><br>
    
    <button onclick="calculate()">Calculate</button>

    <p id="t3"></p>

</body>
</html>

## SERVER SIDE PROCESSING:


## HOMEPAGE:
![alt text](<Screenshot 2024-11-24 102327.png>)

## RESULT:
The program for performing server side processing is completed successfully.
