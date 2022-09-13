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

## Service Workers

Added to the production configuration. The first example is to offer offline viewing (sending a cached version of the site to view later).

As always: install the plugin, require the plugin, and instantiate the plugin.
https://developer.chrome.com/docs/workbox/the-ways-of-workbox/#using-a-bundler

Service workers get an extra step though. You'll want to add some JS in your HTML to call it if the browser supports it.

Make sure your module.exports (outputs) are updated in prod too!
