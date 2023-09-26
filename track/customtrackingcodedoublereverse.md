---
title: Custom tracking code with two values number and text
layout: template
filename: customtrackingcodereverse.md
--- 

<!-- Robs cookie deleter capture code -->
<script>
	
var runDeleteCookie = true;	
	
if(runDeleteCookie){	
	
let COOKIESTODELETE = ["ap3c", "ap3converted", "ap3dm", "ap3sess"];
	
let delete_cookie = function(name) {
    document.cookie = name +'=; Path=/; Expires=Thu, 01 Jan 1970 00:00:01 GMT;';
	console.log("Deleted ", name, "cookie");
};

COOKIESTODELETE.forEach((name) => delete_cookie(name));
	
	runDeleteCookie = false;
	}
	
</script>


<!-- Autopilot robert capture code -->
<script>
	window.ap3c = window.ap3c || {};
	var ap3c = window.ap3c;
	ap3c.cmd = ap3c.cmd || [];
	ap3c.cmd.push(function() {
		ap3c.init('YdOVzkqoVlq0G5Pscm9iZXJ0', 'https://capture-api-master.stgautopilotapp.com/');
		ap3c.track({v: 0,  "ac" : [ {"fi": 'int:cm:exnumber', 'v': 112233},{"fi": "str:cm:generic-text", "v": "numberfirstthentext" }]});
	});
	var s, t; s = document.createElement('script'); s.type = 'text/javascript'; s.src = "https://static.ap3stg.com/capture/master/capture.js";
	t = document.getElementsByTagName('script')[0]; t.parentNode.insertBefore(s, t);
</script>

field: exnumber value: 112233
field: generic-text value: numberfirstthentext


Custom association tracking { "ac" : [ {}, {}, {}, ]}  with a double object
