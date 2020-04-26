# What is this

This is a tool to deploy static html on your Web App on Linux App Service Plan.

# How to use

1. Change the contents of `index.html`
    - Of course, you can add other contents as you want.
1. Deploy this directory to Web App
    - Note: VSCode with Azure App Service extension is useful to deploy

# Remarks

## Architecture of Web App

The Web App should be using `node.js` as an architecture, that means this repo doesn't work like with .Net Core selection.

## node_modules directory

You don't have to deploy `node_modules` directory. This directory would be deleted automatically after completing your deployment.
However, package.json is necessary  to run properly, so don't miss it.

# References

- Things You Should Know: Web Apps and Linux
    - https://docs.microsoft.com/ja-jp/archive/blogs/waws/things-you-should-know-web-apps-and-linux#NodeHome
    - This document says to use `express` library is a good solution.
- Cannot GET index.html Azure Linux Web App
    - https://stackoverflow.com/questions/54236862/cannot-get-index-html-azure-linux-web-app
    - This architecture is describing a solution how to deploy `index.html` file by using Linux App Service Plan.