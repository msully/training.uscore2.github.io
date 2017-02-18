---
title: Amadora city - Portugal
layout: partners
country: Portugal
website: www.facebook.com/amadora.resiliente
size: 24 sq km
population:
- year: 2011
- total: 175575
hazards: Earthquake, Flood, Heat Wave, Land Slide, Technical Disaster
description: The major disaster risks were flash floods (urban area),urban fires,
  industrial fires, landslides, storms (fallen trees, damaged buildings infrastructure)
  and road accidents. Amadora municipality has some vulnerability a highly urbanized
  territory and population insufficiently aware and/or sensitized about the risks
  and hazards.
image: "/images/amandora.png"
map:
  latitude: 38.7417991
  longitude: -9.2224606
  address: " Amadora, Portugal"
  zoom: 10
---

<div class="map" id="map"></div>

<section class="testimonial">
		<div class="container flex">
			<div class="testimonial-block">
				<blockquote>
					<p class="editable">The risks are a biophysical fragility of the territory. Their impact on the infrastructures and population involve a strong strategy. Preparedness, mitigation, prevention are the key of success. Our task is promote a campaign with maximum possible number of agents from the local,scientific and academic communities, demonstrating the relevance of risk reduction and of the amount of natural disasters that afflict the territory.</p>
					<p class="editable">Carla Tavares, MAYOR</p>
				</blockquote>
			</div>
		</div>
	</section>

## HAZARD AND VULNERABILITY PROFILE 

The major disaster risks were flash floods (urban area), urban fires, industrial fires, landslides, storms (fallen trees, damaged buildings infrastructure) and road accidents. Amadora municipality has some vulnerability: a highly urbanized territory and population insufficiently aware and/or sensitized about the risks and hazards. 

![alt text](/images/amandora.png "Amadora - Portugal")

## DISASTER AND RISK REDUCTION ACTIVITIES 

In the context of the preparation, it is worth mentioning the training and awareness creation project for the school community, entitled "Civil Protection Club", which addresses the issues of risks that exist in Amadora (e.g., seismic risk, flood areas, etc.) and identifies the self-protection measures. It is worth noting that there has been a continued effort towards a culture of safety and prevention creating in Amadora. The local institutions have made remarkable efforts to reduce the vulnerability of the population by issuing warnings not to occupy areas of risk. The planning for the seismic risk and the mapping of the flood areas, are also good examples of such efforts, including the risk analyses (zoning of critical areas) and planning for emergency situations. The whole structure of civil protection has made remarkable efforts to involve a great number of institutional partners from both civic and scientific academic spheres of life.

<script type="text/javascript">
	window.mapData = {{ page.map | jsonify }};

	function initMap() {
		var myOptions = {
			scrollwheel: false,
			draggable: false,
			panControl: false,
			disableDefaultUI: true,
			zoom: window.mapData.zoom,
			maxZoom: window.mapData.zoom,
			minZoom: window.mapData.zoom,
			center: new google.maps.LatLng(window.mapData.latitude, window.mapData.longitude),
			mapTypeId: google.maps.MapTypeId.ROADMAP
		};
		map = new google.maps.Map(document.getElementById("map"), myOptions);
		marker = new google.maps.Marker({
			map: map,
			position: new google.maps.LatLng(window.mapData.latitude, window.mapData.longitude)
		});

		google.maps.event.addDomListener(window, "resize", function () {
			map.setCenter(myOptions.center);
		});
	}
</script>

<script async defer src="https://maps.googleapis.com/maps/api/js?key={{ site.google_maps_javascript_api_key }}&amp;callback=initMap"></script>