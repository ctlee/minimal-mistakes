---
title: "Publications"
layout: archive
permalink: /publications/
author_profile: true
classes: wide
---

<p>
{% if site.author.googlescholar %}
	You can also find my articles on my more frequently updated <a href="{{site.author.googlescholar}}">Google Scholar</a> profile.<br/>
{% endif %}
<strong>Key:</strong> Icons link to DOI <i class="ai ai-doi" aria-hidden="true" title="permalink"></i>, biorxiv <i class="ai ai-biorxiv-square" aria-hidden="true" title="permalink"></i>, arxiv <i class="ai ai-arxiv-square" aria-hidden="true" title="permalink"></i>;<br/> 
&nbsp;&nbsp;&nbsp;&nbsp;<sup>*</sup> denotes equal contribution; <sup>$</sup> denotes corresponding author<br/> 

</p>

<h2>Submitted and In Preparation</h2>
<ul>
	{% for post in site.inpreps reversed %}
	  {% include inprep-pub-item.html %}
	{% endfor %}
</ul>

<h2>Peer Reviewed and In Press</h2>
[Sorted by year]({{ base_path }}by-year/){: .btn .btn--inverse .btn--small}
<ol>
	{% assign sorted = site.publications | sort:'date' | reverse %}
	{% for post in sorted %}
	  {% include num-pub.html %}
	{% endfor %}
</ol>
