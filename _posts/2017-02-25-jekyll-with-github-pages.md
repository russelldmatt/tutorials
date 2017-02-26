---
layout: post
title:  "Set up jekyll static site with github pages"
date:   2017-02-25 21:57:22 -0500
categories: jekyll github github-pages
---

## Goal ##
- set up this jekyll site on github (project) page @ http://russelldmatt.github.io/tutorials/

## Instructions ##
- Local
  - create new [jekyll](https://jekyllrb.com/) instance: `jekyll new tutorials` 
- Github site
  - create new repo (tutorials)
- Local
  - cd tutorials
  - git init/add/commit
  - `git remote add origin https://github.com/russelldmatt/tutorials.git`
  - `git push -u origin master`
- Github site
  - [Setup Github Project Site](https://pages.github.com/)
    - Settings
    - Go down to github pages
    - Source -> "master branch"
    - Save
- Local
  - edit `_config.yml` in root of jekyll tree (Note: this does not auto-reload if you're serving local via `jekyll serve` so you need to re-serve)
    - edit title
    - edit email
    - edit description
    - edit (or delete) description
    - delete twitter username
    - edit github_username
    - edit baseurl, e.g. `baseurl: "/tutorials"` (Note: this will change the local serving location)
    - edit url, e.g. `url: "http://russelldmatt.github.io"`
  - edit the `about.md` in root
  
## Done! ##
