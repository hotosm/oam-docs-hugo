# HOT Documentation Site Template

Template for creating HOT documentation sites. 

This project uses the [Hugo](https://gohugo.io/) site generator for static HTML generation for Markdown content.

HOT maintains a custom HOT theme for Hugo sites here: [https://github.com/hotosm/hugo-book](https://github.com/hotosm/hugo-book)


To create a new HOT documentation site clone this repo:

```sh
git clone https://github.com/hotosm/hot-docs-template.git 
```

Then clone the HOT theme 
```
cd hot-docs-template
git submodule add https://github.com/hotosm/hugo-book themes/book
```

This template automates build and deployment using [CircleCI](https://circleci.com/). To take advantage of this functionality, a github repository and access to CircleCI is required. 


## Building a site

# Tutorial




### Configuration

Site level settings are stored in the [config.toml](./config.toml) at the root of this project

```toml
languageCode = "en-us"
title = "HOT Toolbox" <-- change me
theme = "book"
DefaultContentLanguage = "en"
relativeurls = true
enableGitInfo = true

[params]
    BookRepo = "https://github.com/hotosm/toolkit-site"  <-- change me
    BookShowToC = false
    BookEditPath = "/edit/master/content/"

[imaging]
    resampleFilter = "box"
    quality = 75
```


### Content

All Markdown content goes in the content directory. At minimum a site should have an ```_index.md``` file at the root of the content directory and a ```pages/``` directory with at least one markdown content page.  

* The ```_index.md``` file serves as the main landing page of the site or the / route of the page. 
* The ```pages/``` directory holds all pages listed in the file menu on the left of the page. 


The structure should be as follows:
```
content/
├── _index.md
└── pages/
    └── about.md
    └── contact.md

```

This content would create the following pages:

_index.md ---> https://example.com/

about.md ---> https://example.com/pages/about

contact.md ---> https://example.com/pages/contact


#### Front Matter

By default the name of the file in the /content/pages directory will be listed in the menu and in the URL with spaces escaped with dashes `-`. 

e.g. ```content/pages/how-i-spent-my-summer-vacation.md``` will show as How I Spent My Summer Vacation in the menu and as 
example.com/pages/how-i-spent-my-summer-vacation

You can change the title of the content in the Markdown front matter with the "title" parameter. e.g.


how-i-spent-my-summer-vacation.md
```md
---

title: Summer Essay - How I Spent My Summer Vacation

---

# Article Title

Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
sed do eiusmod tempor incididunt ut labore et dolore magna 
aliqua. Ut enim ad minim veniam, quis nostrud exercitation 
...
```


#### Table of Contents

By defualt in the main project config.toml file a right hand side Table of Contents is disabled.  If you need this enabled project-wide you can change this value to ``` true ``` in the TOML file or override in individual Markdown file by adding the ```  ``` option to the front matter. Table of contents will create a list of anchor points from the markdown header elements 
(``` # ## ### ### ```) and clicking them will auto scroll you to that section of the page. 

e.g
```md
---

title: Summer Essay - How I Spent My Summer Vacation
bookShowToC: True

---
```


### Multi-language Sites

This template allows for building multi-language sites by simply creating directories for each language needed, following the same directory structure as a single language site. an example folder structure is as follows:

```
content/
├── english/
│   ├── _index.md
│   └── pages
|       └── about.md 
└── french/
    ├── _index.md
    └── pages
        └── à-propos.md 
```


Then in your site config.toml tell Hugo how to find these directories:

```toml
[languages]
  [languages.en]
    contentDir = "content/english"
    languageName = "English"
    weight = 10
  [languages.fr]
    contentDir = "content/french"
    languageName = "Français"
    weight = 20
```

This will default the site to English but allow you to access the French content but suffixing a /fr to the base URL.

e.g.

https://example.com/pages/about

https://example.com/fr/pages/a-propos