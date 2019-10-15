Firebase Remote Config Quickstart
==============================

The Firebase Remote Config Android quickstart app demonstrates using Remote
Config to define user-facing text in an Android app.

Introduction
------------

This is a clone of remote config quickstart app. Remote config not behaves according to parameter rules if something changes during cache period.

Getting started
---------------

1. Open app with version 1.0(You can run project with branch master or Version1).
2. Click "Display Version Parameter" Button. You should see "My version is 1.0" coming from remote config settings.
3. Update the app to version 2.0.(You can run project from branch Version2 or just update you version to 2.0 from settings or gradle.)
4. Click "Display Version Parameter" Button. You will see "My version is 1.0" coming from remote config settings. However, this doesn't satisfy remote config rules because cache in client has probably no data about parameter rules.
5. Click "Force Fetch and Display" Button.  Now, you will see "My version is 2.0" coming from remote config settings.

What I thought happening was that remote config cache had all data about parameters and rules. So, after update, "Display Version Parameter" Button should have shown "My version is 2.0" on the screen.


