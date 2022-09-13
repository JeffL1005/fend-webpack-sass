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

## Production

formHandler.js is a good example of an GET request.

Optimization plugins (for CSS) have been added to the production configs. One replaces style-loader and two others are used for minifying.
npm install --save-dev mini-css-extract-plugin terser-webpack-plugin@4 optimize-css-assets-webpack-plugin

As always those plugins are required in the config file.

It's always good to look at the documentation to see how certain plugins should be used.

npm i -D mini-css-extract-plugin
npm i -D optimize-css-assets-webpack-plugin terser-webpack-plugin
npm run build-prod

Note: "@^" then the version number will load a certain version if you use it with the scripts.
