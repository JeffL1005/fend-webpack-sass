# Webbpack Express Example App

The goal of this repo is be an example of a basic but functional app built on Express and Webpack.

If you want to follow along, start from branch 0-initial-setup. Each branch in this project is a step along the path to creating a fully functional webpack setup. In each branch, there will be a documentation file that lists out the steps taken in that branch (each step is also roughly a git commit if you look at the history) which you can use as a checklist when setting up your own projects.

## What we will cover

We will cover:

- Webpack entry point
- Webpack output and dist folder
- Webpack Loaders
- Webpack Plugins
- Webpack Mode
- Tools for convenient Webpack development

## Get Up and Running

Fork this repo, then clone the branch of your choice from your forked repo down to your computer:

```
git clone -- git@github.com:[your-user-name]/webpack-express.git --
```

`cd` into your new folder and run:
- ```npm install```
- ```npm start``` to start the app
- this app runs on localhost:8080, but you can of course edit that in server.js

<!-- Further Notes -->

## Fixing JS

The JS needs to be usable, so we're adding it to a library via webpack. (See outputs)

In the HTML and your src JS files (src), you'll want to add "Client." to any functions that reference your JS (that is in this library upon production / run).

Update prod configurations to use some of the new loaders that we've been using in dev.

Tell prod to use / create the same library that dev is using.

Update formHandler.js and server/index.js to use a different port, so it can run at the same time as your app.

All the things to run:
npm install
npm i -D @babel/core @babel/preset-env babel-loader
npm i -D style-loader node-sass css-loader sass-loader
npm i -D clean-webpack-plugin
npm i -D html-webpack-plugin

npm run build-dev
npm run build-prod
