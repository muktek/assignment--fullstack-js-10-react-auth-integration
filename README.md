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
- React
  - initial configuration
  - **application api integration [this assignment]**
  - application auth integration


## The Assignment
For this assignment, we will focus on the application's **React application API integration**.

###  Overview

For this assignment you will need to integrate data from the companies and jobs tables into your React application and render Job and Company components for each record.

You will do this by making a request (using the superagent promise library) to the data exposed from our API at the `/api/jobs` and `/api/companies` endpoints from the `CompanyListings` and `JobListings` components.

`CompanyListings` and `JobListings` components should update their state when the requested data returns from the api.

You will need to map over an array of the returned data to create `Job` components and `Company`.


###  Demo

#### Job Listing Demo

![job listings](demos/job-listing-demo.png)

#### Company Listing Demo

![company listings](demos/company-listing-demo.png)




## Setup Instructions

In Terminal:

```sh
# (1) navigate to your project--devjobs directory
cd ~/Documents/muktek/assignments/project--devjobs

# (2) Commit your changes from the previous demo
git add .
git commit -m 'committing work from part-07-auth-1'

# (3) You will work on the part-08-react-configuration branch for this feature
git checkout -b part-09-react-api-integration

# (4a) Download + Unzip project styles
curl https://raw.githubusercontent.com/muktek/assignment--fullstack-js-09-react-integration/master/style-css.zip > style-css.zip

unzip style-css.zip -d public/css/styles.css

# (4b) Download + Unzip Job, Company, Nav components

curl https://raw.githubusercontent.com/muktek/assignment--fullstack-js-09-react-integration/master/job-company-nav-components.zip > job-company-nav-components.zip

unzip job-company-nav-components.zip -d src/client/js/components/


# (5) Install superagent promise library
npm install --save superagent
```
