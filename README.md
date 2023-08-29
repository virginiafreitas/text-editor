  # PWA: Text Editor

  [![GitHub License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

  ### Table of Content
  * [Description](#description)
  * [Installation](#installation)
  * [Usage](#usage)
  * [Contributing](#contributing)
  * [Developer Information](#developer-information)
  * [License](#license)

  ### Description:
  The project is an assignment of a coding bootcamp program, with the purpose for students learn how to use NoSQL and Mongoose. The application is a social network API where users can interact by creating accounts, sharing their thoughts, adding other users to their friends list, and adding reactions to other users thoughts.

  ### Installation:
  - Clone the initial code git repository.
  - Install Insomnia and MongoDB to the machine if not already installed.
  - Navigate on the terminal to the directory social-network where the code was cloned to.
  - Type "npm i", "node ./seeds/seeds.js" and "npm start".

  ### Usage:
  [Click here](https://drive.google.com/file/d/1pqqa-XCoU99IAJY0qNJvDcsDO7AThHPK/view) to watch a demo on how to use and test the application on Insomnia. 
  - Open Insomnia
  - Select "GET", then type and send "localhost:3002/api/users" to see all the users and "localhost:3002/api/thoughts" to see all the thoughts.
  - Select "POST", then type "localhost:3002/api/users" in the route form and type "{"username": "placeholder","email": "placeholder"}" with your desired placeholders in the JSON form and click "send" to add a new user.
  - Select "PUT", then type "localhost:3002/api/users/:userId" in the route form and type "{"username": "placeholder","email": "placeholder"}" with your desired placeholders in the JSON form and click "send" to replace an existing user.
  - Select "POST", then type "localhost:3002/api/thoughts" in the route form and type "{"thoughtText": "placeholder","username": "placeholder"}" with your desired placeholders in the JSON form and click "send" to add a new thought.
  - Select "PUT", then type "localhost:3002/api/thoughts/:thoughtId" in the route form and type "{"thoughtText": "placeholder","username": "placeholder"}" with your desired placeholders in the JSON form and click "send" to replace an existing thought.
  - Select "POST", then type "localhost:3002/api/users/:userId/friends/:friendId" in the route form and click "send" to add a friend to a user's list of friends.
  - Select "POST", then type "localhost:3002/api/thoughts/:thoughtId/reaction" in the route form and type "{"reactionBody": "placeholder","username": "placeholder"}" with your desired placeholders in the JSON form and click "send" to add a reaction to the thought of a friend.
  - Select "DELETE", then type "localhost:3002/api/thoughts/:thoughtId/reaction/:reactionId" in the route form and click "send" to delete a reaction to the thought of a friend.
  - Select "DELETE", then type "localhost:3002/api/users/:userId/friends/:friendId" in the route form and click "send" to delete a user from another user's friend's list.
  - Select "DELETE", then type "localhost:3002/api/thoughts/:thoughtId" in the route form and click "send" to delete a user's thought'.
  - Select "DELETE", then type "localhost:3002/api/users/:userId" in the route form and click "send" to delete a user's account'.

  ### Contributing
  I have received advice from the UC Berkeley Extension tutors Kyle Vance on pseudocoding and Matthew Calimbas on debugging and testing my code. I also reached out to the [Mozilla Developer](https://developer.mozilla.org/en-US/) webpage and [NPM Docs](https://docs.npmjs.com/) for documentation.

  ### Developer Information:
  - Virginia Freitas
  - GitHub URL: https://github.com/virginiafreitas
  - e-mail address: virginiacdefreitas@gmail.com

  ### License:
  The application is covered under the MIT license.














## Your Task

As you have progressed through this course, you have put together a number of impressive projects that you can show off to potential employers. This project is no exception; in fact, it features some of the most impressive expressions of the concepts you have learned so far.

Your task is to build a text editor that runs in the browser. The app will be a single-page application that meets the PWA criteria. Additionally, it will feature a number of data persistence techniques that serve as redundancy in case one of the options is not supported by the browser. The application will also function offline.

To build this text editor, you will start with an existing application and implement methods for getting and storing data to an IndexedDB database. You will use a package called `idb`, which is a lightweight wrapper around the IndexedDB API. It features a number of methods that are useful for storing and retrieving data, and is used by companies like Google and Mozilla.

You will deploy this full-stack application to Heroku using the [Heroku Deployment Guide on The Full-Stack Blog](https://coding-boot-camp.github.io/full-stack/heroku/heroku-deployment-guide).

**Important**: Make sure your submission includes the `.npmrc` file in this starter code.  This will ensure your application will deploy properly to heroku.

## User Story

```md
AS A developer
I WANT to create notes or code snippets with or without an internet connection
SO THAT I can reliably retrieve them for later use
```

## Acceptance Criteria

```md
GIVEN a text editor web application
WHEN I open my application in my editor
THEN I should see a client server folder structure
WHEN I run `npm run start` from the root directory
THEN I find that my application should start up the backend and serve the client
WHEN I run the text editor application from my terminal
THEN I find that my JavaScript files have been bundled using webpack
WHEN I run my webpack plugins
THEN I find that I have a generated HTML file, service worker, and a manifest file
WHEN I use next-gen JavaScript in my application
THEN I find that the text editor still functions in the browser without errors
WHEN I open the text editor
THEN I find that IndexedDB has immediately created a database storage
WHEN I enter content and subsequently click off of the DOM window
THEN I find that the content in the text editor has been saved with IndexedDB
WHEN I reopen the text editor after closing it
THEN I find that the content in the text editor has been retrieved from our IndexedDB
WHEN I click on the Install button
THEN I download my web application as an icon on my desktop
WHEN I load my web application
THEN I should have a registered service worker using workbox
WHEN I register a service worker
THEN I should have my static assets pre cached upon loading along with subsequent pages and static assets
WHEN I deploy to Heroku
THEN I should have proper build scripts for a webpack application
```

## Mock-Up

The following animation demonstrates the application functionality:

![Demonstration of the finished Module 19 Challenge being used in the browser and then installed.](./Assets/00-demo.gif)

The following image shows the application's `manifest.json` file:

![Demonstration of the finished Module 19 Challenge with a manifest file in the browser.](./Assets/01-manifest.png)

The following image shows the application's registered service worker:

![Demonstration of the finished Module 19 Challenge with a registered service worker in the browser.](./Assets/02-service-worker.png)

The following image shows the application's IndexedDB storage:

![Demonstration of the finished Module 19 Challenge with a IndexedDB storage named 'jate' in the browser.](./Assets/03-idb-storage.png)

## Grading Requirements

> **Note**: If a Challenge assignment submission is marked as “0”, it is considered incomplete and will not count towards your graduation requirements. Examples of incomplete submissions include the following:
>
> * A repository that has no code
>
> * A repository that includes a unique name but nothing else
>
> * A repository that includes only a README file but nothing else
>
> * A repository that only includes starter code

This Challenge is graded based on the following criteria:

### Technical Acceptance Criteria: 40%

* Satisfies all of the above acceptance criteria plus the following:

  * Uses IndexedDB to create an object store and includes both GET and PUT methods

  * The application works without an internet connection

  * Automatically saves content inside the text editor when the DOM window is unfocused

  * Bundled with webpack

  * Create a service worker with workbox that Caches static assets

  * The application should use babel in order to use async / await

  * Application must have a generated `manifest.json` using the `WebpackPwaManifest` plug-in

  * Can be installed as a Progressive Web Application

### Deployment: 32%

* Application deployed to Heroku at live URL with build scripts

* Application loads with no errors

* Application GitHub URL submitted

* GitHub repo contains application code

### Application Quality: 15%

* Application user experience is intuitive and easy to navigate

* Application user interface style is clean and polished

* Application resembles the mock-up functionality provided in the Challenge instructions

### Repository Quality: 13%

* Repository has a unique name

* Repository follows best practices for file structure and naming conventions

* Repository follows best practices for class/id naming conventions, indentation, quality comments, etc.

* Repository contains multiple descriptive commit messages

* Repository contains quality README file with description, screenshot, and link to deployed application

## Review

You are required to submit the following for review:

* The URL of the deployed application

* The URL of the GitHub repository, with a unique name and a README describing the project

- - -
© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.
