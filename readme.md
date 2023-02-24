# Web 322 examples

The repo contains examples for the WEB 322 course for Seneca College.

## Contents

* [Requirements](#a0)
* [Cloning the repo](#a1)
* [Running the examples](#a2)
* [Descriptions of the examples](#a3)
* [Submitting corrections or updates](#a4)

<a name="a0"></a>
## Requirements

The examples require some preparation ahead of time to be able to pull them down and run them. The first thing you will need is Git on your computer. Windows users can download [Git for Windows (msysgit)](https://git-for-windows.github.io/) and Mac users will need [Git for Mac](https://git-scm.com/download/mac)

After installing Git you will be able to clone this repository.

You will need to also install other applications to run the examples once the repository is cloned.
* [node.js](https://nodejs.org/en/download/) Get the 64 bit version.
* [Mongo DB](https://www.mongodb.com/download-center?jmp=nav#community) Get the 64 bit version.

<a name="a1"></a>
## Cloning the repo

The command to clone the repo is:
> `git clone https://github.com/sictweb/web322.git`.

You will want to already be in the folder where you want the repo to be cloned and stored. A good place is c:\gitrepos on windows or /gitrepos on mac. A gitrepos folder right in your root of your main drive. You can put it anywhere you want though.

Important Note: If you run the 'git clone' command from within an open folder Visual Studio Code, you will need to close the current folder and open the newly cloned 'examples' folder before you start working.

<a name="a2"></a>
## Running the examples

One you have cloned the repo you will want to make sure you are in the "Code Examples" folder and you can set up the examples.

The main step is to run npm install in the repo to install all the packages that the examples are dependant on.
> `npm install`

The week 8 example requires MongoDB to be running as well. See the class notes for instructions on that.

When you want to deploy one of the examples, you will need to edit the package.json file for the `start` property under scripts. Change the command to the example you want to run.

For example, to run the week 2 example, make the following changes in package.json:
```
"scripts": {
  "start": "node week2.js"
},
```
<a name="a3"></a>
## Descriptions of the examples

* hello.js - A basic hello world example
* week2.js - A basic hello world using Express.js
* week3.js - A set of functions that can be run to demonstrate different JavaScript features
* week4.js - A more detailed Express.js example with routes and 404 handling
* week5.js - An Express.js app that handles file uploading
* week6.js - An Express.js app that uses the handlebars templating library
* week7.js - An Express.js demonstrating a connection to PostgreSQL database using Sequelize
* week8.js - An Express.js photo book app that connects to MongoDB and handles saving pictures
* week9.js - An Express.js REST API and test client (HTML / AJAX)
* week10.js - An Express.js app with client sessions and basic logins
* week11.js - An Express.js app that serves up a "home" view, containing jQuery and Bootstrap examples
* week12.js - A more advanced Express.js app with secure HTTPS logins and client sessions

<a name="a4"></a>
## Submitting corrections or updates

You can submit a correction or update to the code if you find it is necessary. Examples are bug fixes, package updates, readme.md fixes, etc.

Speak to your professor about forking the repo, creating a patch, and submitting a pull request for the changes. You may need permission to create an issue or pull request on this repository.