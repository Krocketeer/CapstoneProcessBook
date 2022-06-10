---
layout: home
title: Overview
nav_exclude: false
nav_order: 0
permalink: /
---

# Dropbox Clip

Introducing Dropbox Clip, a multi-device clipboard with an expanded capacity.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Ur5-U_L4FRg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

When Dropbox first approached us, they wanted us to investigate how Gen-Z creatives work on projects and interact with
files. Our initial research found that Gen-Z struggled to maintain organization of their cloud storage and instead used
the cloud storage to send files to others or between their own devices. Gen-Z tend to use ad-hoc ways to share content 
between their devices such as texting themselves or creating their own Discord server with themselves. In particular,
when they are using these ad-hoc ways, they are only doing it for immediate transfer of ephemeral content — content
that does not require long term storage. This lead us to the question of **how might we support immediate content sharing
across multiple devices?**

Dropbox Clip doesn't change the system's clipboard, but rather expands on it with additional features that we saw were
pain-points in our research. When a user copies something on their device, it copies directly into Dropbox Clip. Then, 
any other device that has Dropbox Clip as well can access that copied content. This provides a quick solution to share
content across devices regardless of operating system. Dropbox Clip can also hold up to six copied items at once,
allowing users to retrieve past copies conveniently without having to search for them again.

## Team Members

{% assign team_members = site.staffers | where: 'role', 'Team Member' %}
{% for staffer in team_members %}
{{ staffer }}
{% endfor %}


