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
  The project is an assignment of a coding bootcamp program, with the purpose for students learn about PWA. The goal of this project was to build a text editor that runs in the browser. As a developer I wanted to create notes or code snippets with or without an internet connection so that I can reliably retrieve them for later use. The app is a single-page application that meets the PWA criteria. Additionally, it features a number of data persistence techniques that serve as redundancy in case one of the options is not supported by the browser. The application also functions offline. To build this text editor, I started with an existing application and implement methods for getting and storing data to an IndexedDB database. I used a package called `idb`, which is a lightweight wrapper around the IndexedDB API. It features a number of methods that are useful for storing and retrieving data, and is used by companies like Google and Mozilla.

  ### Installation:
  - Clone the initial code git repository.
  - Navigate on the terminal to the directory text-editor where the code was cloned to.
  - Type "npm i" and "npm start".

  ### Usage:
  GIVEN a the text editor web application that can be found deployed by [clicking here](https://tranquil-harbor-96082-b2b4a591ce66.herokuapp.com/):
  - WHEN I open my application in my editor, THEN I should see a client server folder structure
  - WHEN I run `npm run start` from the root directory, THEN I find that my application should start up the backend and serve the client
  - WHEN I run the text editor application from my terminal, THEN I find that my JavaScript files have been bundled using webpack
  - WHEN I run my webpack plugins, THEN I find that I have a generated HTML file, service worker, and a manifest file
  - WHEN I use next-gen JavaScript in my application, THEN I find that the text editor still functions in the browser without errors
  - WHEN I open the text editor, THEN I find that IndexedDB has immediately created a database storage
  - WHEN I enter content and subsequently click off of the DOM window, THEN I find that the content in the text editor has been saved with IndexedDB
  - WHEN I reopen the text editor after closing it, THEN I find that the content in the text editor has been retrieved from our IndexedDB
  - WHEN I click on the Install button, THEN I download my web application as an icon on my desktop
  - WHEN I load my web application, THEN I should have a registered service worker using workbox
  - WHEN I register a service worker, THEN I should have my static assets pre cached upon loading along with subsequent pages and static assets
  - WHEN I deploy to Heroku, THEN I should have proper build scripts for a webpack application
  - WHEN I access the deployed application, THEN I can type text in the main user interface
  - WHEN I refresh the browser, THEN the text typed remains in the page and is not resetted
  - WHEN I click the "install" button, THEN the application for offline usage opens
  - WHEN the offline application is opened, THEN I see that the typed text remained there
  - WHEN I type new text or remove existing text on the offline application interface, THEN I see that it is also updated on the browser

  ### Contributing
  I have received advice from the UC Berkeley Extension tutors Kyle Vance on pseudocoding and Matthew Calimbas on debugging and testing my code. I also reached out to the [Mozilla Developer](https://developer.mozilla.org/en-US/) webpage and [NPM Docs](https://docs.npmjs.com/) for documentation.

  ### Developer Information:
  - Virginia Freitas
  - GitHub URL: https://github.com/virginiafreitas
  - e-mail address: virginiacdefreitas@gmail.com

  ### License:
  The application is covered under the MIT license.