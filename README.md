
## How-To
### Prerequisits
* OIDC Provider: This client app was tested with https://github.com/dskyberg/oidc-server
* Node: Before you begin, ensure Node is installed.  This has been tested with Node 14.0.4.

Download this repository
````bash
$ git clone https://github.com/dskyberg/oidc-client-spa.git
````

Install the node components
````bash
$ cd oidc-client-spa
$ npm install
````

Run the client
````bash
$ npm start
````
The client app should pop up on your default browser

### Accounts (Users)
Both OAuth2/OIDC clients and user accounts are managed in the OIDC Provider service.
Currently, passwords are not validated.  So, when providing username/password on the
ODIC Provider Sign In page, you can use any value for password.

I test with `bob.smith@example.com`

### Host Error
If you get this error: `Error: getaddrinfo ENOTFOUIND <your hostname>`
Try unsetting your HOST env variable
````bash
$ unset HOST
$ npm start
````


## Developer Info

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `npm run test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
