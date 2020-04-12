---
date: {{ .Date }}
title: "{{ replace .Name "-" " " | title }}"
linkTitle: "{{ replace .Name "-" " " | title }}"
author: "Rex Walters"
tdg_id: "TDG0000"
description: ""
type: "docs"
weight: 2
resources:
- src: "**.{png,jpg}"
  title: "Image #:counter"
---
