# Klahanie Website

The Klahanie website is a static site which is generated using Jekyll. 

### Creating announcements

To create a new announcement, add a new file to the _announcements folder following this template. When you add an announcement, it automatically adds it to the announcements page. Be sure to update the date, title, and body. The body follows a format called [Markdown](https://commonmark.org/help/), but you can add html as needed. 

```md
---
layout: default
title: Title of the article
date: 2019-05-27 03:59
author: Klahanie
comments: true
categories: [announcements]
show-title: true
---

This is the article body. 

* [Link](https://link.com)
* [Link](https://link.com)

### Subheader

Another paragraph

```

### Adding magazine publications
To add an magazine release to the magazines section, add the following to the _magazine directory. These should be named with the date of the release. 
* PDF of the magazine (2020-04-01.pdf)
* JPG of the magazine's cover (2020-04-01.jpg)
* MD file following the following format. Update the properties in the markdown file. 
 (2020-04-01.md)
  
```md
---
title: Klahanie Magazine - Winter 2012 
date: 2018-10-01 00:00
author: Klahanie
filename: 2018-10-01
description: Learn how Klahanie is modernizing our compliance strategy.  
---
```
