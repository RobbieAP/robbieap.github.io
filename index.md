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

<script>
let delete_cookie = function(name) {
    document.cookie = name +'=; Path=/; Expires=Thu, 01 Jan 1970 00:00:01 GMT;';
	console.log("Deleted ", name, "cookie");
};
</script>


# Robs ap-widget-tester

Note: Most of the links will contain code to delete the set cookies so appearing on each click is expected behaviour
Some of these links will automatically clear cookies, most are probalby turned off if they don't work due to running out of credits


---
## Remove Cookies

* <button onclick="delete_cookie('ap3c')">Delete ap3c Cookie</button> <--- will be set each time no point
* <button onclick="delete_cookie('ap3converted')">Delete ap3converted Cookie</button>
* <button onclick="delete_cookie('ap3dm')">Delete ap3dm Cookie</button>
* <button onclick="delete_cookie('ap3sess')">Delete ap3sess Cookie</button>


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

<span class="TestLinkClass">A span of text</span>
<h4 class="TestLinkClass">A Text heading of text h4</h4>
<p class="TestLinkClass">A paragraph of text, I have used this as an example for a widget being able to click on a paragraph of text that contains a .class. Ideally what should happen is if the widget that includes the .TestLinkClass is enabled it should popup based on its other conditions. </p>

<svg height="32" aria-hidden="true" viewBox="0 0 16 16" version="1.1" width="32" data-view-component="true" class="octicon octicon-mark-github v-align-middle TestLinkClass">
    <path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path>
</svg>


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


### Capture Forms
* [All Mandatory](form/allMandatory.md)
* [Mandatory Multiselect Embedded form](form/mandatoryMultiSelect.md)
* [Popup with mandatory multi select form](form/popupWithMandatoryMultiSelectForm.md)

* [Notification capture until known](notification/untilKnown.md)
### Bar - Built from Scratch

* [Bar on Load](bar/onLoad.md)
* [Bar on timer](bar/onTimer.md)
* [Bar on Exit](bar/onExit.md)
* [Bar on Scroll](bar/onScroll.md)

### Banner - Built from Scratch

* [Banner on Load](banner/onLoad.md)
* [Banner on timer](banner/onTimer.md)
* [Banner on Exit](banner/onExit.md)
* [Banner on Scroll](banner/onScroll.md)

### Popup - Built from Scratch 

* [Popup on Load](popup/onLoad.md)
* [Popup on Schedule](popup/onSchedule.md)
* [Popup on timer](popup/onTimer.md)
* [Popup on Exit](popup/onExit.md)
* [Popup on Scroll](popup/onScroll.md)

### Notification - Built from Scratch 

* [Notification on Load](notification/onLoad.md)
* [Notification on timer](notification/onTimer.md)
* [Notification on Exit](notification/onExit.md)
* [Notification on Scroll](notification/onScroll.md)

### Takeover - Built from Scratch 

* [Takeover on Load](takeover/onLoad.md)
* [Takeover on timer](takeover/onTimer.md)
* [Takeover on Exit](takeover/onExit.md)
* [Takeover on Scroll](takeover/onScroll.md)

### Spinner - Built from Scratch 

* [Spinner on Load](spin/onLoad.md)
* [Spinner on timer](spin/onTimer.md)
* [Spinner on Exit](spin/onExit.md)
* [Spinner on Scroll](spin/onScroll.md)

### Prompt - Built from scratch

* [Prompt on Load - with push notification](prompt/onLoad.md)

### Prebuilt Widgets

* TODO

### TRACKED FORMS



* [Basic Tracked Form - duplicate different url](trackedform/basictrackedform2.md)
* [Tracked Form with all inputs](trackedform/primarytrackedform.md)
* [Two forms on page - Tracked Form](trackedform/twoforms.md)
* [Unique Tracked Form](trackedform/uniqueform.md)
* [Another basic tracked Form](trackedform/basictrackedform3.md)
* [A basic tracked Form that redirects on submit](trackedform/tfredirected.md)
* [Form that also has org fields](trackedform/tfuserwithorgfields.md)
* [Form created on a provider - todo not implemented](trackedform/tfproviderform.md)
* [Form created on mailchimp](trackedform/tfmailchimp.md)
* [Form using tracking code robs sandbox](trackedform/tfrobssandbox.md)
* [Check random input robs sandbox](trackedform/tfrandominput.md)
* [TF basic on custom dom](trackedform/basictrackedformcustomdom.md)
* [Basic Tracked Form - on robs auto instance](trackedform/basictrackrobsauto.md)
* [TF with hidden fields](trackedform/tfhiddenfields.md)
#### Not expected to work - These are for testing
* [A form with no actual fields](trackedform/zerofieldform.md)
* [Blank page with only a capture script no form for testing](trackedform/capturenoform.md)
* [Basic Tracked Form with no script](trackedform/basictrackedformnoscript.md)
* [Basic Tracked Form that has no form element](trackedform/basictrackedformnoformelement.md)
* [Basic Tracked Form with no ids on elements](trackedform/basictrackedformnoids.md)
* [Basic Tracked Form with no labels but has ids](trackedform/basictrackedformnolabels.md)
* [Basic Tracked Form with no labels and no ids](trackedform/tfnoidentifiers.md)
* [Basic Tracked Form with only name attribute](trackedform/tfjustname.md)
* [Basic Tracked Form with no unique fields e.g email phone](trackedform/tfnounique.md)
* [Basic Tracked Form with script from a different account](trackedform/tfdiffaccountscript.md)
* [Tracked form that has org fields](trackedform/tforgfields.md)


#### Quick Start

* [Blog Subscribe url filename contains blg ](prebuilt/blg.md)
* [Blog Subscribe url path contains blog](blog/subscribe.md)
* [Covid 19 Bar](prebuilt/covid.md)
* [Subscription Notification url contains blog](blog/subscriptionNotification.md)
* [Subscribe Bar](prebuilt/subscribeBar.md)
* [Subscribe Newsletter](prebuilt/subscribeNewsletter.md)

Disabled account not setup
* [SMS Embeddable Form](prebuilt/smsEmbeddableForm.md)
* [SMS Notification](prebuilt/smsNotification.md)
* [SMS Popup](prebuilt/smsPopup.md)

#### Feedback & Surveys

* [Customer Satisfaciton Survey](prebuilt/customerSatisfactionSurvey.md)
* [Customer Satisfaciton Survey Custom](prebuilt/customerSatisfactionSurveyCustom.md)
* [Is Content Helpful?](prebuilt/isContentHelpful.md) 

### Zendesk Stuff

* [Zendesk Chat Widget](zendesk/webWidget.md)

### Custom FE Activity

* [Custom FE Activity Page](activity/frontendactivity.md)
* [Custom FE Activity Page (Sandbox may not work)](activity/frontendactivity2.md)

### Embedded Form - 
* [An embedded form](embedded/embeddedform.md);
* [An embedded form with all fields](embedded/efallfields.md);


