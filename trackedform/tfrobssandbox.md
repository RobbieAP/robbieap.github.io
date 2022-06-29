---
title: An example Basic tracked Form for robs sand box
layout: template
filename: tfrobssandbox.md
--- 
<!-- Ortto robsandbox capture code -->
<script>
    window.ap3c = window.ap3c || {};
    var ap3c = window.ap3c;
    ap3c.cmd = ap3c.cmd || [];
    ap3c.cmd.push(function() {
        ap3c.init('YhgEsfo4U3AQ0Cj0cm9ic2FuZGJveA', 'https://capture-api-master.stgautopilotapp.com/');
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

# A tracked form that is for use on robs sandbox account

* <button onclick="delete_cookie('ap3c')">Delete ap3c Cookie</button> <--- will be set each time no point
* <button onclick="delete_cookie('ap3converted')">Delete ap3converted Cookie</button>
* <button onclick="delete_cookie('ap3dm')">Delete ap3dm Cookie</button>
* <button onclick="delete_cookie('ap3sess')">Delete ap3sess Cookie</button>




<fieldset>
    <legend>Fill out the Basic form:</legend>
<form id="basictrackedformrsb" action="">
  <label for="fnamersb">First name:</label><br>
  <input type="text" id="fnamersb" name="fname" placeholder="First Name"/><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" placeholder="Last Name"/><br>
  <label for="email">Email</label><br>
  <input type="email" id="email" name="email" placeholder="Email"/><br>
  <label for="phone">Phone (tel):</label><br>
  <input type="tel" id="phone" name="phone"/><br>
   <input id="submitrsb" type="submit" value="Submit"/>
</form> 

</fieldset>


