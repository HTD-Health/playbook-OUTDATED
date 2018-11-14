### Introduction

This readme describes the protocols explaining how to release a beta version of mobile apps to beta users

There are a number of scenarios when releasing a beta version of an app is not a simple act of sending an installation link to beta users but requires careful preparation. It might be that the realease affects a large amount of users and presents a potential risk of damaging HTD reputation. Therefore the process of releasing a beta version should be approached carefully.

### Why this is very important

Imagine the following scenario. You have been building a mobile app for patients that has a deadly form of cancer. You are working with two doctors who run a hospital department and treat tens of such patients there. At some point the team decides to to gather a focus group of such patients to ask them for feedback. To get the best feedback possible the doctors ask patients to come to the hospital specially to take part in a focus group. Now, because of last minute bugfixes the team did not invite patients to the beta app via good old Apple Test Flight tools and instead they relied on continuouns builds done by a third-party CI service. It turned out then that the third-party service is down for a few hours. The focus group patients had waited 2 hours in the hospital to get the installation link before the doctors decided that the process presents too much risk for cancer patients and they were taken back home. Consequently the focus group was cancelled. HTD has never again been given an opportunity to work with this hospital.

### Common mistakes

- Sending out an app build built from _master_ or _develop_ or feature branch. Beta releases (not a _release_ word) should be cut from _master_ or _develop_ branch and tagged. Then tested. Same for the backend. There should be a separate backend instance used for beta testing and the deployment there should not be done from either from _develop_ or _master_ branch
- Inviting beta testers to install the app just before a focus group happens. It's better to do it early so that you can learn about potential issues installing the app
- Relying on third-party services instead of on good old Apple Test Flight and _external testers_ there.
