<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Survey Form</title>
<style>
body {
font-family: Courier New;
margin: 0;
padding: 20px;
background-color: #7FB3D5;
}

.container {
max-width: 800px;
margin: 0 auto;
padding: 20px;
}

h1 {
text-align: center;
margin-bottom: 20px;
}

form {
display: grid;
grid-template-columns: 1fr 1fr;
grid-gap: 20px;
}

label {
display: block;
margin-bottom: 5px;
}

input[type="text"],
textarea {
width: 90%;
padding: 10px;
margin-bottom: 20px;
}

button[type="submit"] {
background-color: #7FB3D5;
color: white;
padding: 10px 20px;
border: none;
cursor: pointer;
width: 100%;
}

@media (max-width: 768px) {
form {
grid-template-columns: 1fr;
}
}
</style>
</head>
<body>
<h1>Survey Form</h1>
<div>
<label for="name">Name:</label>
<input type="text" id="name" name="name" required>
</div>
<div>
<label for="email">Email:</label>
<input type="text" id="email" email="email" required>
</div>
<div>
<label for="age">Age(optional):</label>
<input type="text" id="age" age="age" optional>
</div>
<form action="#" method="post">
<fieldset>
<legend>Is this course your 1st choice?</legend>
<label for="yes">Yes</label>
<input type="radio" id="yes" name="answer" value="yes" required />
<label for="no">No</label>
<input type="radio" id="no" name="answer" value="no" required />
</fieldset>
<fieldset>
<legend>What course would you take(if yes)</legend>
<textarea id="answer" name="answer"></textarea>
</fieldset>
<fieldset>
  <legend>Do you think you can easily find a job after you graduate?</legend>
  <label for="yes">Yes</label>
<input type="radio" id="yes" name="answer" value="yes" required />
<label for="no">No</label>
<input type="radio" id="no" name="answer" value="no" required />
</fieldset>
<fieldset>
<legend>What job are you trying to get?</legend>
<textarea id="answer" name="answer"></textarea>
</fieldset>
<button type="submit">Submit</button>
</form>
<div class="container">

