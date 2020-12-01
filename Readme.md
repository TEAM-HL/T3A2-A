# ![]()T3A2-A - Full Stack App (Part A)

## Hugh & Luke

----------

### Purpose
***Courts*** is a simple to use booking application designed for a local tennis court business. It was developed to replace their previous system that relied on phone bookings and cash envelopes.

##### Client Requirements

- Simple, easy to use UI 
- online payments
- Ability for coaches to advertise lessons on a member noticeboard
- Admin functions to: 
  - post events on a member noticeboard
  - create, edit and delete any bookings

### Functionality / Features
There are 3 types of user accounts: *Player*, *Coach* and Admin. 

Users must create a profile first before a booking can be made and have the option of uploading a profile picture.

Players can book a court for an allotted time and hire additional tennis gear at checkout. Coaches can do the same as players with the added ability to advertise their coaching services on the member noticeboard.

Admins can create, edit and delete any booking or any post on the virtual noticeboard. 

The homepage for the Player and Coach comprises a tennis court graphic that shows the current and next availability of each court. The Admin has an additional calendar interface to see bookings across days and weeks, as well as events.

### Target audience

The target audience are the players and coaches that use the tennis court as well as the admin staff who run the court.

### Tech stack (explain what each part of the tech stack is doing)

##### [NodeJS](https://nodejs.org/) 
NodeJS is a JavaScript runtime environment that allows JavaScript code to be run on the server. 

##### [ExpressJS](https://expressjs.com/)

ExpressJS is a web framework that runs on top of NodeJS and will be used to handle HTTP requests, middleware and routing.

##### [MongoDB](https://www.mongodb.com/) / [Atlas](https://www.mongodb.com/cloud/atlas) / [Mongoose](https://mongoosejs.com/)

Our database will be created using *MongoDB*, a NoSQL, non-relational database system. The most important advantage for us is the ability to store any file type in a document model and will allow us to store files that are uploaded to our site by different users. The major use case will be user profile display pictures.

*Mongo Atlas* allows us to store our data in the cloud and connect it to our application.

*Mongoose* is an object modelling solution that is used to interface with and create the schema for the Mongo database.

##### [ReactJS](https://reactjs.org/)

ReactJS will be used to create the interactive UI. The interface will automatically update to reflect data changes such as bookings made and court availability.


##### [Netlify](https://www.netlify.com/) 

Netlify will host the ReactJS frontend code and assist with testing from the development to the production stage.

##### [Heroku](https://www.heroku.com/)

Heroku will host the backend code and handle traffic, resources, management and device compatibility.

##### [OAuth](https://oauth.net/)

This is how our application will handle Authentication and will provide much needed security for the application and the user data that will be handled. OAuth 2.0 has improved security with API access using a token instead of login data for secure access and protection for user data.

##### [Stripe](https://stripe.com/au)

Stripe will be used to handle payments and refunds for the application. It is easy to use, setup and customise for our application and user experience.

##### [ToastUI Calendar](https://ui.toast.com/tui-calendar)

ToastUI is a JavaScript user interface library. We will be specifically using the Calendar features for the admin user to keep track of all events and bookings. Multiple features of the application will require access to the calendar or its data to keep information up to date and in sync. The main benefit of choosing this particular library is that it is open source (free) and versatile enough for our use case. Other options we considered provided the necessary features but required a paid subscription which wasn't an option for us.

##### [Multer](https://github.com/expressjs/multer)

This is a middleware we will be using to manage form data and handle the storage of uploaded files to be stored in our database.
(Potential compatibility issues)

### Context / Dataflow Diagrams

The below *context diagram* gives a birds-eye view of the inputs and outputs that are sent and received between external entities, related to the core purpose of the application. 

![CD-input&output](docs/diagrams/ContextDiagram.png)

The below *Dataflow Diagram* illustrates how/what data is passed around the application from the perspective of a Player or Coach.

![DFD-Player & coach](docs/diagrams/DataFlowDiagram_player_coach.png)

The below *Dataflow Diagram* illustrates the additional dataflows that exist for an Admin user.

![DFD-Admin](docs/diagrams/DataFlowDiagram_admin.png)

### Application Architecture Diagram

![AAD](docs/diagrams/MERN-Architecture-Diagram.png)

### 

### User Stories

| AS A..     | I WANT TO..                                                  | SO THAT..                                                    |
| ---------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **Player** | Create a profile and upload a profile picture                |                                                              |
| **Player** | Create a court booking                                       |                                                              |
| **Player** | Hire additional gear as part of court booking                | only one transaction is required                             |
|            | *include racquet & ball canister options*                    |                                                              |
| **Player** | Send a message to the admin                                  | I can have any query or problem resolved                     |
| **Player** | View my current bookings                                     |                                                              |
| **Player** | View a current booking                                       |                                                              |
| **Player** | Edit or Delete a current booking                             |                                                              |
| **Coach**  | Create a profile and upload a profile picture                |                                                              |
| **Coach**  | Create a court booking                                       |                                                              |
| **Coach**  | Hire additional gear as part of court booking                | only one transaction is required                             |
|            | *include racquet, ball canister & ball hopper options*       |                                                              |
| **Coach**  | Send a message to the admin for assistance                   | I can have any query or problem resolved                     |
| **Coach**  | Post advertisement for lessons on events page                | student players can contact me                               |
| **Admin**  | View all court bookings on a single calendar                 | I can visually assess current court bookings and locate any upcoming bookings |
| **Admin**  | Create, Edit and Delete any event post                       |                                                              |
| **Admin**  | Create, Edit and Delete any court booking                    |                                                              |
| **Admin**  | Create, Edit and Delete any user player or coach user profile |                                                              |
| **Admin**  | View all player and coach user profiles                      | I can easily locate a user                                   |



### Wireframes

### Trello