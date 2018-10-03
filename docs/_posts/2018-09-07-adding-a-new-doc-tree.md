---
layout: post
title:  "Adding a New Documentation Tree"
author: dwatkins
---

The following are instructions for adding an additional documentation tree. In other words, this is the process to add a new collection of documents that will be separte from `Docs` and will have its own side menu and navigation.

![]({{ "/assets/docs-otherdocs-blog.PNG" | relative_url }})


## Create the new collections folder

```bash
#in root dir
mkdir _docsname
```

## Update `_config.yml` to include the new collection

```yaml
defaults:
- scope:
    path: _docsname
    type: docsname
  values:
    layout: docs
    sectionid: docsname
    seo:
      type: "WebPage"


collections:
  docsname:
    permalink: /:collection/:path/
    output: true

```

## Add content

`.md` files with front matter

```yaml
---
title: [Title]
permalink: /otherdocs/[path]/
---
```
## Add a new data file to describe order and contents

Create a file names `docsname.yml` in `_data` and specify the ordering of content. 

See the original `_data/docs.yml` as an example



