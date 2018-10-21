---
layout: search
title: Search
permalink: /search.html
banner-heading: Search
banner-text:
hero-text: Explore CDC Open Technology
category: search
---
<div id="search-results">Please use the search at the top to begin exploring CDC Open Technology.</div>

<script>
  var baseurl = "{{ site.baseurl }}";
  var searchData = {{ site.data.search | jsonify }};
</script>

<script src="{{ '/assets/js/lib/lunr.min.js' | prepend: site.baseurl  }}"></script>
<script src="{{ '/assets/js/search.js' | prepend: site.baseurl  }}"></script>
