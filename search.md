---
layout: page
title: Lorg
permalink: /lorg/
---

Tòisich a' sgrìobhadh anns a' bhogsa gu h-ìosal airson lorg sna puist.

<!-- Html Elements for Search -->
<div class="form-group" id="search-container">
<input class="form-control" type="text" id="search-input" placeholder="Lorg sna puist..."><br />
<ul id="results-container"></ul>
</div>

<!-- Script pointing to search-script.js -->
<script src="{{ site.baseurl }}/search-script.js" type="text/javascript"></script>

<!-- Configuration -->
<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '{{ site.baseurl }}/search.json'
})
</script>
