# HowToUploadReactCodeToGitHub
How to uload your react project on your github page step by step

step 1 : first run this command in your root directory

    npm install gh-pages --save-dev

step 2:  Make a repository on github with any name you want in the URL

step 3: Add these lines in package.json set the homepage and url formated as - https://<username>.github.io/<repository-name>.     Add this line 

    "homepage": "https://<yourusername>.github.io/<reponame>",

step 4: Add predeploy and deploy script in the package.json

    "predeploy": "npm run build",
    "deploy": "gh-pages -d build",

step 5: Initialize Git  Run this command in the root directory

    git init

step 6: Add and Commit Files:

    git add .
    git commit -m "Initial commit"

step 7: Push to GitHub  Run this command

    git remote add origin https://github.com/<username>/<repositoryname>.git
    git branch -M main
    git push -u origin main

step 8: Run Deploy this will publish the site on the github run this command

    npm run deploy
