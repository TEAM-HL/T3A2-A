# T3A2-A - Full Stack App (Part A)

## Hugh & Luke



### Purpose

*Courts* is a simple to use booking application designed for a local tennis court business. It was developed to replace their previous system involving phone bookings and cash envelopes.

### Client Requirements

- Simple, easy to use court booking system with online payment functionality

- Function for admin to communicate events to members

  

### Functionality / Features

There are three user types: Player, Coach and Admin.

### Target audience

The target audience are the players and coaches that use the tennis court as well as the staff who run the court.

### Tech stack (explain what each part of the tech stack is doing)

##### NodeJS 

Mongoose (MongoDB/Atlas) - (Mongo required for MERN app)Our database will be created using MongoDB this is a RDMS that has many advantages. The most important advantage for us is the ability to store any file type and will allow us to store files that are uploaded to our site by different users. A major use of this is with user profiles and their display pictures. Mongo Atlas allows us to store our data in the cloud and connect it to our application. Still needs Mongoosejs (Schema building)

##### React 

(frontend)

##### Express

(backend)

##### Netlify 

(frontend) testing, management system (repo to deployment)

##### Heroku

(backend) handling traffic, resources, management, device compatibility

##### OAuth

This is how our application will handle Authentication, this will provide much needed security for the application and user data that will be handled. OAuth2.0 has improved security with API access using token instead of login data for secure access and protection for user data.

##### Stripe

Will be used to handle payments and refunds for the application, the importance of stripe is that it is easy to use, setup and customise for our application and user experience.

##### ToastUI Calendar

Toast UI is a UI library for JS, we a specifically using the Calendar branch of Toast UI this core to the application as a calendar is needed to keep track of all events and bookings made at the tennis court (not just through the app but in person as well). Multiple features of the application will require access to the calendar or its data to keep information up to date and in sync. The reason for Toast UI specifically is because it is open source (free) and versatile, other software provides the features we need to build this application however some features are locked behind a paywall. Toast UI meets our requirements at no cost.(slight repetition)

##### Multer

This is a middleware we will be using to manage form data and handle the storage of uploaded files to be stored in our database.
(Potential compatibility issues)

### Dataflow Diagram

### Application Architecture Diagram

### User Stories

### Wireframes

### Trello