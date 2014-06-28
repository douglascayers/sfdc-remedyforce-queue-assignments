Easy Queue Member Assignments with Visualforce
==============================================

Simple visualforce page for maintaining queue member assignments and exporting users to Excel.

Overview
========

In the [Remedyforce app](http://www.bmc.com/it-solutions/remedyforce.html), you may setup multiple support groups with assigned IT support staff. These groups are known as [Queues](https://help.salesforce.com/HTViewHelpDoc?id=queues_overview.htm&language=en_US). In the [Salesforce platform](http://www.salesforce.com/platform/overview/), the management of these queues requires elevated platform access, several clicks to add new users to the queue, and [no way of reporting](https://success.salesforce.com/ideaview?id=08730000000BqYaAAK) on who belongs to which queues.

Solution: Visualforce and Apex
==============================

As the System Administrator, I wanted to provide authorized users a way to manage queue assignments without necessarily granting them more platform access than necessary. Secondly, I wanted to provide a basic export to excel of queue members. To accomplish these goals, I created some visualforce pages and apex controller.

Deployment: How To
==================

To simplify deployment of this custom code to your org, you may use the [github deploy tool](http://andyinthecloud.com/2013/09/24/deploy-direct-from-github-to-salesforce/) developed by [Andy Fawcett](https://twitter.com/andyinthecloud).

To deploy in your **sandbox**:
https://githubsfdeploy-sandbox.herokuapp.com/app/githubdeploy/douglascayers/sfdc-remedyforce-queue-assignments

To deploy to **production**:
https://githubsfdeploy.herokuapp.com/app/githubdeploy/douglascayers/sfdc-remedyforce-queue-assignments

*If deploying to production via github tool fails due to tests not being run, you may opt to use Change Sets or Ant Tool or however you normally deploy your code from sandbox to production. Please use your best judgement and due diligence before making any production changes to your org.*
