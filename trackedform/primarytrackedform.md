---
title: An example Tracked Form
layout: template
filename: primarytrackedform.md
--- 
<!-- Autopilot robert capture code -->
<script>
	window.ap3c = window.ap3c || {};
	var ap3c = window.ap3c;
	ap3c.cmd = ap3c.cmd || [];
	ap3c.cmd.push(function() {
		ap3c.init('YdOVzkqoVlq0G5Pscm9iZXJ0', 'https://capture-api-master.stgautopilotapp.com/');
		ap3c.track({v: 0});
	});
	var s, t; s = document.createElement('script'); s.type = 'text/javascript'; s.src = "https://static.ap3stg.com/capture/master/capture.js";
	t = document.getElementsByTagName('script')[0]; t.parentNode.insertBefore(s, t);
</script>

<script>
let delete_cookie = function(name) {
    document.cookie = name +'=; Path=/; Expires=Thu, 01 Jan 1970 00:00:01 GMT;';
	console.log("Deleted ", name, "cookie");
};
</script>


# A tracked form example

* <button onclick="delete_cookie('ap3c')">Delete ap3c Cookie</button> <--- will be set each time no point
* <button onclick="delete_cookie('ap3converted')">Delete ap3converted Cookie</button>
* <button onclick="delete_cookie('ap3dm')">Delete ap3dm Cookie</button>
* <button onclick="delete_cookie('ap3sess')">Delete ap3sess Cookie</button>




<fieldset>
    <legend>Fill out the form:</legend>
<form id="allfieldsform" action="">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" placeholder="First Name"/><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" placeholder="Last Name"/><br>
  <label for="email">Email</label><br>
  <input type="email" id="email" name="email" placeholder="Email"/><br>
  <label for="phone">Phone:</label><br>
  <input type="tel" id="phone" name="phone"><br>

  <label for="color">Fav Colour:</label><br>
  <input type="color" id="color" name="color"/><br>

  <label for="checkbox">Check this box:</label><br>
  <input type="checkbox" id="checkbox" name="checkbox" value="checked!"/><br>

<label for="date">A Date:</label><br>
<input type="date" id="date" name="date"/><br>

<label for="datetime">A DateTime:</label><br>
<input type="datetime-local" id="datetime" name="datetime"/><br>

<label for="hidden">A Hidden field:</label><br>
<input type="hidden" id="hidden" name="hidden" value="hiddenvalue"/><br>


<label for="month">A Month:</label><br>
<input type="month" id="month" name="month"/><br>

<label for="week">A week:</label><br>
<input type="week" name="week" id="week"/><br>

<label for="number">A Number:</label><br>
<input type="number" id="number" name="number"/><br>

<label for="password">A Password:</label><br>
<input type="password" id="password" name="password"/><br>

<label for="radio1">True</label><br>
<input type="radio" id="radio1" name="radio" value="true"/><br>

<label for="radio2">False</label><br>
<input type="radio" id="radio2" name="radio" value="false"/><br>

<label for="range">A Range slider:</label><br>
<input type="range" id="range" name="range"/><br>

<label for="text">A Textfield:</label><br>
<input type="text" id="text" name="text"/><br>

<label for="time">A Time input:</label><br>
<input type="time" id="time" name="time"/><br>

<label for="url">URL:</label><br>
<input type="url" id="url" name="url"/><br><br>
 
  <input type="submit" value="Submit"/>
</form> 

</fieldset>


