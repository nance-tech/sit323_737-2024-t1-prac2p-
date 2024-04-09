# Setting Up Node.js Web Server with Express

Hey there! Welcome to my documentation on setting up a Node.js web server using Express for SIT323. In this guide, I'll walk you through the steps I took to create a simple web server for the course assignment. Let's get started!

## Table of Contents

[Project folder structure]()

[Setting Up Git](#setting-up-git)

[Installing Tools](#installing-tools)

[Creating a Simple Web Server with Express](#creating-a-simple-web-server-with-express)

## Project folder structure

```
.
├── assets
│   ├── css
│   │   └── index.css
│   ├── img
|   |   └── Screenshot.png
│   └── js
├── index.html
├── index.js
├── package.json
├── package-lock.json
└── README.md

```

## Setting Up Git

**1. Git Installation**

First things first, I made sure to have Git installed on my system. If you don't have it yet, you can download it from [here](https://git-scm.com/).

**2. Creating a Git Account**

Next,I created a repository in my existing github account that i will use for this unit.

## Installing Tools

**1. Visual Studio Code Installation**

Next, I installed Visual Studio Code for writing my code. It's a fantastic code editor and you can get it from here. After that, I installed Node.js, which is essential for running JavaScript code outside the browser. You can download it here.

**2. Node.js Installation**

Next, I downloaded and installed the latest version of Node.js from nodejs.org.
To verify the installation, I opened terminal and run node --version, which gave me the version of the installed node version.

## Creating a Simple Web Server with Express

**1. Project Setup**

I opened Visual Studio Code and created a new folder for my project. Then, I opened a terminal in VS Code and navigated to my project folder.

**2. Initialize Project and Install Dependencies:**

Using the terminal, I initialized a new Node.js project by running `npm init -y`. This command creates a package.json file with default settings.

**3. Installing Express**

With the project initialized, I installed Express, the web framework for Node.js, by running `npm install express` in the terminal.

**4. Creating HTML Content**

I created an HTML file named `index.html` in my project folder and added the content I wanted to display on my web page.This file contains the markup for the web page I wanted to display.

**5. Writing Server Code**

Next, I created a JavaScript file named `index.js`. This file contains the code to set up a basic web server using Express and serve the HTML content. I copied the example code provided in the assignment and modified it to suit my needs.

```javascript
    const express = require("express");

    const path = require("path");

    const app = express();

    app.use(express.static("assets"));

    app.get("/", (req, res) => {
    res.sendFile(path.join(\_\_dirname, "/index.html"));
    });

    app.listen(4000, () => {
    console.log("Express server running on http://localhost:4000 🚀");
    });
```

## Run the Server

To start the web server, I ran `npm start` in the terminal. This command executes the JavaScript file containing the server code. With the server up and running, I opened my web browser and navigated to http://localhost:3000 to view my web page.

## Submission

With the project completed and initialized a Git repository in my project folder, I added all the files to the repository using `git add .`, committed the changes using the command `git commit -m "Initial commit"`, and pushed the code to a new repository on GitHub. I named the repository `sit323_737-2024-t1-prac2p`, as per the assignment instructions. Finally I pushed the code to github using the command `git push`.
