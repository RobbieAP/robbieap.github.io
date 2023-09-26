---
title: Custom tracking code with double value
layout: template
filename: customtrackingcodedoubletwoint.md
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
		ap3c.track({v: 0,  "ac" : [ {"fi": 'int:cm:apinumber', 'v': 5555588}, {"fi": 'int:cm:exnumber', 'v': 45444777} ]});
	});
	var s, t; s = document.createElement('script'); s.type = 'text/javascript'; s.src = "https://static.ap3stg.com/capture/master/capture.js";
	t = document.getElementsByTagName('script')[0]; t.parentNode.insertBefore(s, t);
</script>
Two ints
field: int:cm:apinumber value: 5555588
field: exnumber value: 45444777

Custom association tracking { "ac" : [ {}, {}, {}, ]}  with a double object
