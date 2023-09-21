---
title: An example Basic tracked Form with hidden fields
layout: template
filename: tfhiddenfields.md
--- 

<!-- Ortto robert capture code -->
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
    <legend>Fill out the Basic form that contains some static hidden fields:</legend>
<form id="tfwithhideenfields" action="" onsubmit="return false;">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" placeholder="First Name"/><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" placeholder="Last Name"/><br>
  <label for="email">Email</label><br>
  <input type="email" id="email" name="email" placeholder="Email"/><br>
  <label for="phone">Phone (tel):</label><br>
  <input type="tel" id="phone" name="phone"/><br>
  
  <!-- Hidden -->
  <input type="hidden" id="hiddenphone2" value='0430000000' name="hidden phone"/><br>
  <input type="hidden"  name="UTM_Campaign" value="[utm_campaign]"/><br>
  <input type="hidden" id="hidden3" name="UTM_Source" value="[utm_source]"/><br>
  <input type="hidden" id="hiddenfalsy" name="a false value", value='false' /><br>
  <input type="hidden" id="hiddentruthy" name="a true value", value='true' /><br>
  <input type="hidden" id="hiddennumeric" name="a number value", value=1234567 /><br>
  <input id="submit" type="submit" value="Submit"/>
</form> 

</fieldset>


