---
date: {{ .Date }}
title: "{{ replace .Name "-" " " | title }}"
linkTitle: "{{ replace .Name "-" " " | title }}"
author: "Rex Walters"
description: ""
type: "docs"
weight: 2
resources:
  - src: "**.{png,jpg}"
    title: "Image #:counter"
---
