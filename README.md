<!DOCTYPE html>
<html>

<head>
<title>BMI Calculator</title>
</head>

<body>

<h2>BMI Calculator</h2>

<input id="height" placeholder="Enter height (meters)">
<br><br>

<input id="weight" placeholder="Enter weight (kg)">
<br><br>

<button onclick="calculateBMI()">Calculate BMI</button>

<p id="result"></p>

<script>

function calculateBMI(){

let h = document.getElementById("height").value;
let w = document.getElementById("weight").value;

let bmi = w / (h*h);

if(bmi < 18.5){
document.getElementById("result").innerText = "Underweight";
}

else if(bmi < 25){
document.getElementById("result").innerText = "Normal weight";
}

else if(bmi < 30){
document.getElementById("result").innerText = "Overweight";
}

else{
document.getElementById("result").innerText = "Obese";
}

}

</script>

</body>

</html>
