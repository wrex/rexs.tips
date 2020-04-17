---
date: {{ .Date }}
title: "{{ replace .Name "-" " " | title }}"
linkTitle: "{{ replace .Name "-" " " | title }}"
description: ""
toc_hide: true
author: "Rex Walters"
resources:
  - src: "**.{png,jpg}"
    title: "Image #:counter"
---
