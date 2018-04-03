---
layout: search
title: Search
permalink: /search.html
banner-heading: Explore CDC Open Technology
banner-text:
hero-text: Enter a search term below.
category: search
---
<section>
  {% include search.html %}
</section>
<div id="search-results"></div>

<script>
  var baseurl = "{{ site.baseurl }}";
  var searchData = {{ site.data.search | jsonify }};
</script>


<script src="{{ '/assets/js/lib/lunr.min.js' | prepend: site.baseurl  }}"></script>
<script src="{{ '/assets/js/search.js' | prepend: site.baseurl  }}"></script>
