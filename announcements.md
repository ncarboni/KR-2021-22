---
layout: page
title: Announcements
nav_exclude: true
description: A feed containing all of the class announcements.
---


{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}
