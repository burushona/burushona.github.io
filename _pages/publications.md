---
layout: page
permalink: /publications/
title: publications
description:
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<style>
  .publications h2.pub-section { font-size: 1.6rem; font-weight: 500; margin-top: 3rem; margin-bottom: 0.5rem; }
  .publications h2.pub-section:first-child { margin-top: 1rem; }
  .publications .reference { padding-left: 1.5em; text-indent: -1.5em; }
  .publications .reference a { color: var(--global-theme-color); overflow-wrap: break-word; }
  .publications ol.bibliography .row { margin-left: 0; margin-right: 0; }
  .publications ol.bibliography .row > div { padding-left: 0; padding-right: 0; }
  .publications .links { margin-top: 0.25rem; }
</style>

<div class="publications">

<h2 class="pub-section">Books</h2>
{% bibliography -f {{ site.scholar.bibliography }} --query @book[keywords!~edited] %}

<h2 class="pub-section">Edited volumes and special issues</h2>
{% bibliography -f {{ site.scholar.bibliography }} --query @*[keywords~=edited] %}

<h2 class="pub-section">Journal articles</h2>
{% bibliography -f {{ site.scholar.bibliography }} --query @article[keywords!~edited] %}

<h2 class="pub-section">Book chapters and encyclopedia entries</h2>
{% bibliography -f {{ site.scholar.bibliography }} --query @incollection[keywords!~edited] %}

</div>
