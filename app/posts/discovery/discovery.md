---
layout: collection
title: Discovery
description: A service for candidates to find courses by location, provider or subject
related:
  items:
    - text: Prototype
      description: |
        Username: `find`
        Password: `bat`
      href: https://find-prototype.herokuapp.com/
pagination:
  data: collections.discovery
  reverse: true
  size: 50
permalink: "discovery/{% if pagination.pageNumber > 0 %}page/{{ pagination.pageNumber + 1 }}{% endif %}/"
override:tags:
  - post
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    excerpt: "{{ description }}"
    parent: home
    order: 1
---
