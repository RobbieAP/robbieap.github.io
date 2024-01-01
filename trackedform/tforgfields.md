---
title: An example tracked form for org fields
layout: template
filename: tforgfields.md
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

# A tracked form example that has org type fields only

* <button onclick="delete_cookie('ap3c')">Delete ap3c Cookie</button> <--- will be set each time no point
* <button onclick="delete_cookie('ap3converted')">Delete ap3converted Cookie</button>
* <button onclick="delete_cookie('ap3dm')">Delete ap3dm Cookie</button>
* <button onclick="delete_cookie('ap3sess')">Delete ap3sess Cookie</button>




<fieldset>
    <legend>These should be mapped to org fields:</legend>
<form id="orgform" action="">
  <label for="orgname">Org Name:</label><br>
  <input type="text" id="orgname" name="Org name" placeholder="Org Name"/><br>
  <label for="industry">Industry:</label><br>
  <input type="text" id="industry" name="Industry" placeholder="Industry"/><br>
  <label for="website">Website</label><br>
  <input type="email" id="website" name="Website" placeholder="Website"/><br>
  <label for="text">Generic Text:</label><br>
  <input type="text" id="text" name="Generic Text"/><br>
   <input id="submitorgform" type="submit" value="Submit"/>
</form> 

</fieldset>


