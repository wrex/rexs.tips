---
date: {{ .Date }}
title: "{{ replace .Name "-" " " | title }}"
linkTitle: "{{ replace .Name "-" " " | title }}"
author: "Rex Walters"
description: ""
tdgid: "D0000"
tutorial: ""
type: "tests"
weight: 2
resources:
  - src: "**.{png,jpg}"
    title: "Image #:counter"
---

{{% tdgtutorial %}}

## Demonstration

## Procedure

## Pass criteria

## Extra credit

## Subtests
