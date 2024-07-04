---
layout: default
---

## About Me
<tr>
    <td> <img class="profile-picture" src="me.jpg"></td>
    <td><div class="profile-doc">
		Msc @ Brown University <br>
        Visual Computing & AI<br>
		<br> 
		<a href="mailto:aman_agarwal1@brown.edu">
			<i class="fa fa-envelope" aria-hidden="true"></i> aman_agarwal1@brown.edu</a> <br> 
		<a href="https://github.com/aman190202">
			<i class="fa fa-github" aria-hidden="true"></i> Github </a> <br> 
		<!-- <a href="https://scholar.google.com/citations?user=9ixpc8MAAAAJ&hl=en&oi=ao">
			<i class="fa fa-google" aria-hidden="true"></i> Google Scholar </a> <br>  -->
		<a href="https://www.linkedin.com/in/aman190202/">
			<i class="fa fa-linkedin" aria-hidden="true"></i> LinkedIn </a>
            <br>
			<br>
	</div></td>
</tr>

I am an upcoming CS Grad at Brown, joining the program this Fall. My primary research interests are Computer Vision and Graphics, particulary in the emerging field of Inverse rendering via Neural Fields such as [NeRFs](https://www.matthewtancik.com/nerf) and [Gaussian Splatting](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/).

## Experience
{% assign years = site.data.experience | group_by:"year" | sort: "name" | reverse %}

{% for year in years %}
### {{ year.name }}	
---

{% for jobs in year.items %}
<table class="paper-list">
  <tr>
  	{% if jobs.logo %}
    <td><img class="paper-logo" src="{{jobs.logo}}"></td>
	{% endif %}
	{% if paper.paper-logo-mp4 %}
    <td>
		<div class="paper-logo">
		<video width="80%" height="80%" muted autoplay loop>
			<source src="{{paper.paper-logo-mp4}}" type="video/mp4">
			Your browser does not support the video tag.
		</video>
		</div>
	</td>
	{% endif %}
    <td>
		<p class="paper-title">{{jobs.title}}</p>  
		<p class="paper-authors">
			{{jobs.description}}
		</p>
		<p class="paper-pub">{{paper.paper-pub}}</p>
		<p class="paper-links">
			{% if paper.link-pdf %}
			<a href="{{paper.link-pdf}}" target="_blank" rel="noopener">
				<i class="fa fa-file-pdf-o" aria-hidden="true"></i> PDF </a>
			{% endif %}

		</p>
	</td>
  </tr>
</table>
{% endfor %}
{% endfor %}


<!-- ## Publications
{% assign years = site.data.papers | group_by:"year" | sort: "name" | reverse %}

{% for year in years %}
### {{ year.name }}	
---

{% for paper in year.items %}
<table class="paper-list">
  <tr>
  	{% if paper.paper-logo %}
    <td><img class="paper-logo" src="{{paper.paper-logo}}"></td>
	{% endif %}
	{% if paper.paper-logo-mp4 %}
    <td>
		<div class="paper-logo">
		<video width="80%" height="80%" muted autoplay loop>
			<source src="{{paper.paper-logo-mp4}}" type="video/mp4">
			Your browser does not support the video tag.
		</video>
		</div>
	</td>
	{% endif %}
    <td>
		<p class="paper-title">{{paper.paper-title}}</p>  
		<p class="paper-authors">
			{% for author in paper.paper-authors %}
				{% if forloop.last == true %}
					{{author.name}}.
				{% else %}
					{{author.name}},
				{% endif %}
			{% endfor %}
		</p>
		<p class="paper-pub">{{paper.paper-pub}}</p>
		<p class="paper-links">
			{% if paper.link-pdf %}
			<a href="{{paper.link-pdf}}" target="_blank" rel="noopener">
				<i class="fa fa-file-pdf-o" aria-hidden="true"></i> PDF </a>
			{% endif %}

		</p>
	</td>
  </tr>
</table>
{% endfor %}
{% endfor %} -->

---
## Projects

<tr>
    <td><div>
        <a href="https://github.com/aman190202/LovingVincentt">
			<i class="fa fa-github" aria-hidden="true"></i> Loving Vincet:</a> Convert your videos into moving paintings of your choice
            <br> 
            <br> 
        <a href="https://github.com/aman190202/ray_tracing_weekend">
			<i class="fa fa-github" aria-hidden="true"></i>  Ray Tracer on MLX:</a> Implementing an entire Ray Tracer built from scratch in NumPy and modifying it to run on <a href="https://ml-explore.github.io/mlx/build/html/index.html">MLX</a>,a NumPy-like array framework designed for efficient and flexible machine learning on Apple silicon. [Ongoing]
            <br>
			<br> 
        <a href="https://devpost.com/software/rescue-shark">
			<i class="fa fa-github" aria-hidden="true"></i>  Rescue Shark:</a> Built a SOS application for Truck Drivers - Won a MLH Hackathon for "Most Creative Use of Twilio"
            <br>
			<br> 
	</div></td>
</tr>

<!-- ---
## Invited talks

Date | Event | Details
-----|-------|--------
April, 24th 2024 | FMX 2024  | Survey on NeRFs and 3DGS for the Lighting & Rendering track organized by [Christophe Hery](https://www.linkedin.com/in/christophehery/) in Stuttgart, Germany. Thank you all for the great time there!
May, 6th 2024 | Machine Learning Coffee Seminar | Finnish Center for Artificial Intelligence (FCAI) [talk](https://fcai.fi/calendar/2024/5/6/juho-kannala-tba) on neural rendering. -->


---
<br>
 Template Credits : <a href="https://maturk.github.io">Matias Turkulainen</a>