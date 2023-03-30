# Website Instructions

List of how Kristan can work on her website

## Working on the website

- open a terminal
- run `portfolio` in the terminal
- in a web browser go to page `http://127.0.0.1:4000/`
- make whatever changes you want to the website, the README.md has a solid set of instructions

### Adding a resume or CV

There is a default CV page that exists, but I think it's a bit of a pain to keep updating instead of just uploading a `.pdf` of whatever CV/resume you have. Let me know if you'd like to host a .pdf instead - that's what [I did on my website](https://alanpapalia.github.io/cv/) so it's easy to copy over.

### I want to modify the content on a page (non-project)

Most page content is is stored in markdown files in the `_pages` subfolder (`_pages/*.md`). There are some good samples already in the repo, so feel free to look around them to see how to do things. There's some metadata kept in the tops of the files that is often good to change.

For example, in the `_pages/projects.md` the top of the file says

```markdown
---
layout: page
title: projects
permalink: /projects/
description: A growing collection of your cool projects.
nav: true
nav_order: 2
display_categories: [work, fun]
horizontal: false
---
```

title - the title of the page and how it will be represented in the navigation bar at the top of the page
description - some more information that will be placed at the top of the page
nav - whether the link to the page will be shown in the navigation bar
nav_order - the ordering of where this page will be in the navbar (doesn't matter if `nav: false`)
display_categories - this is unique to this page and determines which categories of projects will be shown on the project page

### I want to modify or make a new project page

Modifying project pages is similar to other pages but is organized under the `_projects` subfolder (`_projects/*.md`).

### I'd like to add some pictures or a .pdf

Put any pictures you want to use in the folder `assets/img`. If you have a collection of photos you want to organize by category (like a specific project), you can make a new sub-folder `assets/img/new_folder` and put them there. There are examples

Similarly, `.pdf` files should go in `assets/pdf`. We can host your CV or resume on the website.


## Sharing your website with the world

- go to the repository - `cd kristanhilby.github.io`
- add your changes you've made - `git add .`
- commit the changes and give a message on what you've changed - `git commit -m "I made X Y Z changes since the last website update"`
- push the changes - `git push`
- enter your github username & password
- after a few minutes you should be able to see the changes online - https://kristanhilby.github.io
- note that I haven't spent time debugging the online website so there may be something weird, but it should be good!
