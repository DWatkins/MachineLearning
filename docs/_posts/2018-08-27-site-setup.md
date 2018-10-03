---
layout: post
title:  "Documentation Site Setup Steps"
author: dwatkins
---


This is a static site built with Jekyll using the **Jekyll Doc Theme** by [aksakalli](https://github.com/aksakalli/jekyll-doc-theme).

Setup details below

## Jekyll Setup

[Installation Instructions](https://jekyllrb.com/docs/installation/#ubuntu)

[Quick Start Instructions](https://jekyllrb.com/docs/quickstart/)

## Theme Setup

1. Download the [repo](https://github.com/aksakalli/jekyll-doc-theme) into `docs` folder (assuming gh-pages is set up to build from `docs` folder)

2. Open and modify `_config.yml` to replace the base url and github url with actual ones

3. commmit and push, example site should now be hosted

4. Modify as needed

## Serve Locally

```
#in repo
cd docs
bundle update
bundle exec jekyll serve
#navigate in browser to the server address specified on the command line to view
```
## MathJax Setup

[Jekyll Mention of MathJax](https://jekyllrb.com/docs/extras/#math-support)

[Adding MathJax to github pages jekyll site](http://sgeos.github.io/github/jekyll/2016/08/21/adding_mathjax_to_a_jekyll_github_pages_blog.html)

[MathJax Documentation](http://docs.mathjax.org/en/latest/tex.html)
