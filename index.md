---
layout: home
title: Home
---

<div id ="intro-wrapper" class="l-middle">
	<div id="intro-title-wrapper" class="intro-left">
		<h1 id="intro-title">Jon Saad-Falcon</h1>
		<!-- <div id="intro-subtitle">
			Undergrad in the College of Computing at Georgia Tech.
		</div> -->
	</div>
	<div class="intro-left">
	<div class="intro-left">
		I'm currently completing the joint B.S./M.S. in Computer Science in the College of Computing at Georgia Tech <img class="intro-logo" style="width: 18px; padding-bottom: 3px;" src="/images/gt.png" />. I'm advised by <a href="http://www.cc.gatech.edu/~dchau/">Polo Chau</a> and <a href="https://www.cc.gatech.edu/~dyang888/">Diyi Yang</a>, working at the <a href="http://poloclub.gatech.edu">Polo Club of Data Science</a> and <a href="https://www.cc.gatech.edu/~dyang888/group.html">Social and Language Technologies (SALT)</a> lab, respectively. I am currently supported by the <a href="https://stampsps.gatech.edu/">Stamps President's Scholarship</a> and work as a Predoctoral Young Investigator at the <a href="https://allenai.org/"> Allen Institute for Artificial Intelligence (AI2)</a>.
	</div>
	<div style="height: 1rem"></div>
	<div>
		My research interests span across natural language processing, machine learning, and human-computer interaction. I'm excited to work on projects that use NLP architectures and models in the biomedical and scientific domains. 
	</div>
	<div style="height: 1rem"></div>
	<div>
		I've had the privilege to collaborate with researchers and scientists at <img class="intro-logo" style="width: 22px; padding-bottom: 5px;" src="/images/stanford.svg" /> Stanford AI Lab, <img class="intro-logo" style="width: 25px; padding-bottom: 3px;" src="/images/AI2.svg" /> Allen Institute for Artificial Intelligence (AI2), and <img class="intro-logo" style="width: 22px" src="/images/goldmansachs.svg" /> Goldman Sachs.
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
