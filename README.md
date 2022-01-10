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


# Robs ap-widget-tester

Trialled
* Bar Widget Time delay
* Popup on exit
* Notification on Click Id, Class
* Takeover on Click Class
* Banner 10 Secs



---
### Test Links 

~~~
#TestLinkId
.TestLinkClass
~~~

* <a class="TestLinkClass">This is a link with class</a>
* <a id="TestLinkId">This is a link with id no class</a>
* <a href="" class="TestLinkClass">This is a link with an empty href - reloads page</a>
* <a href="#" class="TestLinkClass">This is a link with an # href</a>
* <a href="#" class="TestLinkClass">This is a link with an #0 href an unused reference</a>
* <a href="#" onclick="return false;" class="TestLinkClass">This is a link with a onclick return false and href = #  </a>
* <a href="javascript:void(0)" class="TestLinkClass"> This is a link with a javascript void(0) tag </a>
* <a href="javascript:{}" class="TestLinkClass"> This is a link with a javascript {} tag </a>
* <a href="http://www.google.com" class="TestLinkClass">This is a regular link to google</a>


### Test Buttons

* <button class="TestLinkClass">A non navigating button with TestLinkClass</button>
---

### Specific Capture Buttons

* <button id="barWidget">Bar widget</button>
* <button id="popupWidget">Popup widget</button>
* <button id="notificationWidget">Notification widget</button>
* <button id="takeoverWidget">Takeover widget</button>
* <button id="bannerWidget">Banner widget</button>
* <button id="spinWidget">Spin widget</button>
