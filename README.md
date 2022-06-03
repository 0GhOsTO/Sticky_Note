# Sticky_Note

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
1. [Schema](#Schema)
2. [Developer Comments](#Developer-Comments) 

## Overview
### Description: 
Allow users to make a note and put on the screen of the phone as a widget. 


### App Evaluation
- **Category:** Lifestyle
- **Mobile:** Developed for mobile by taking advantage of quick and simple and readable.
- **Story:** Users type the brief or important notes and save on their phone. 
- **Market:** All age groups are targeted. People who need to make a quick notes on the phone.
- **Scope:** Application could explanded to contain more features based on the feedback from the user.


### 2. Screen Archetypes
1. Login(Google Account)
2. Register(Google Account)
3. Home(Tab Layout / 2 Recycler View)
4. Edit/Compose/Save (Fragment)
5. Widget

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
- Make Note 
- Feedback
- Widget

## Wireframes
### Design (Figma)
https://www.figma.com/file/Op5T6MotwUd4ZTqTv5OCoz/Kotlin-Project?node-id=0%3A1
<img src='https://github.com/Codepath-Android-pod1/Final_Project/blob/master/WireFrame3.png' />

## Video Walkthrough 
Briefly shows the current progress of the project.

<img src='https://github.com/Codepath-Android-pod1/Final_Project/blob/master/CP-3.gif' />


## Schema 
### Models
#### Notes
| Property(Key) | Type          | Description  |
| ------------- |-------------  | ------------ |
| objectId      | String        | Unique id for the event |
| title         | String        | Title of the Note |
| details       | String        | Detail of the Note |
| favorite      | boolean       | Marked as important note or not|
| deleted       | boolean       | Deleted note or not|
| calendar      | Date          | Mark the due date of the note and alarm|

#### User / Requirement for Google Account
| Property(Key) | Type          | Description  |
| ------------- |-------------  | ------------ |
| objectId      | String        | |
| username      | String        | |
| email         | String        | |
| name          | String        | |
| phonenum      | String        | |

### Networking
#### List of network requests by screen
 - Home Feed Screen
    - (Read/GET/DELETE) Get the account's note and display on the recycler view.
 - Garbage Note Feed Screen
    - (Read/POST/DELETE) Create a new event object
 
## Developer Comments
