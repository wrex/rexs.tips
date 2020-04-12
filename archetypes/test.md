---
date: {{ .Date }}
title: "{{ replace .Name "-" " " | title }}"
linkTitle: "{{ replace .Name "-" " " | title }}"
author: "Rex Walters"
description: ""
tdgid: "TDG0000"
type: "docs"
weight: 2
resources:
- src: "**.{png,jpg}"
  title: "Image #:counter"
---
