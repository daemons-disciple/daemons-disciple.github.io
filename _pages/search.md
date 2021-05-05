---
layout: page
title: Search
permalink: /search/
---

<div id="search-container">
    <wired-search-input type="text" id="search-input" placeholder="Search through blog post titles ..." style="font-family: Neucha,sans-serif;" elevation="3">
        Search box
    </wired-search-input>
    <ul id="results-container"></ul>
</div>

<script src="{{ site.baseurl }}/assets/simple-jekyll-search.min.js" type="text/javascript"></script>

<script>
    SimpleJekyllSearch({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    searchResultTemplate: '<div style="text-align: left !important;"><a href="{url}"><h1 style="text-align:left !important;">{title}</h1></a><span style="text-align:left !important;">{date}</span></div>',
    json: '{{ site.baseurl }}/search.json'
    });
</script>