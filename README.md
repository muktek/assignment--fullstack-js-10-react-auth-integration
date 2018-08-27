# Full Stack JS Project - React API Integration
**`fullstack-js-09--react-api-integration`**


## Context
You are going to build a full stack web application with node.js + React. In order to become familiar with how a node project works, you will be responsible for configuring the  initial major components of the project.  

- express server
- application routes
- views
- api layer
  - data access
  - data models + relations (ORM)
  - RESTful routes
- authentication
  - initial configuration
  - application integration
  - protected routes
- React
  - initial configuration
  - application api integration
  - **application auth integration** [this assignment]
  - application api integration w/ protected routes

## The Assignment
Create the React components that allow a user to register, login, and logout. When a user logs in, they should

###  Overview

For this assignment you will need to configure the React components to connect to the backend authentication. You will need

###  Requirements

+ Install react-notification-system as project dependency

  `npm install --save react-notification-system`

+ Configure `RegisterForm.js` so that user can register a new account

  + Successful authentication should: route the user to the `/login`

  + Failed authentication should: show a react-notification-system error

+ Configure `LoginForm.js` so that user can authenticate.

   + Successful authentication should: route the user to the `/dashboard`

   + Failed authentication should: show a react-notification-system error message

   + Update the `App` component's state with the authenticated user returned from the POST query to `/auth/login`

+ Configure `App.js` component to check the `/auth/current` route for an authenticated user's session when the app initializes.
  + Pass global app state to `Nav` component and the `Dashboard` components.

+ Configure `Nav.js` component

  + If there is an authenticated user (received as props from `App` component): the navbar should create `NavLink` to the *Dashboard* and a *Logout* button
    - The *Dashboard* button allows the user to navigate to the `/dashboard` route
    - The *Logout* button allows the user to send a POST request to `/auth/logout`, then routes the user to login.

  + If there is NO authenticated user: the navbar should create a `NavLink` for _Sign In_ and _Log In_ buttons

  + NOTE: make sure that you configure the `Nav` component with React Router's `withRouter` so that the `Nav` component can receive pass route information.

+ Configure `Dashboard.js` component

  + If there is NO authenticated user, the component should re-route the user to the `/login` route

### Expected Functionality


#### `RegisterForm.js`


#### `LoginForm.js`


#### `Dashboard.js`




## Setup Instructions

In Terminal:

```sh
# (1) navigate to your project--devjobs directory
cd ~/Documents/muktek/assignments/project--devjobs

# (2) Commit your changes from the previous demo
git add .
git commit -m 'committing work from part-09-react-api-integration'


# (3) Merge changes to master
git checkout master
git merge part-09-react-api-integration


# (4) You will work on the part-09-react-api-integration branch for this feature
git checkout -b part-10-react-auth-integration

```
