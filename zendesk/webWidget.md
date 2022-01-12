---
title: Zendesk webWidget
layout: template
filename: webWidget.md
--- 


# Zendesk webWidget - no tracking code  but will need to open incognito


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
