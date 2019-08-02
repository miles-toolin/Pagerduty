# Pagerduty Technical Exercise

1. Create a PagerDuty trial

2. Account Setup

	a. Add five users to the account via the Web UI

	![Users Added Via UI](https://i.imgur.com/1eXyoE3.png)

	b. Create an account level V2 API Key via the Web UI

	![API Key Created](https://i.imgur.com/BH8XBDO.png)

	c. Create a Team using the PagerDuty API

		Script: custom_TeamCreation.curl

	![Team Created Using API](https://i.imgur.com/k4CzBlP.png)


	d. Create a simple On Call Schedule with multiple users via the Web UI

	![Schedule Created](https://i.imgur.com/2Qy6Ms4.png)

	e. Create an Escalation Policy including at least one Schedule via the API

		Script: custom_PolicyCreate.curl

	![Policy Created](https://i.imgur.com/AMcpmJF.png)

	f. Create at least one new Service utilizing the above Escalation Policy via the API

		Script: custom_ServiceCreate.curl

	![Service Create](https://i.imgur.com/LF9348J.png)

	g. Configure the new Service for Time based Alert Grouping via the Web UI

	![Time Based Alerting](https://i.imgur.com/CScqBUs.png)

	h. Setup multiple contact methods via the Web UI

	![Added Multiple Contact Methods](https://i.imgur.com/fBLtVRz.png)

	i. Install the PagerDuty Mobile application on your phone and add that Mobile application as a contact method for your user in the Web UI

	![Pagerduty Installed on Phone](https://i.imgur.com/2nzYUbQ.png) ![Pagerduty App logged in](https://i.imgur.com/Xo2peVM.png) ![Added AS contact Method](https://i.imgur.com/1kRpEio.png)

	j. Add multiple High and Low Urgency Notification Rules to your user profile via the Web UI

![Multiple High and Low Notifications](https://i.imgur.com/4zceAr6.png)


# Incident Response Workflow

3. Incident Response Workflow

	a. Send an Event to PagerDuty using the API

		Script: custom_EventCreate.curl

	![Event Sent via API and Alert triggered](https://i.imgur.com/aTWPsTX.png) 

Call received on phone as soon as POST API Call was made.

![Alert Received on Phone](https://i.imgur.com/PG8rpvZ.png)

b. Trigger an incident using the API

		Script: custom_EventCreate.curl

![Event Sent via API and Alert triggered](https://i.imgur.com/aTWPsTX.png)

c. Acknowledge the incident via the Mobile Application

![Ack event via mobile App](https://i.imgur.com/84vrt4n.png)

d. Using the Response Mobilizer in either the Web UI or Mobile App, add multiple users to the incident

![Added multiple users](https://i.imgur.com/y6pvZTY.png)

e. Using the Subscriber Notification capability, add multiple stakeholder users to the incident via the Web UI

![Added multiple users](https://i.imgur.com/y6pvZTY.png)

f. Add some Notes to the incident through the Web UI or Mobile App

Added Notes via the Web UI

![Adding Test notes](https://i.imgur.com/FxphIiD.png)

g. Resolve the incident via the Mobile App

No more Incidents as resolved using Mobile App

![No more Events as all are resolved](https://i.imgur.com/LKkKJcA.png)

h. Using the API, return a list of the log entries for the incident created in the steps above


