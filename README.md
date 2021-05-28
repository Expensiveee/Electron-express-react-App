# Electron Express React App Quick Start
Quick starter for an Electron app using an Express server and React

* [Setup](#setup)
* [Start app on `production` mode](#to-start-up-the-app-on-production-mode)
* [Start app on `development` mode](#to-start-up-the-app-on-development-mode)


## Setup
```
$ cd electron-express-react-app
$ npm install --force (optionnal)
$ npm start
or
$ npm run dev
```

## To start-up the app on "development mode"
- Go to the `index.js` file comment the 4th line ONLY, it's used to start the server simultaneously to the app
- Run this command: `npm run dev`

This will start the server using nodemon then the Electron app that will load the specified address that is by default set to `http://localhost:5000`.
You can now make edits on your server/api and see the edits live.
- After a Webpack build on development mode (it will build evey time you edit something on the `app` folder) you need to refresh the app by simply typing `location.reload()` in the devtools or if you are not too lazy add a button for it on the app.

## To start-up the app on "production mode"
- Go to the `index.js` file and uncomment the 4th line if you have it commented.
- Run `npm start`
