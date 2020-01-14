# django-session-tracker

Django app to manage user logins and session

This app is used to track user sessions, and store basic information each time a user visits your site from a new location or device.

The reason for tracking and storing this data is to be able to audit user activity, and to take appropriate action.

* Log user out if accessing site from a new IP
* Track how many devices a user is using
* Monitor for possible fraudulent behaviour
* Alert in event of credential sharing

It's partly inspired by Sqreen - which is a fantastic security application I would highly recommend; also inspired by the big online platforms who are now much more proactive in alerting users to "You have logged in from a different device; if this isn't you, please ..." etc.


Data to track:

* Django user id
* Client IP
* Client user-agent
* Client session key

**GDPR, PII, etc.**

This data is personally identifiable, so must be stored in accordance with data protection laws (e.g. GDPR in the EU), and must be called out in your site privacy policy. Be responsible.
