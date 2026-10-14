---
layout: page
permalink: /publications/
title: publications
description: publications in reversed chronological order.
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

## Books
{% bibliography -f {{ site.scholar.bibliography }} --query @book %}

## Journal articles
{% bibliography -f {{ site.scholar.bibliography }} --query @article %}

## Book chapters
{% bibliography -f {{ site.scholar.bibliography }} --query @incollection %}

## Encyclopedia entries and other
{% bibliography -f {{ site.scholar.bibliography }} --query @misc %}

</div>
