---
title: Zendesk webWidget
layout: template
filename: webWidget.md
--- 


# Zendesk webWidget - no tracking code  but will need to open incognito



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


<!-- Start of d3v-robautopilot Zendesk Widget script -->
<script id="ze-snippet" src="https://static.zdassets.com/ekr/snippet.js?key=8ad005b2-c6ed-454f-a85e-73af0e699eea"> </script>
<!-- End of d3v-robautopilot Zendesk Widget script -->

<script>
  
  function deleteZendeskLocal(){
    
  for(let [key, value] of Object.entries(localStorage)){
    if (key.includes("appUserId")){
    localStorage.removeItem(key)
   }
  }
}
  
</script>

<button onclick="deleteZendeskLocal()">delete local storage key for zendesk</button>
