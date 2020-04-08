---
date: {{ .Date }}
title: "{{ replace .Name "-" " " | title }}"
linkTitle: "{{ replace .Name "-" " " | title }}"
description: ""
author: "Rex Walters"
resources:
- src: "**.{png,jpg}"
  title: "Image #:counter"
---
