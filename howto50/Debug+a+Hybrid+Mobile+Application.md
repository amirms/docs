---
title: "Debug a Hybrid Mobile Application"
category: "howto50"
space: "Mendix 5 How-to's"
---
# Debug a Hybrid Mobile Application

<table><thead><tr><th class="confluenceTh">Mendix Version</th><th class="confluenceTh">Create Date</th><th colspan="1" class="confluenceTh">Modified Date</th></tr></thead><tbody><tr><td class="confluenceTd">5.17</td><td class="confluenceTd">Jun 22, 2015 16:49</td><td colspan="1" class="confluenceTd">Apr 11, 2016 08:33</td></tr></tbody></table>

This how-to explains the steps involved in debugging a Mendix application that is running in the Mendix Developer App on your mobile phone.

**After completing this how-to you will know:**

*   How to debug a mobile application

## 1. Preparation

Before you can start with this how-to, make sure you have completed the following prerequisites.

*   Install [weinre](https://people.apache.org/~pmuellr/weinre/docs/latest/)
*   Mendix Developer App (v1.1 or later) installed on your mobile device. You can find it in your platform's appstore. 

## 2\. Start weinre

From your console, start weinre with the following parameters:

weinre --boundHost 1.2.3.4 --httpPort 9090

where 1.2.3.4 is your local IP. This will most probably match the address that you see in the History of your Mendix Developer App. You can change 9090 to a different port, as long as it doesn't clash with your application's port, which is usually 8080. 

## 3\. Connect your Mendix Developer App

Click the settings icon (top right, see screenshot) to configure your debugger. On the configure screen, fill in the same settings that you used to start weinre. This should be [http://1.2.3.4:9090](http://1.2.3.4:9090) (where 1.2.3.4 is your local IP)

You can now surf to the **same** address from your local browser to start the debugging session.

![](attachments/14090647/14385197.png)

## 4\. Related content

*   [Finding the Root Cause of Runtime Errors](/howto50/Finding+the+Root+Cause+of+Runtime+Errors)
*   [Clearing Warning Messages in Mendix](/howto50/Clearing+Warning+Messages+in+Mendix)
*   [Finding the Root Cause of Runtime Errors](/howto6/Finding+the+Root+Cause+of+Runtime+Errors)
*   [Clearing Warning Messages in Mendix](/howto6/Clearing+Warning+Messages+in+Mendix)
*   [Testing web services using SoapUI](/howto6/Testing+web+services+using+SoapUI)
*   [Testing web services using SoapUI](/howto50/Testing+web+services+using+SoapUI)
*   [Debugging Microflows](/howto50/Debugging+Microflows)
*   [Common Mendix SSO Errors](/howto50/Common+Mendix+SSO+Errors)
*   [Monitoring Mendix using JMX](/howto50/Monitoring+Mendix+using+JMX)
*   [Debugging Java Actions](/howto50/Debugging+Java+Actions)
