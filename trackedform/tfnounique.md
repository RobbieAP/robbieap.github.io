---
title: An example Basic tracked Form
layout: template
filename: tfnounique.md
--- 
<!-- Ortto robert capture code -->
<script>
    window.ap3c = window.ap3c || {};
    var ap3c = window.ap3c;
    ap3c.cmd = ap3c.cmd || [];
    ap3c.cmd.push(function() {
        ap3c.init('YdOVzkqoVlq0G5Pscm9iZXJ0', 'https://testsubdomain.robs2.qa.lulzderp.com/');
        ap3c.track({v: 0});
    });
    ap3c.activity = function(act) { ap3c.act = (ap3c.act || []); ap3c.act.push(act); };
    var s, t; s = document.createElement('script'); s.type = 'text/javascript'; s.src = "https://testsubdomain.robs2.qa.lulzderp.com/app.js";
    t = document.getElementsByTagName('script')[0]; t.parentNode.insertBefore(s, t);
</script>


<script>
let delete_cookie = function(name) {
    document.cookie = name +'=; Path=/; Expires=Thu, 01 Jan 1970 00:00:01 GMT;';
	console.log("Deleted ", name, "cookie");
};
</script>

# A tracked form with no unique identifier for capture e.g email or phone

* <button onclick="delete_cookie('ap3c')">Delete ap3c Cookie</button> <--- will be set each time no point
* <button onclick="delete_cookie('ap3converted')">Delete ap3converted Cookie</button>
* <button onclick="delete_cookie('ap3dm')">Delete ap3dm Cookie</button>
* <button onclick="delete_cookie('ap3sess')">Delete ap3sess Cookie</button>




<fieldset>
    <legend>Fill out the Basic form:</legend>
<form id="nouniqueform" action="">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" placeholder="First Name"/><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" placeholder="Last Name"/><br> 
   <input id="submit" type="submit" value="Submit"/>
</form> 

</fieldset>


