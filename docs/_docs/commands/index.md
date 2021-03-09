---
layout: docs
title: Commands
menu_name: Introduction
permalink: /docs/commands/
---


# Introduction

The database commands are executed in this order (for a batch download):

```
start()
for each image
    for each tag
        tag_before()
    image()
    for each tag
        tag_after()
end()
```

Database commands are enabled as soon as you put your database login information in the settings. Note that you have to create the database/tables beforehand.
