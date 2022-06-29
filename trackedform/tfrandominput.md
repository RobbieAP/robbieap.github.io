---
title: An example Basic tracked Form for other input values
layout: template
filename: basictrackedform.md
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

# A tracked form that tests other values

* <button onclick="delete_cookie('ap3c')">Delete ap3c Cookie</button> <--- will be set each time no point
* <button onclick="delete_cookie('ap3converted')">Delete ap3converted Cookie</button>
* <button onclick="delete_cookie('ap3dm')">Delete ap3dm Cookie</button>
* <button onclick="delete_cookie('ap3sess')">Delete ap3sess Cookie</button>




<fieldset>
    <legend>A basic form to fillout:</legend>
<form id="basictrackedform" action="">
  <label for="decimal">First name:</label><br>
  <input type="text" id="decimal" name="Decimal Text" placeholder="0.05"/><br>
  <label for="currency">Last name:</label><br>
  <input type="number" id="currency" name="Currency Number"/><br>
  <label for="email">Email</label><br>
  <input type="email" id="email" name="email" placeholder="Email"/><br>
  <label for="checktrue">Checkbox</label><br>
  <input type="checkbox" id="checktrue" name="Check Me"/><br>
   <label for="number">Number:</label><br>
  <input type="number" id="number" name="Number"/><br>
   <input id="submit" type="submit" value="Submit"/>
</form> 

</fieldset>


