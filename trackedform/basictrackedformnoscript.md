---
title: An example Basic tracked Form with no capture script
layout: template
filename: basictrackedformnoscript.md
--- 

<script>
let delete_cookie = function(name) {
    document.cookie = name +'=; Path=/; Expires=Thu, 01 Jan 1970 00:00:01 GMT;';
	console.log("Deleted ", name, "cookie");
};
</script>

# A tracked form that has no capture script

* <button onclick="delete_cookie('ap3c')">Delete ap3c Cookie</button> <--- will be set each time no point
* <button onclick="delete_cookie('ap3converted')">Delete ap3converted Cookie</button>
* <button onclick="delete_cookie('ap3dm')">Delete ap3dm Cookie</button>
* <button onclick="delete_cookie('ap3sess')">Delete ap3sess Cookie</button>




<fieldset>
    <legend>Fill out the Basic form:</legend>
<form action="">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" placeholder="First Name"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" placeholder="Last Name"><br>
  <label for="email">Email</label><br>
  <input type="email" id="email" name="email" placeholder="Email"><br>
  <label for="phone">Phone (tel):</label><br>
  <input type="tel"><br>
   <input type="submit" value="Submit">
</form> 

</fieldset>


