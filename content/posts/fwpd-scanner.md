---
title: FWPD Scanner
date: 2023-11-18T22:03:09-04:00
summary: Local police activity iOS app in Swift/SwiftUI
description: Local police activity iOS app in Swift/SwiftUI
tags: ['Swift', 'SwiftUI', 'Python', 'Firebase', 'Firestore', 'Cloud Functions']
author: Kyle Kincer
toc: false
readTime: true
autonumber: false
---
### Local police activity monitoring for iOS
FWPD Scanner brings Fort Wayne, Indiana's police activity log to your iOS device with compelling features like maps, location-based notifications, commenting and social integrations, filtering, and more.

The app is built with SwiftUI and uses Firebase for authentication, Firestore for data storage, and Cloud Functions for server-side logic.

### Links
- [App Store](https://apps.apple.com/tt/app/fwpd-scanner/id1605283140)
- [GitHub](https://github.com/KyleKincer/FWPD-Scanner)

### Screenshots
![Screenshot 1](/images/Scanner-screenshot1.png)

## Features
### Maps
The app uses Apple Maps to display the location of each incident in relation to the user's current location. 

![Screenshot 3](/images/Scanner-screenshot3.png)

### Location-based notifications
Users can set up notifications to be alerted when an incident occurs within a certain distance of their current location, or when an incident of a certain type occurs anywhere. 

![Screenshot 5](/images/Scanner-screenshot5.png)

### Commenting and social integrations
Users can create an account or sign in with Google to comment on incidents and view other users' comments and profiles.

![Screenshot 2](/images/Scanner-screenshot2.png)
![Screenshot 4](/images/Scanner-screenshot4.png)

### Filtering
Users can filter incidents by type, date, and distance from their location.

![Screenshot 6](/images/Scanner-screenshot6.jpeg)

## Implementation
### Scraper
The app uses a Python script to scrape the Fort Wayne Police Department's activity log and post the data to Firestore. The script runs on a schedule using Cloud Functions.

### Firestore
The app uses Firestore to store all data, including user accounts, incidents, and comments.

### Cloud Messaging
The app uses Cloud Messaging to send notifications to users when incidents occur that they are subscribed to.

### SwiftUI
The iOS app is built entirely with SwiftUI. 
