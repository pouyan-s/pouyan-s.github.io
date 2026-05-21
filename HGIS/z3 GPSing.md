---
layout: post
title: 'GPSing Historical Travelers: Dynamic Spatiotemporal Mapping and 3D Trajectory Visualization of Sadegh Hedayat’s Isfahan Travel Account'
description: 'Dynamic Spatiotemporal Mapping and 3D Trajectory Visualization of Sadegh Hedayat’s Isfahan Travel Account'
image: 
nav-menu: false
permalink: /GPSing/
---
<!-- Main -->
<div id="main" class="alt">

  <!-- One -->
  <section id="one">
	<!--<ul class="actions fit">
		<li><a href="https://media.dlib.indiana.edu/media_objects/47429z735" target="_blank" class="button fit">Watch my Avicenna map talk</a></li>
		<li><a href="https://iu.maps.arcgis.com/apps/instant/slider/index.html?appid=3923df36605840ca82dfb64d3090db59" target="_blank" class="button fit">Explore the interactive map</a></li>
		<li><a href="https://insights.arcgis.com/#/view/cdc61d577e694380a83d3b1fbb62730e" target="_blank" class="button fit">Explore the  geospatial analysis</a></li>
	</ul>-->
    <div class="inner">
	<!--Overview-->
		  <h4 style="color:#8ED530">Overview</h4>
		  <p><i>Isfahan—half the world</i> (<i>Isfahān nisf-i jahān</i>) is Sadegh Hedayat’s travel account of his brief visit to Isfahan in May 1932. A pioneer of the modern Persian novel, Hedayat documents each step of a journey through a country in transition—from tradition to modernity—offering a perspective uniquely his own.</p>
      <!-- Content -->
      <div class="row">
		<!-- Left column -->
        <div class="6u 12u$(small)">
          <!--Rest of the overview-->
		  <p>This ongoing project draws on the logistical data embedded in Hedayat’s account to reconstruct the dynamics of intercity travel in the early 20th century. I focus on the route, stops, timing, pace, and landscapes described in the text, integrating them into a temporally dynamic map and a 3D scene to offer a spatial and experiential understanding of the journey—especially for readers unfamiliar with the geography and historical context.</p><p>I extracted the times and locations from Hedayat’s account, tracing his path from Rayy (south of Tehran) to Isfahan. I then georeferenced a 1954 historical map of the region that includes the roads he likely traveled. From this, I digitized the relevant road segments, created a point layer along each stretch between his stops, and interpolated travel times based on his reported departure and arrival—producing a dataset that resembles GPS tracking.</p><p>To visualize this movement, I animated the temporal point layer using an SVG icon of a car appropriate to Hedayat’s era. I also constructed a 3D scene using a digital terrain model (DTM) to convey the topography and landscape features that shaped the journey—elements that remain invisible on a 2D map but are essential to understanding the physical and perceptual dimensions of travel in that period.</p>
		  <!-- Software-->
		<h4 style="color:#8ED530">Software</h4><p>QGIS 3.4</p>
		</div>
		<!-- Right column -->
        <div class="6u$ 12u$(small)">
			<div style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden;">
			  <iframe src="https://www.youtube-nocookie.com/embed/jtdcdC9QQB8"
					  title="YouTube video player"
					  frameborder="0"
					  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
					  allowfullscreen
					  style="position:absolute; top:0; left:0; width:100%; height:100%;">
			  </iframe>
			</div>
		  <p style="text-align:center;">Parallel simulation of travel times on Sadegh Hedayat’s twelve-hour road trip from Rayy to Delijan (May 12–13, 1932), visualized on a historical map and satellite image</p>
		  
          <div style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden;">
			  <iframe src="https://www.youtube-nocookie.com/embed/KdZxXQLXEE0"
					  title="YouTube video player"
					  frameborder="0"
					  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
					  allowfullscreen
					  style="position:absolute; top:0; left:0; width:100%; height:100%;">
			  </iframe>
			</div>
		  <p style="text-align:center;">A 3D scene built in QGIS using a digital terrain model (DTM) to convey the topography and landscape features that shaped Sadegh Hedayat’s trip from Rayy to Delijan (Iran)</p>
        </div>
      </div>
	  <!-- Data-->
		<h4 style="color:#8ED530">Data</h4>
		<ul>
			<li><span style="color:#E0115F; font-weight:bold;">Temporal point data</span> in CSV format extracted from a travel account</li>
			<li><span style="color:#E0115F; font-weight:bold;">Raster data</span> of digitized print maps</li>
			<li><span style="color:#E0115F; font-weight:bold;">Temporal line data</span> extracted from georeferenced raster</li>
			<li><span style="color:#E0115F; font-weight:bold;">Digital Terrain Model:</span> Hawker, Luke, et al. <i>FABDEM V1-2: Forest and Buildings Removed Copernicus DEM</i>. University of Bristol, 2022. <a href="https://gee-community-catalog.org/projects/fabdem/">https://gee-community-catalog.org/projects/fabdem/.</a></li>
		</ul>
		<!-- Skills -->
		<h4 style="color:#8ED530">Skills used</h4><p>Textual geolocation parsing (Data extraction from unstructured sources), temporal data modeling, georeferencing historical maps, digitizing analog road networks, feature extraction, point layer creation from CSV, time interpolation, trajectory modeling, temporal animation, SVG icon integration, symbolization, digital terrain model (DTM) integration, 3D scene construction, perspective design, multimodal integration, audience adaptation, metadata and captioning</p>
    </div> <!-- closes .inner -->
  </section> <!-- closes #one -->
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
</div> <!-- closes #main -->

