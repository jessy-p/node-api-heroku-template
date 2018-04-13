# Node API Template for Heroku

This template can be used for a simple node api project that can be run locally and also deployed on heroku

## Getting Started

### Prerequisites

Node
npm
Heroku CLI

### Installing

This is how to get the code up and running for your project

Get it locally & rename

```
1. git clone https://github.com/jescrafts/node-api-heroku-template.git
2. cd node-api-heroku-template
3. Rename folder and rename the project in package.json
4. npm install
```

Test it on local

```
5. heroku local web
6. Test http://localhost:5000/ and http://localhost/api/self
```

Deploy to heroku

```
5. git add .
6. git commit -m "Initial Commit"
7. heroku create <heroku-app-name> (might prompt for heroku login)
8. git push heroku master
6. heroku open
```

## Using the template

You can use this template to create your application quickly

### Keys management

The template supports management of keys seperately for production vs development environments. For any service that requires secure credentials, create the development and production credentials. 
. 

```
1. Update the development keys in config/dev.js
2. git rm config/dev.js & commit
3. Update .gitignore file to not commit config/dev.js
3. Login to heroku dashboard to set up the production Key. Update config/prod.js to fetch the keys
4. Test locally vs deployed to heroku versions
```

### API

Modify routes.js to add the api routes
Modify models to add new models and support functionality required for your application

