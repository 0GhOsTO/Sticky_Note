# Sticky_Note

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
1. [Schema](#Schema)
2. [Developer Comments](#Developer-Comments) 

## Overview
### Description: 


### App Evaluation
- **Category:** 
- **Mobile:** 
- **Story:** 
- **Market:** 
- **Habit:** 
- **Scope:** 
## Product Spec
### 1. User Stories (Required and Optional)

**Required Must-have Stories**
- Create:   
- Read: 
- Update: 
- Delete:

**Optional Nice-to-have Stories**
- 
- 

# Underneath is an Example(Need to Be Edited)

### 2. Screen Archetypes
1. Login
2. Register
3. Home (Tab Layout)
4. Edit/Compose (Fragment)
5. Chat/Friend (Fragment)
6. ...

### 3. Navigation

**Tab Navigation** (Tab to Screen)
- Search
- Setting
- Report
- Feedback
- ...

**Flow Navigation** (Screen to Screen)
- Login/Register
- Home with Professional/Social Event
- Profile
- Compose Event 
- Setting
- Report
- Feedback
- ...

## Wireframes
### Design (Figma)
https://www.figma.com/file/Op5T6MotwUd4ZTqTv5OCoz/Kotlin-Project?node-id=0%3A1
<img src='https://github.com/Codepath-Android-pod1/Final_Project/blob/master/WireFrame3.png' />
## PowerPoint Walkthrough
https://docs.google.com/presentation/d/1da7IXtV4kkPxpi9mSwFok32b2ZYULYGRZ6Ag0Tb0H2A/edit?usp=sharing
## Video Walkthrough
Briefly shows the current progress of the project.

<img src='https://github.com/Codepath-Android-pod1/Final_Project/blob/master/CP-3.gif' />


## Schema 
### Models
#### Event

| Property(Key) | Type          | Description  |
| ------------- |-------------  | ------------ |
| objectId      | String        | Unique id for the event |
| user          | String        | Event organizer |
| title     | String            | Name of the event|
| description   | String        | Description of the event|
| location      | GeoPoint      | Latitude and longitude values of the event|
| locationName      | String    | Google Maps name of event location|
| date          | Date          | Date and start time of the event|

#### User
| Property(Key) | Type          | Description  |
| ------------- |-------------  | ------------ |
| objectId      | String        | Unique id for the user |
| username      | String        | username from registering |
| email         | String        | email of the user|
| name          | String        | set by user after registering |
| phonenum      | String        | phone number of the user|

### Networking
#### List of network requests by screen
 - Home Feed Screen
    - (Read/GET) Query events based on filters
 - Organizer List Feed Screen
    - (Read/GET) Query list of Organizers
 - Chat Feed Screen
    - (Read/GET) Query logged in user Chat objects
    - (Create/POST) Send message
 - Create Event Feed Screen  
    - (Create/POST) Create a new event object
 - Create Profile
    - (Create/POST) Create a new user(objectId) with detail included
 - Display Profile
    - (Read/GET) Query details of the user(objectId) and display and profile
 - Remove Profile
    - (Delete) Delete the user(objectId) with detail permanently

#### Existing API Endpoints
##### Ticketmaster Discovery API
- Base URL - [https://app.ticketmaster.com/discovery/v2/](https://developer.ticketmaster.com/products-and-docs/apis/discovery-api/v2/)

 HTTP Verb | Endpoint | Description
 ----------|----------|------------
  `GET`    | /events.json?apikey={apikey}&{params} | gets all events (relevant parameters include `keyword`, `geoPoint`, `postalCode`, `radius`, `unit`, etc)
  
#### Dependencies
- Material Design
- Glide
- Parse
- Retrofit
- GeoFire
- Google Play Location
- EasyPermissions
 
## Developer Comments
