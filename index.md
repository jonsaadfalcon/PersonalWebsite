---
layout: home
title: Home
---

<div id ="intro-wrapper" class="l-middle">
	<div id="intro-title-wrapper" class="intro-left">
		<h1 id="intro-title">Jon Saad-Falcon</h1>
		<!-- <div id="intro-subtitle">
			Research Assistant at Stanford University.
		</div> -->
	</div>
	<div class="intro-left">
	<div class="intro-left">
		I am a joint Computer Science Ph.D. and MBA student at Stanford University <img class="intro-logo" style="width: 22px; padding-bottom: 5px;" src="/images/stanford.svg" />, advised by <a href="http://azaliamirhoseini.com/">Azalia Mirhoseini</a> (<a href="https://scalingintelligence.stanford.edu/">Scaling Intelligence Lab</a>) and <a href="https://cs.stanford.edu/~chrismre/">Christopher Ré</a> (<a href="https://hazyresearch.stanford.edu/">Hazy Research</a>). Previously, I was a research assistant at Stanford, advised by <a href="https://web.stanford.edu/~cgpotts/">Christopher Potts</a> and <a href="https://cs.stanford.edu/people/matei/">Matei Zaharia</a>. I completed the joint B.S./M.S. in Computer Science at Georgia Tech <img class="intro-logo" style="width: 18px; padding-bottom: 3px;" src="/images/gt.png" />, where I was advised by <a href="http://www.cc.gatech.edu/~dchau/">Polo Chau</a> and <a href="https://cs.stanford.edu/~diyiy/">Diyi Yang</a>.
	</div>
	<div style="height: 1rem"></div>
	<div class="intro-left">
		I was supported by the <a href="https://stampsps.gatech.edu/">Stamps President's Scholarship</a>. I also worked as a Predoctoral Young Investigator at the <a href="https://allenai.org/">Allen Institute for Artificial Intelligence (AI2)</a>, advised by <a href="https://users.cs.northwestern.edu/~ddowney/">Doug Downey</a>. Additionally, I received a <a href="https://us.fulbrightonline.org/">Fulbright Scholarship</a> and <a href="https://www.gatescambridge.org/">Gates-Cambridge Scholarship</a>.
	</div>
	<div style="height: 1rem"></div>
	<div>
		My research interests span across <b>natural language processing</b>, <b>machine learning</b>, <b>information retrieval</b>, and <b>ML systems</b>. I've had the privilege to collaborate with researchers and scientists at <img class="intro-logo" style="width: 22px; padding-bottom: 5px;" src="/images/stanford.svg" /> Stanford AI Lab, <img class="intro-logo" style="width: 25px; padding-bottom: 3px;" src="/images/AI2.svg" /> Allen Institute for Artificial Intelligence (AI2), and <img class="intro-logo" style="width: 22px" src="/images/goldmansachs.svg" /> Goldman Sachs.
	</div>
</div>

<div class="intro-right">
	<img id="intro-image" class="intro-right" src="/images/jon.png">
	<div style="height: 0.5rem"></div>
	<div id="intro-image-links" class="intro-right">
		{% for link in site.data.social-links %}
			{% if link.on-homepage == true %}
				{% include social-link.html link=link %}
			{% endif %}
		{% endfor %}
	</div>
	<div style="height: 0.5rem"></div>
	<div id="intro-cv-wrapper" class="intro-right">
		{% for link in site.data.social-links %}
			{% if link.id == "cv-web" %}
				{% include social-link.html link=link %}
			{% endif %}
		{% endfor %}
		<!-- <div id="intro-cv"><a href="/cv">Here's my CV.</a></div> -->
	</div>
	</div>
</div>

<hr class="l-middle home-hr">

<h2 class="feature-title l-middle">
	Featured <a href="/cv#publications">Research Publications</a>
</h2>
<div class="cover-wrapper l-screen">
	{% assign sortedPublications = site.categories.papers | sort: 'feature-order' %}
	{% for feature in sortedPublications %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>



[gt]: http://www.gatech.edu "Georgia Tech"
[cse]: http://cse.gatech.edu "Georgia Tech Computational Science and Engineering"
[coc]: http://www.cc.gatech.edu "Georgia Tech College of Computing"

[cv]: {{ site.url }}/cv
[polo]: http://www.cc.gatech.edu/~dchau/ "Polo Chau"
