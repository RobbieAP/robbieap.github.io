---
title: An example with two tracked Forms
layout: template
filename: twoforms.md
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
    <legend>Fill out form1:</legend>
<form id="form1" action="">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" placeholder="First Name"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" placeholder="Last Name"><br>
  <label for="email">Email</label><br>
  <input type="email" id="email" name="email" placeholder="Email"><br>
  <label for="phone">Phone (tel):</label><br>
  <input type="tel" id="phone" name="phone"><br>
   <input id="form1submit" type="submit" value="Submit">
</form> 

</fieldset>


<fieldset id="form2fieldset">
    <legend>Fill out form2:</legend>
<form id="form2" action="">
  <label for="fname2">First name:</label><br>
  <input type="text" id="fname2" name="fname2" placeholder="First Name"><br>
  <label for="lname2">Last name:</label><br>
  <input type="text" id="lname2" name="lname2" placeholder="Last Name"><br>
  <label for="email2">Email</label><br>
  <input type="email" id="email2" name="email2" placeholder="Email"><br>
  <label for="form2uniquetext">Form2 Unique Text</label><br>
  <input type="text" id="form2uniquetext" name="form2uniquetext"><br>
  <br>

  <input type="radio" id="yes" name="radioselection" value="yes">
  <label for="yes">yes</label><br>  
  <input type="radio" id="no" name="radioselection" value="no">
  <label for="no">no</label><br>

   <input id="form2submit" type="submit" value="Submit">
</form> 

</fieldset>