---
layout: post
title: GIS for Community Archival Access
description:
image:
nav-menu: false
permalink: /GIS-for_CommArch/
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
		  <p>I categorize cartographic records (maps, aerial photographs) and photographic records of places according to their elevation relative to human ground-level perspective. This yields three categories: <b>ground-level imagery</b>, <b>low oblique aerial imagery</b>, and <b>vertical aerial imagery</b>. This project explores GIS-based solutions to make such materials from the <a href="https://www.westonhistoricalsociety.ca/" target="blank">Weston Historical Society</a>’s community archive publicly accessible, with minimal computational demands and technical skill requirements.</p>
		  <!--Buttons-->
		  <ul class="actions small">
				<li><a href="#Linked" class="button small">Linked Photos</a></li>
				<li><a href="#Oblique" class="button small">Oblique Aerial Photos</a></li>
				<li><a href="#Web" class="button small">Web GIS and Google Earth</a></li>
				<li><a href="#Spatial" class="button small">Spatial Recontextualization</a></li>
				<li><a href="#Data" class="button small">Info.</a></li>
		  </ul>
	
      <!-- Content -->
      <div class="row">
		<!-- Left column -->
        <div class="6u 12u$(small)">
          <!--Rest of the overview-->
		  <section id="Linked" style="scroll-margin-top:80px;">
		  <br>
		  <h4 style="color:#8ED530">1. Spatially Linked Photos with Reconstructed Perspectives</h4>
		  <p>Due to urban changes, locations depicted in ground-level photographs are often difficult to recognize. To address this, I created a point layer representing approximate camera positions, each annotated with azimuth (the angle relative to geographic north), a hyperlink to the image, and a second link to its archival record. The points are visualized as directional arrows indicating both location and viewing angle. Using HTML-coded map tips, I enabled thumbnail popups that appear on hover, each linked to the full archival record online.</p>
		  <ul class="actions fit">
			<li><a href="https://qgiscloud.com/pouyan_s/Weston_Landscp_with_Camera_POV/?fbclid=IwY2xjawNwgOhleHRuA2FlbQIxMABicmlkETFwbGVOU2NkNE9lZkhkMmJrAR7MbkEFXmi8fpNo0BxvkHqIxUAjSK8w3foWqprEe-P570d3ndRmtvE5ix0Opg_aem_kPSGgX1KAhsfJI6nNDCAGw&l=Weston%20%E2%80%94%20toronto_crs84%2CCamera%20POV_Weston%20landscape%2Clandmarks_of_weston%2CEsri%20World%20Imagery&bl=mapnik&t=Weston_Landscp_with_Camera_POV" class="button" style="background-color:#8ED530; color:black;">Explore the Annotated Web Map</a></li>
		  </ul>
		  </section>
		  <section id="Oblique" style="scroll-margin-top:80px;">
		  <h4 style="color:#8ED530">2. Georeferencing Oblique Aerial Imagery and Footage via 3D Mapping</h4>
		  <p>Tilted aerial photographs and footage that exclude the horizon are known as low oblique aerial imagery. When georeferenced onto horizontal 2D maps, these images often appear so distorted that they become spatially unusable. To correct this, I manually adjust their orientation within QGIS’s 3D scene, so that vertical elements appear visually upright and corners approximate right angles—a manual-visual rectification process.</p>
		  <br>
		  <p>Using a swipe tool, the resulting georeferenced historical imagery can be compared with satellite imagery or with the current map. This example shows a historical oblique aerial photo of Weston (York, Ontario), which I georeferenced and manually rectified in a 3D QGIS scene using both visual and spatial cues.</p>
		  <br><br>
		  <p>The same procedure applies to frames extracted from oblique aerial footage:</p>
		  <img src="{% link assets/images/04_GIS_for_CommArch/7.48.2025_ISF_OBLQ_1956_02.png %}" alt="" data-position="top center" />
		  <p style="text-align:center; font-size:12px;"> A Georeferenced frame from Oblique Aerial footage via 3D Mapping</p>
		  </section>
		  <section id="Web" style="scroll-margin-top:80px;">
		  <h4 style="color:#8ED530">3. From Archives to Access: Historical Maps and Aerials in Web GIS and Google Earth</h4>
		  <p>Historical maps and vertical aerial photographs often remain inaccessible to the general public unless they are visualized within a spatial context that users can recognize. In this project, my goal was to bring such archival materials back to life by aligning them with their corresponding locations on modern maps.</p><p>I used two strategies to accomplish this. First, after georeferencing the maps and aerials in QGIS, I published the resulting layers to QGIS Cloud and shared the web map link with members of the Weston Historical Society via <a href="https://www.facebook.com/groups/565520831292199" target="blank">their public Facebook group</a>. Second, to support more personal and offline use, I converted the georeferenced layers into KMZ (Keyhole Markup Language Zipped) files. Users can simply drag and drop these files into Google Earth Pro (desktop) or Google Earth Web, where the historical imagery appears as a spatially accurate overlay on the modern basemap.</p>
		  </section>
		  <br><br><br><br>
		  <section id="Spatial" style="scroll-margin-top:80px;">
		  <h4 style="color:#8ED530">4. Historical Spatial Recontextualization with Archival Maps and Aerial Photographs (Diachronic Spatial Simulation)</h4>
		  <p>This project explores how a present-day walk unfolds across historical geographies by anchoring the temporal experience while recontextualizing spatial surroundings. Using archival vertical aerial photographs and historical maps, I project a single temporal event—the walk—onto multiple spatial frames. The result is a diachronic spatial shift: the temporal anchor (the relative time intervals within the GPS track) remains constant, while the geographic context changes.</p><p>A side-by-side animated map of the same walk across two historical eras allows viewers to observe spatial transformations over time. To create this, I recorded GPS data during a walk in the Weston neighborhood (York, Ontario). In QGIS, I animated the GPS trajectory in two parallel maps: one using a current basemap, and one using a georeferenced historical aerial photograph of the same area.</p>
		  </section>
		</div>
		<!-- Right column -->
        <div class="6u$ 12u$(small)">
		<br>
			<div style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden;">
			  <iframe src="https://www.youtube-nocookie.com/embed/QRXXntgGggk"
					  title="YouTube video player"
					  frameborder="0"
					  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
					  allowfullscreen
					  style="position:absolute; top:0; left:0; width:100%; height:100%;">
			  </iframe>
			</div>
		  <p style="text-align:center; font-size:12px;">Hovering over the directional arrows—indicating camera location and angle—reveals a thumbnail of the corresponding historical photo, linked to its archival record. <a href="https://qgiscloud.com/pouyan_s/Weston_Landscp_with_Camera_POV/?fbclid=IwY2xjawNwgOhleHRuA2FlbQIxMABicmlkETFwbGVOU2NkNE9lZkhkMmJrAR7MbkEFXmi8fpNo0BxvkHqIxUAjSK8w3foWqprEe-P570d3ndRmtvE5ix0Opg_aem_kPSGgX1KAhsfJI6nNDCAGw&l=Weston%20%E2%80%94%20toronto_crs84%2CCamera%20POV_Weston%20landscape%2Clandmarks_of_weston%2CEsri%20World%20Imagery&bl=mapnik&t=Weston_Landscp_with_Camera_POV&e=-8853866%2C5418622%2C-8851157%2C5420601">Explore the Annotated Web Map.</a></p>
		  <br><br><br>
		  <div style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden;">
			  <iframe src="https://www.youtube-nocookie.com/embed/CSTp_skozgQ"
					  title="YouTube video player"
					  frameborder="0"
					  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
					  allowfullscreen
					  style="position:absolute; top:0; left:0; width:100%; height:100%;">
			  </iframe>
			</div>
		  <p style="text-align:center; font-size:12px;">Georeferencing Oblique Aerial Imagery via 3D Mapping</p>
		  <div style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden;">
			  <iframe src="https://www.youtube-nocookie.com/embed/-w7pe8xkvkE"
					  title="YouTube video player"
					  frameborder="0"
					  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
					  allowfullscreen
					  style="position:absolute; top:0; left:0; width:100%; height:100%;">
			  </iframe>
			</div>
			<br>
			<div style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden;">
			  <iframe src="https://www.youtube-nocookie.com/embed/70Q6yW9Yr98"
					  title="YouTube video player"
					  frameborder="0"
					  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
					  allowfullscreen
					  style="position:absolute; top:0; left:0; width:100%; height:100%;">
			  </iframe>
			</div>
			<p style="text-align:center; font-size:12px;">Georeferencing frames from Oblique Aerial footage via 3D Mapping</p>
			<br><br>
			<div style="position:relative; padding-bottom:110%; height:0; overflow:hidden;">
			  <iframe	src="https://qgiscloud.com/pouyan_s/Weston_York_Ontario_1910/?fbclid=IwY2xjawNvH69leHRuA2FlbQIxMQABHv5w62v01Uxlu2dYKCuexv76mgWP_DWtqFMFn0lwxw9PFlLoys8PKjTQZgMG_aem_JVsBLBWxMeKG8CWkp-OZ3A&l=Heritage%20Register__Weston%20York%20ON%2CWeston%20York%20ON__Boundaries%2C1910%20Map%20of%20Weston__Plate%2080%20a%2C1910%20Map%20of%20Weston__Plate%2079%2C1910%20Map%20of%20Weston__Plate%2080%20b&bl=mapnik&t=Weston_York_Ontario_1910&e=-8855203%2C5416988%2C-8848429%2C5421936"
				title="QGIS Cloud Map"
				frameborder="0"
				allowfullscreen
				style="position:absolute; top:0; left:0; width:100%; height:100%;"
			  ></iframe>
			</div>
			<p style="text-align:center; font-size:12px;">The 1910 map of Weston (York, Ontario), from Goad’s Atlas of the City of Toronto and Suburbs, georeferenced and visualized alongside the neighborhood’s current boundaries and designated cultural heritage properties. Explore the interactive map directly here or <a href="https://qgiscloud.com/pouyan_s/Weston_York_Ontario_1910/?fbclid=IwY2xjawNvH69leHRuA2FlbQIxMQABHv5w62v01Uxlu2dYKCuexv76mgWP_DWtqFMFn0lwxw9PFlLoys8PKjTQZgMG_aem_JVsBLBWxMeKG8CWkp-OZ3A&l=Heritage%20Register__Weston%20York%20ON%2CWeston%20York%20ON__Boundaries%2C1910%20Map%20of%20Weston__Plate%2080%20a%2C1910%20Map%20of%20Weston__Plate%2079%2C1910%20Map%20of%20Weston__Plate%2080%20b&bl=mapnik&t=Weston_York_Ontario_1910&e=-8855203%2C5416988%2C-8848429%2C5421936" target="blank">use this link</a>.</p>
			<br><br><br>
			<div style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden;">
			  <iframe 
				src="https://www.youtube-nocookie.com/embed/xLn4bC9W8_w"
				title="YouTube video player"
				frameborder="0"
				allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
				allowfullscreen
				style="position:absolute; top:0; left:0; width:100%; height:100%;">
			  </iframe>
			</div>
        </div>
      </div>
	  <hr>
	  <section id="Data" style="scroll-margin-top:80px;">
	  <!-- Software-->
		<h4 style="color:#8ED530">Software</h4><p>QGIS 3.4, QGIS Cloud</p>
	  <!-- Data-->
		<h4 style="color:#8ED530">Data</h4>
		<ul>
			<li><span style="color:#E0115F; font-weight:bold;">Historical maps</span></li>
			<li><span style="color:#E0115F; font-weight:bold;">vertical aerial photographs</span></li>
			<li><span style="color:#E0115F; font-weight:bold;">oblique aerial imagery and footage</span></li>
			<li><span style="color:#E0115F; font-weight:bold;">ground-level archival photographs</span></li>
			<li><span style="color:#E0115F; font-weight:bold;">GPS trajectory data</span></li>
			<li><span style="color:#E0115F; font-weight:bold;">modern basemaps</span></li>
			<li><span style="color:#E0115F; font-weight:bold;">structured CSV tables</span></li>
			<li><span style="color:#E0115F; font-weight:bold;">georeferenced raster layers</span></li>
		</ul>
		<!-- Skills -->
		<h4 style="color:#8ED530">Skills used</h4><p>Spatial data creation and annotation, Vector data creation, Georeferencing and spatial alignment (raster imagery), Oblique imagery rectification, Point layer creation from CSV, Temporal data structuring and encoding, GPS trajectory integration, Temporal-spatial animation, Time-enabled map creation, 3D scene construction and perspective correction, Interactive map tip design (HTML-based), Swipe tool integration, Metadata linking and captioning, Web GIS publishing and deployment via QGIS Cloud, KMZ file preparation for Google Earth, Audience adaptation, User-centered design for accessibility, Photogrammetric reasoning and spatial inference</p>
		</section>
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

