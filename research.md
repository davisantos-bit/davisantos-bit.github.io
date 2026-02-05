---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

## Journal Articles
{% assign pubs = site.publications 
   | where: "pubtype", "journal" 
   | sort: "date" 
   | reverse %}
{% for post in pubs %}
  {% include archive-single.html %}
{% endfor %}

## Working Papers
{% assign pubs = site.publications 
  | where: "pubtype", "workingpaper" 
  | sort: "date" 
  | reverse %}
{% for post in pubs %}
  {% include archive-single.html %}
{% endfor %}

## Book Chapters
{% assign pubs = site.publications | where: "pubtype", "chapter" %}
{% for post in pubs %}
  {% include archive-single.html %}
{% endfor %}
