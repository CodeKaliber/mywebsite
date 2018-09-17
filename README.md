# mywebsite
Creating a gh-pages Front Page

gh-page Simple Front-End Website

Create Folder then open with Visual Studio - VS
Create Folder any name example dist
Create two files in the Folder called index.html and About.html
RUN npm init - (Creates package.json)

{
  "name": "mywebsite",
  "version": "1.0.0",
  "description": "Creating a Simple gh-page Front Page",
  "main": "index.js",
  "scripts": {
    "deploy": "gh-pages -d dist" <— Change “test” to “deploy” and add gh-pages -d with folder name that has index.html in it OR in react “build” after running npm build.
  },
  "keywords": [],
  "author": "Kevin Patterson",
  "license": "MIT",
  "homepage": "https://CodeKaliber.github.io/mywebsite", <— This is added manually
  "dependencies": {
    "gh-pages": "^2.0.0"
  }
}

Run npm i gh-pages <— This added the “dependencies” to the (package.json) above.

Now create a NEW Repository in your GitHub

Create .gitignore in the root and add “node_modules” so the node_modules doesn’t load to the GitHub Repo.
Run git init again
Run git add .
Run git commit -m “Some Messages”
NOW copy the ‘git remote add origin https://github.com/CodeKaliber/mywebsite.git' from your GitHub page and paste into VS Terminal
Then Run ‘git push -u origin master’ in the VS Terminal
NOW go to GitHub page and refresh — this will show all code from your VS to your GitHub Repo
NOW to get “gh-pages” on your Repository you Run “npm run deploy” in your VS Terminal then go to GitHub page and refresh the page.
NOW on your GitHub page click setting button upper right and scroll down to the link that was created. Click to see your site.
