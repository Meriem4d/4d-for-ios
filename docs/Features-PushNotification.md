---
id: push-notification
title: Push notifications
---

<div markdown="1" class = "tips">

**OBJECTIVES**

Integrate push notification to your 4d for iOS apps

</div>


# What is a push notification?

On a mobile phone, a push notification is an alert message received via an application and that you can open, delete, allow or block. It can be very useful for example to notify your app users that a new version is available.

But what about the architecture to be implemented, in order to integrate this functionality into a mobile application? And what is the process of a push notification, from creation to display on the user's mobile?

# Technical architecture

Here are the different elements needed to create, send and receive a mobile push notification:

![Push notification process](assets/en/push-notification/4D-for-ios-push-notification.png)

# Prerequisites

In order to use the component that is necessary to send push notifications, an AuthKey_XXXX.p8 authentication file from Apple is required.

First, go to Apple developer account page, sign in, then select Certificates, IDs & Profiles.

You will then be able to generate your push certificate and download it.

You can find more information about this process [here]() in the documentation component.

# A component to deal with push notifications

A toolbox component has been developed to help you manage several processes: the 4D Mobile App Server Component.

<div markdown="1" style="text-align: center; margin-top: 20px; margin-bottom: 20px">
<a class="button"
href="https://github.com/4d-for-ios/4D-Mobile-App-Server">4D Mobile App Server Component</a>
</div>

To install this component:

* Create a Components folder next to the 4D database with the app's data.
* Place the 4D Mobile App Server.4dbase component in the newly created Components folder.

And you are done ! 

All you have to do now is following the steps descriped in the [component documentation]() to build your authentication object and send push notifications in just a few click.