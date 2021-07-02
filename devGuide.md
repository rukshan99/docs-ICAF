# Conference Management Tool for ICAF
**This is the developer guide for the Conference Management Tool for "International Conference on Application Frameworks" also known as [ICAF](https://icaf-sliit.herokuapp.com/).** 

**To get a more technical idea of the system use our [technical report](reports/technicalReport.pdf ':ignore'). Checkout our [user guide](userGuide.md) if you're new here.**
<hr />

## Rest API

The backend of the conference management tool is a RESTful API running JSON based web services, and implemented with Node.js and Express.js

### Getting started

#### Cloning

First, the project is needed to be cloned to your local space.

`git clone https://github.com/rukshan99/api-ICAF`

Since the API uses MongoDB atlas as the database, [a cluster should be created](https://docs.atlas.mongodb.com/getting-started/) and the connection string sould be added to a `.env` file in the project root.

![](images/dotenv.png ':size=1000')

#### Installing packages

Install the required dependencies needed in both development and production as defined in the `package.json`.

Run `npm install` in your CLI.

#### Development mode

You can test the API endpoints using an API tester like [Postman](https://www.postman.com/). To do that, run `npm start` in your CLI to run the server in development mode.

Server will restart automatically if you do any edits.

#### Testing

API testing is handled using Jest framework and MongoDB-memory-saver package. Jest provides 
methods to create, organize and run the tests. The mongodb-memory server creates a cluster which 
only exists in the device’s main memory and is not physically stored to disk. Therefore, once the 
application terminates, the database instance will no longer exist.

To run the test cases use `npm test` in your terminal.

<hr />

## React App

The frontend of the system is based on React related technologies and it consumes the JSON based service endpoints of the REST API.

### Getting started

#### Cloning

First, the project is needed to be cloned to your local space.

`git clone https://github.com/rukshan99/app-ICAF`

#### Installing packages

Install the required dependencies needed in both development and production as defined in the `package.json`.

Run `npm install` in your CLI.

#### Development mode

To run the app in the development mode use `npm start` in your CLI.
Open http://localhost:3000 to view it in the browser.

The page will reload if you make edits.
You will also see any lint errors in the console.

#### Testing

React component testing and snapshot testing was done using Jest and Enzyme.

Run `npm test` in the CLI to launch the test runner in the interactive watch mode.

#### Preparing for deployment

Run `npm run build` in your CLI to build the app for production to the build folder.
It correctly bundles React in production mode and optimizes the build for the best performance.

<hr />

# Contribution guidelines

* Before starting development, create a branch.
  * `git checkout -b <FTR|ENH|BUG-name>`
* Stage and commit changes to the local repo.
  * `git add .`
  * `git commit -m "<commit message>"`
* Push to the new remote branch.
  * `git push -u origin <FTR|ENH|BUG-name>` (for first push to origin)
* Create the pull request
  * Add a proper descriptive title.
  * Use description box to explain the changes proposed in the pull request and affecting parts of the system.

