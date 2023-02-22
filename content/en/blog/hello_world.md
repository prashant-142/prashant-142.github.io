---
author: "Prashant Yadav"
title: "How to create Hugo blog"
description: "Sample article showcasing basic Markdown syntax and formatting for HTML elements."
tags: ["markdown", "css", "html"]
date: 2022-07-14
thumbnail: https://picsum.photos/id/1019/500/200
---


## Hello This is my first blog with 191 words.
### Checking how the third line looks like

Create 2 github repos. 
1) Hugo blog -  Where you will be creating your blog
2) Your username - Where you'll be hosting the blog

In local create hugo blog, add upstream origin to github Hugo blog repo

commands
*hugo new site blog*
cd blog
D:\Projects\hugo>cd blog

D:\Projects\hugo\blog>git init
Initialized empty Git repository in D:/Projects/hugo/blog/.git/
D:\Projects\hugo\blog>git branch -M 'main'
D:\Projects\hugo\blog>git remote add origin https://github.com/prashant-142/hugo-blog.git

Add gitignore from toptal
git add .
git push origin HEAD

Add Blist Theme.
$ git submodule add https://github.com/apvarun/blist-hugo-theme.git themes/blist

Configuring theme to a hugo website 
Copy package.json and package-lock.json to the root folder of your the website
Run npm install to install required packages for theme
Run npm i -g postcss-cli to use PostCSS with Hugo build
Set theme = 'blist' in config.toml
Run npm start to start your local server


## Add Github pages repo to the public folder.
git submodule add -f https://github.com/prashant-142/prashant.git public

Build hugo blist theme and push changes to public folder for deployment
hugo -t blist

Create first blog
hugo new blog/hello_world.md

Create First Page
hugo new page/about.md

## Helpful Links

[Blogging with Hugo and Github Actions](https://www.youtube.com/watch?v=aqAaYZOqiTw)

[Automatically deploy Hugo site to GitHub pages with actions](https://xdeb.org/post/2023/deploy-hugo-github-pages-actions/)

[Deploying a Blog Powered by Hugo to Github Pages w/ Custom Domain via Github Actions](https://theplaybook.dev/docs/deploy-hugo-to-github-pages/)

[Using GitHub Pages with Actions to deploy Hugo sites in seconds - Tommy Byrd // HugoConf 2022](https://www.youtube.com/watch?v=Z_7RIuf_Z-Q)





