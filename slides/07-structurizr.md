---
title: "Structurizr - java"
layout: Center
hide_toc: true
---

```java
Workspace workspace = new Workspace("techtribes.je", "This is a model...");
Model model = workspace.getModel();
SoftwareSystem techTribes = model.addSoftwareSystem("techtribes.je", "techtribes.je is the only way...");
SoftwareSystem twitter = model.addSoftwareSystem("Twitter", "twitter.com");
techTribes.uses(twitter, "Gets profile information and tweets from.");
SoftwareSystem gitHub = model.addSoftwareSystem("GitHub", "github.com");
techTribes.uses(gitHub, "Gets information about public code repositories from.");
SoftwareSystem blogs = model.addSoftwareSystem("Blogs", "RSS and Atom feeds");
techTribes.uses(blogs, "Gets content using RSS and Atom feeds from.");
...
```
