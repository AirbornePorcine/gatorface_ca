---
layout: default
title: Projects
header_type: hero
header_img: /assets/images/IMG_0190.webp
permalink: /projects/
---

Examples of my past projects. New things are happening all the time, this is just an sample of the breadth of work I do.

{% assign images = "" | split: "," %}
{% assign captions = "" | split: "," %}
{% assign links = "" | split: "," %}

{% for project in site.projects %}
  {% if project.image %}
    {% assign images = images | push: project.image %}
    {% assign captions = captions | push: project.title %}
    {% assign links = links | push: project.url %}
  {% endif %}
{% endfor %}

{% include lightbox.html images=images captions=captions links=links %}