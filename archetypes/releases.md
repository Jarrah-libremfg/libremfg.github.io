---
title: {{ replace .File.ContentBaseName `-` `.` | title | humanize }}
date: '{{ .Date }}'
description: Release notes for v{{ replace .File.ContentBaseName `-` `.` | title }} of the Rhize application
categories: ["releases"]
weight: 1 ##one if latest
menu:
  main:
    parent: releases
---

Release notes for version {{ replace .File.ContentBaseName `-` `.` | title }} of the Rhize application.

_Release date:_
{{ $t := time.Now }}{{ time.Format "2 Jan 2006" $t }}

## Breaking changes

## Changes by service

## Upgrade

To upgrade to v{{ replace .File.ContentBaseName `-` `.` | title }}, follow the [Upgrade instructions](/deploy/upgrade).
