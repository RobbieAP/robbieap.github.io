---
title: An example Basic tracked Form with no labels
layout: template
filename: basictrackedformnolabels.md
--- 
<!-- Ortto robert capture code -->
<script>
    window.ap3c = window.ap3c || {};
    var ap3c = window.ap3c;
    ap3c.cmd = ap3c.cmd || [];
    ap3c.cmd.push(function() {
        ap3c.init('YdOVzkqoVlq0G5Pscm9iZXJ0', 'https://subtracking.robs.qa.lulzderp.com/');
        ap3c.track({v: 0});
    });
    ap3c.activity = function(act) { ap3c.act = (ap3c.act || []); ap3c.act.push(act); };
    var s, t; s = document.createElement('script'); s.type = 'text/javascript'; s.src = "https://subtracking.robs.qa.lulzderp.com/app.js";
    t = document.getElementsByTagName('script')[0]; t.parentNode.insertBefore(s, t);
</script>




<script>
let delete_cookie = function(name) {
    document.cookie = name +'=; Path=/; Expires=Thu, 01 Jan 1970 00:00:01 GMT;';
	console.log("Deleted ", name, "cookie");
};
</script>

# A tracked form example that has ids but no labels

* <button onclick="delete_cookie('ap3c')">Delete ap3c Cookie</button> <--- will be set each time no point
* <button onclick="delete_cookie('ap3converted')">Delete ap3converted Cookie</button>
* <button onclick="delete_cookie('ap3dm')">Delete ap3dm Cookie</button>
* <button onclick="delete_cookie('ap3sess')">Delete ap3sess Cookie</button>




<fieldset>
    <legend>Fill out the Basic form that has no labels:</legend>
<form id="nolabels" action="">
  <input type="text" id="fname"  placeholder="First Name"/><br>
  <input type="text" id="lname"  placeholder="Last Name"/><br>
  <input type="email" id="email"  placeholder="Email"/><br>
  <input type="tel" id="phone"  placeholder="Phone"/><br>
   <input id="submit" type="submit" value="Submit"/>
</form> 

</fieldset>


