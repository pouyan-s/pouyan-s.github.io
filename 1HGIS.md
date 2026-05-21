---
title: Historical GIS (HGSI)
layout: landing
description: 'From historical texts, maps & archival imagery to temporally dynamic geospatial narratives, geodatabases & spatial analysis'
image: assets/images/01_HGIS/01_StryMpThumb.png
nav-menu: true
permalink: /HGIS/
---

<!-- Main -->
<div id="main">

<!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h2 style="color:#8ED530">About My Methodology</h2>
		</header>
		<!-- Left column -->
		<div class="row">
			<div class="6u 12u$(small)">
				<p>I use geographic information systems (GIS) to visualize and analyze historical data on maps, framing each piece as a quadruple of actor, action, location, and time. I build geospatial databases from these units and often animate temporal data to reveal local motion and shifting circumstances over time. Through techniques of 3D mapping in historical GIS, I offer scholars and learners a spatial sense of the past. I extract historical data from maps, aerial photographs, and footage—both vertical and oblique—by georeferencing them. These practices allow me to construct historical landscapes by establishing simultaneity between events in their context and by shifting the scale of historical inquiry, ultimately leading to the creation of nuanced historical narratives.</p>
			</div>
		<!-- Right column -->
			<div class="6u$ 12u$(small)">
				<div style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden; max-width:100%;">
				  <iframe
					src="https://www.youtube.com/embed/ZH_q3VcIouM?autoplay=1&mute=1&controls=0&loop=1&playlist=ZH_q3VcIouM&modestbranding=1&rel=0"
					title="YouTube video"
					frameborder="0"
					allow="autoplay; encrypted-media"
					allowfullscreen
					style="position:absolute; top:0; left:0; width:100%; height:100%;"
				  ></iframe>
				</div>
				<p style="text-align: center; font-size:12px;">My 3D visualization of a user-contributed GPS track in QGIS, combined with a digital terrain model of the Damavand region, reveals possible historical trails that are absent from existing maps.</p>
			</div>
        </div>
		<div>
			<header class="major">
				<h2 style="color:#8ED530">Explore My HGIS Projects</h2>
			</header>
			<ul class="actions small">
				<li><a href="#Avicenna" class="button small">Mapping Avicenna</a></li>
				<li><a href="#Isfahan" class="button small">Avicenna in Isfahan</a></li>
				<li><a href="#GPSing" class="button small">GPSing Travelers</a></li>
				<li><a href="#Community" class="button small">Community Archiving</a></li>
				<li><a href="#Leaflet" class="button small">Leaflet Mapping</a></li>
			</ul>
		</div>
	</div>
</section>

<!-- Two -->
<section id="" class="spotlights">
	<section id="Avicenna">
		<a href="{{ '/mapping-avicenna/' | relative_url }}" class="image">
			<iframe
			  width="500"
			  height="500"
			  src="https://www.youtube.com/embed/w1xd4-lCOZg?autoplay=1&mute=1&controls=0&loop=1&playlist=w1xd4-lCOZg&modestbranding=1&rel=0"
			  title="YouTube Shorts video"
			  frameborder="0"
			  allow="autoplay; encrypted-media"
			  allowfullscreen
			></iframe>
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3 style="color:#E0115F;"><a href="{{ '/mapping-avicenna/' | relative_url }}">Mapping Avicenna: A Geospatial Bio-Bibliography for Animated Visualization and Analysis</a></h3>
				</header>
				<p>In my doctoral dissertation, I employed GIS-based mapping as a digital humanities method to engage with the complex corpus of Avicenna (Ibn Sīnā, 10th–11th c. CE), much of which was produced during his lifelong itinerancy. I extracted his whereabouts — recorded as placenames with latitude and longitude — and his scholarly output across time and space, structuring this data as a CSV. I also digitized roads and the shifting borders of ruling dynasties during Avicenna’s lifetime from historical print maps.</p>
				<ul class="actions">
					<li><a href="{{ '/mapping-avicenna/' | relative_url }}" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	<section id="Isfahan" style="scroll-margin-top:50px;">
		<a href="{{ '/avicenna-in-isf/' | relative_url }}" class="image">
			<img src="{% link assets/images/02_Avicenna_in_Isf/01 out_view.png %}" alt="" data-position="top center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3 style="color:#E0115F;"><a href="{{ '/avicenna-in-isf/' | relative_url }}">Ibn Sīnā (Avicenna) in Isfahan: A Geospatial Critique of his Imagined Past in the City</a></h3>
				</header>
				<p>In the Dardasht district of Isfahan (Iran) stands a dodecagonal, domed building known as the Madras-i Ibn Sīnā (Academy of Avicenna). It is widely believed to be the site where Avicenna (Ibn Sīnā, 980–1037 CE), the renowned physician-philosopher and polymath, taught students during his residence in Isfahan (1024–1037 CE). I used digital mapping to critically assess this claim.</p>
				<ul class="actions">
					<li><a href="{{ '/avicenna-in-isf/' | relative_url }}" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	<section id="GPSing" style="scroll-margin-top:50px;">
		<a href="{{ '/GPSing/' | relative_url }}" class="image">
			<iframe
			  width="560"
			  height="315"
			  src="https://www.youtube.com/embed/jtdcdC9QQB8?start=10&end=13&autoplay=1&mute=1&controls=0&loop=1&playlist=jtdcdC9QQB8&modestbranding=1&rel=0"
			  title="YouTube Shorts video"
			  frameborder="0"
			  allow="autoplay; encrypted-media"
			  allowfullscreen
			></iframe>
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3 style="color:#E0115F;"><a href="{{ '/GPSing/' | relative_url }}">GPSing Historical Travelers: Dynamic Spatiotemporal Mapping and 3D Trajectory Visualization of Sadegh Hedayat's Isfahan Travel Account</a></h3>
				</header>
				<p>This ongoing project draws on the logistical data embedded in Hedayat’s account to reconstruct the dynamics of intercity travel in the early 20th century. I focus on the route, stops, timing, pace, and landscapes described in the text, integrating them into a temporally dynamic map and a 3D scene to offer a spatial and experiential understanding of the journey—especially for readers unfamiliar with the geography and historical context.</p>
				<ul class="actions">
					<li><a href="{{ '/GPSing/' | relative_url }}" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	<section id="Community">
		<a href="{{ '/GIS-for_CommArch/' | relative_url }}" class="image">
			<iframe
			  width="560"
			  height="420"
			  src="https://www.youtube.com/embed/-w7pe8xkvkE?autoplay=1&mute=1&controls=0&loop=1&playlist=-w7pe8xkvkE&modestbranding=1&rel=0"
			  title="YouTube Shorts video"
			  frameborder="0"
			  allow="autoplay; encrypted-media"
			  allowfullscreen
			></iframe>
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3 style="color:#E0115F;"><a href="{{ '/GIS-for_CommArch/' | relative_url }}">GIS for Community Archival Access</a></h3>
				</header>
				<p>This project explores GIS-based solutions to make cartographic records (maps, aerial photographs) and photographic records of places from the Weston Historical Society’s community archive publicly accessible, with minimal computational demands and technical skill requirements.</p>
				<ul class="actions">
					<li><a href="{{ '/GIS-for_CommArch/' | relative_url }}" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	<section id="Leaflet">
		<a href="{{ '/web-mapping/' | relative_url }}" class="image">
			<iframe
  width="420"
  height="525"
  src="https://www.youtube.com/embed/0cxjKr0tEb4?autoplay=1&mute=1&controls=0&loop=1&playlist=0cxjKr0tEb4&modestbranding=1&rel=0"
  title="YouTube Shorts video"
  frameborder="0"
  allow="autoplay; encrypted-media"
  allowfullscreen
></iframe>
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3 style="color:#E0115F;"><a href="{{ '/web-mapping/' | relative_url }}">Leaflet-based Web Mapping</a></h3>
				</header>
				<p>Sharing maps on proprietary platforms can be costly and often comes with storage limitations. To ensure open and sustainable access, I used the QGIS2Web plugin to export maps as Leaflet-based interactive web maps, then customized them with JavaScript, HTML, and CSS.</p>
				<ul class="actions">
					<li><a href="{{ '/web-mapping/' | relative_url }}" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
</section>
<!-- Contact -->
<section id="two">
	<div class="inner">
		<header class="major">
			<h2>Contact Me</h2>
		</header>
		<!--<p>Nullam et orci eu lorem consequat tincidunt vivamus et sagittis libero. Mauris aliquet magna magna sed nunc rhoncus pharetra. Pellentesque condimentum sem. In efficitur ligula tate urna. Maecenas laoreet massa vel lacinia pellentesque lorem ipsum dolor. Nullam et orci eu lorem consequat tincidunt. Vivamus et sagittis libero. Mauris aliquet magna magna sed nunc rhoncus amet pharetra et feugiat tempus.</p>
		<ul class="actions">
			<li><a href="generic.html" class="button next">Get Started</a></li>
		</ul>-->
	</div>
</section>

</div>