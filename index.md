---
layout: default
---

## About Me
<tr>
    <td> <img class="profile-picture" src="me.png" style="width: 25%; height: auto;"></td>
	<!-- <td>
		<iframe src="https://antimatter15.com/splat/?url=https://aman190202.github.io/model-5.splat" width="300" height="300" style="border:none;  float: right;"></iframe>
	</td> -->
    <td><div class="profile-doc">
		Sc.M. @ Brown University <br>
        Visual Computing & AI<br>
		<br> 
		<a href="mailto:amanag@brown.edu">
			<i class="fa fa-envelope" aria-hidden="true"></i> amanag@brown.edu</a> <br> 
		<a href="https://github.com/aman190202">
			<i class="fa fa-github" aria-hidden="true"></i> Github </a> <br> 
		<!-- <a href="https://scholar.google.com/citations?user=9ixpc8MAAAAJ&hl=en&oi=ao">
			<i class="fa fa-google" aria-hidden="true"></i> Google Scholar </a> <br>  -->
		<a href="https://www.linkedin.com/in/aman190202/">
			<i class="fa fa-linkedin" aria-hidden="true"></i> LinkedIn </a> <br> 
		<a href="https://antimatter15.com/splat/?url=https://aman190202.github.io/model-5.splat">
			<i aria-hidden="true"></i> 💻 Watch me in 3D</a>
            <br>
			<br>
	</div></td>
</tr>

I'm a Master's student in Computer Science at Brown University, specializing in **Visual Computing and AI**. I am advised by [Dr. James Tompkin](https://jamestompkin.com), and my current research focuses on interpretibility of 3D and 4D feedforward models.


---
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
<!-- ## Projects

<tr>
    <td><div>
	    <a href="https://github.com/aman190202/neural_fields_bvc">
            <i class="fa fa-github" aria-hidden="true"></i> Neural Fields with encoding:</a> A comparision of different encoding methods for 2D inputs
            <br> 
            <br> 
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
</tr> -->

<style>
    body {
        background-color: #ffffff !important; /* Set background to white */
        color: #000000; /* Change text color to black for visibility */
    }
    h1, h2, h3, h4, h5, h6 {
        color: #000000; /* Ensure all headings are visible on white background */
    }
    .page-title {
        color: orange; /* Set your title color to orange */
    }
    .header-name {
        color: orange; /* Set your name color to orange */
    }
    .link-box {
        position: relative;
        display: inline-block;
        padding: 10px;
        border: 2px solid #000000;
        border-radius: 8px;
        transition: transform 0.3s;
        width: 100%;
        box-sizing: border-box;
    }
    .link-box:hover {
        transform: scale(1.05); /* Pop-up effect */
    }
    a {
        color: #4da6ff; /* Default link color (light blue) */
        text-decoration: none; /* Remove underline */
    }
    a:hover {
        color: orange; /* Change link color to orange on hover */
        text-decoration: underline; /* Optional: add underline on hover */
    }
    .project-container {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 20px;
    }
    .project-item {
        text-align: center;
        margin-bottom: 20px;
    }
    .project-image {
        width: auto;
        border-radius: 10px;
        height: 200px;
        max-width: 100%;
    }
    
    /* Dynamic background for experience section */
    @keyframes gradientAnimation {
        0% {
            background-position: 0% 50%;
        }
        50% {
            background-position: 100% 50%;
        }
        100% {
            background-position: 0% 50%;
        }
    }

    /* Experience section styling */
    .paper-list {
        background: linear-gradient(270deg, #f5f5f5, #e5e5e5, #f5f5f5);
        background-size: 400% 400%;
        animation: gradientAnimation 15s ease infinite; /* Apply animation */
        color: #000000; /* Text color */
        border-radius: 8px;
        padding: 10px;
        margin-bottom: 15px;
        transition: transform 0.3s;
        border: 1px solid #cccccc;
    }
    .paper-list:hover {
        transform: scale(1.02);
    }
    .paper-title {
        color: #000000 !important;
        font-weight: bold;
    }
    .paper-authors, .paper-pub, .paper-links {
        color: #333333 !important;
    }
    .paper-logo {
        background-color: transparent !important;
    }
    
    /* Fix for any tables in the document */
    table {
        background-color: #ffffff !important;
        color: #000000 !important;
        border-collapse: collapse;
    }
    td, th {
        color: #000000 !important;
        padding: 8px;
        background-color: #ffffff !important;
    }
    
    /* Profile section */
    .profile-doc, .profile-picture {
        color: #000000 !important;
    }
    
    /* Resume section styling */
    .resume-section, .resume-section * {
        color: #000000 !important; /* Ensure all text in the resume section is black */
    }
    
    /* Fix for section backgrounds */
    section, div, article {
        background-color: #ffffff !important;
    }
</style>



## Projects




<div class="project-container">
    <!-- Project 0 -->
    <div class="project-item">
        <div class="link-box">
            <a href="https://github.com/aman190202/cuda" style="text-decoration: none; color: inherit;">
                <video controls style="width: 100%; border-radius: 10px; max-height: 200px;">
                    <source src="assets/100000.mov" type="video/mp4">Your browser does not support the video tag.
                </video>
                <h3>Explosion</h3>
            </a>
        </div>
        <p>
            Designed and implemented a volumetric path tracer to render explosions with millions of lights
        </p>
    </div>

    <!-- Project 1 -->
    <div class="project-item">
        <div class="link-box">
            <a href="https://github.com/aman190202/Clouds" style="text-decoration: none; color: inherit;">
                <video controls style="width: 100%; border-radius: 10px; max-height: 200px;">
                    <source src="assets/FullHD.mp4" type="video/mp4">Your browser does not support the video tag.
                </video>
                <h3>Volummetric Rendering for Clouds & Procuderal Terrain, on OpenMP</h3>
            </a>
        </div>
        <p>
            Designed and implemented a custom ray-marcher and ray-tracer from scratch to render realistic clouds and generate procedural terrain. The rendered scene includes dynamic interactions with point lights, creating visually accurate and immersive effects.
        </p>
    </div>
    
    <!-- Project 2 -->
    <div class="project-item">
        <div class="link-box">
            <a href="https://github.com/aman190202/small_NeRF" style="text-decoration: none; color: inherit;">
                <img src="assets/img_0_21.png" alt="Neural Radiance Fields" class="project-image">
                <h3>Implemented NeRFs</h3>
            </a>
        </div>
        <p>Implemented the <a href="https://arxiv.org/abs/2003.08934">Neural Radiance Fields</a> paper by Ben Mildenhall et al.; Removed heirarical sampling to reduce complexity while maintaining PSNR scores.</p>
    </div>
    
    <!-- Project 3 -->
    <div class="project-item">
        <div class="link-box">
            <a href="https://github.com/aman190202/neural_fields_bvc" style="text-decoration: none; color: inherit;">
                <img src="assets/output2.png" alt="Neural Fields Thumbnail" class="project-image">
                <h3>Neural Fields with Encoding</h3>
            </a>
        </div>
        <p>A comparison of different encoding methods for 2D inputs</p>
    </div>
    
    <!-- Project 4 -->
    <div class="project-item">
        <div class="link-box">
            <a href="https://github.com/aman190202/LovingVincentt" style="text-decoration: none; color: inherit;">
                <img src="assets/ezgif.com-gif-maker.gif" alt="Loving Vincent Thumbnail" class="project-image">
                <h3>Loving Vincent</h3>
            </a>
        </div>
        <p>Convert your videos into moving paintings of your choice</p>
    </div>
    
    <!-- Project 5 -->
    <div class="project-item">
        <div class="link-box">
            <a href="https://devpost.com/software/rescue-shark" style="text-decoration: none; color: inherit;">
                <img src="https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/001/638/714/datas/original.JPG" alt="Rescue Shark Thumbnail" class="project-image">
                <h3>Rescue Shark</h3>
            </a>
        </div>
        <p>Built an SOS application for Truck Drivers - Won a MLH Hackathon for "Most Creative Use of Twilio"</p>
    </div>
</div>


<!-- ---
## Invited talks

Date | Event | Details
-----|-------|--------
April, 24th 2024 | FMX 2024  | Survey on NeRFs and 3DGS for the Lighting & Rendering track organized by [Christophe Hery](https://www.linkedin.com/in/christophehery/) in Stuttgart, Germany. Thank you all for the great time there!
May, 6th 2024 | Machine Learning Coffee Seminar | Finnish Center for Artificial Intelligence (FCAI) [talk](https://fcai.fi/calendar/2024/5/6/juho-kannala-tba) on neural rendering. -->


---
<br>
 Template Credits : <a href="https://maturk.github.io">Matias Turkulainen</a>

