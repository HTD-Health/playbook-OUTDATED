### Introduction

This readme describes the protocols explaining how to release a beta version of mobile apps to beta users in _high risk risk cases_ i.e. when a lot of external users are involved. When releasing an app within the Scrum team the process can be lean and more relaxed, even if the Scrum team involves people from the client company.

There are a number of scenarios when releasing a beta version of an app is not a simple act of sending an installation link to beta users but requires careful preparation. It might be that the realease affects a large amount of users and presents a potential risk of damaging HTD reputation. Therefore in such cases the process of releasing a beta version should be approached carefully.

### Why this might be very important

Imagine the following scenario. 

You have been building a mobile app for patients that has a deadly form of cancer. You are working with two doctors who run a hospital department and treat tens of such patients there. At some point the team decides to to gather a focus group of such patients to ask them for feedback. To get the best feedback possible the doctors ask patients to come to the hospital specially to take part in a focus group. Now, because of last minute bugfixes the team did not invite patients to the beta app via good old Apple Test Flight tools and instead they relied on continuouns builds done by a third-party CI service. It turned out then that the third-party service is down for a few hours. The focus group patients had waited 2 hours in the hospital to get the installation link before the doctors decided that the process presents too much risk for cancer patients and they were taken back home. Consequently the focus group was cancelled. HTD has never again been given an opportunity to work with this hospital. The content marketing campaign and conference talks planned were needed to be cancelled, too because the doctors decided to not provide excellent references to HTD.

### Be paranoid

Murphy's law states that "whatever can go wrong, will go wrong." Be paranoid. If you rely on a third-party service, assume it might be down just at the time when you need it most. Think what can go wrong and proactively limit the amount of weak points.

### The checklist

- [ ] Make sure the whole team is aware of a need for releasing a beta version of the app. Explain who will be the users, when the relese process will happen, why we need a beta version and what features are to be included.
- [ ] When the time comes, create a separate branch or tag from the main line of the code (typically _develop_ or _master_ branch). Do it both for the backend and for the frontend.
- [ ] Test, fix bugs, iterate. Incorporate the bugfixes back to the main line of the codebase. Note "Only bugfixes!" part in [this diagram](https://datasift.github.io/gitflow/GitFlowHotfixBranch.png).
- [ ] Make sure the key developers are online at the time of release and available to jump in when needed. Even though you prepared for the release, there might still be a need for an urgent hot fix or restarting a server.
- [ ] Make sure the team knows the process of releasing a potential bugfix including: where to push the code, how to create a build or trigger a CI, how to deploy the fix etc.
- [ ] Make sure the team knows how to monitor the app and the backend. This includes making sure the team has access to real time logs of the app and the backend
- [ ] Make sure the team know how to rollback a bugfix efficiently. This includes rollbacking a database change. Prep for this so that you can act calmly and professionally when things go wrong at 3am.

### Common mistakes

- Sending out an app build built from _master_ or _develop_ or feature branch. Beta releases (not a _release_ word) should be cut from _master_ or _develop_ branch and tagged. Then tested. Same for the backend. There should be a separate backend instance used for beta testing and the deployment there should not be done from either from _develop_ or _master_ branch
- Inviting beta testers to install the app just before a focus group happens. It's better to do it early so that you can learn about potential issues installing the app
- Relying on third-party services instead of on good old Apple Test Flight and _external testers_ there.
