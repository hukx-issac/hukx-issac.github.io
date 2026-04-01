---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a researcher in generative recommendation and sequential behavior modeling. I received my Ph.D. from Wuhan University of Technology in June 2024, under the supervision of Prof. Lin Li. During 2022–2023, I was a visiting Ph.D. student at the University of Technology Sydney, supported by the China Scholarship Council (CSC), where I worked with Prof. Guandong Xu on social computing and recommender systems.

## Research Interests
- Sequential Modeling and Behavior Analysis
- Recommender Systems
- Multimodal Machine Learning
- Social Computing


## Education Experience
- Ph.D. in Computer Science, Wuhan University of Technology, China, 2019–2024  
- Visiting Ph.D. Student in Computer Science, University of Technology Sydney, Australia, 2023–2024 (supported by the China Scholarship Council, CSC)
- M.Eng. in Control Engineering, Chongqing University, China, 2015–2018  
- B.Eng. in Automation, Hubei University of Automotive Technology, China, 2011–2015 

## Working Experience
- Lecturer, School of Computer Science and Artificial Intelligence, Wuhan Textile University, China, 2024–Present
- Data Mining Algorithm Engineer, CETC Big Data Research Institute Co., Ltd., China, 2018–2019

## Selected Places I Have Visited

<div id="travel-map" style="height: 460px; width: 100%; margin-top: 1em;"></div>

<link
  rel="stylesheet"
  href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
/>
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>

<script>
document.addEventListener("DOMContentLoaded", function () {
  var map = L.map("travel-map").setView([30.5928, 114.3055], 3);

  L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
    maxZoom: 18,
    attribution: '&copy; OpenStreetMap contributors'
  }).addTo(map);

  var places = [
    {name: "Wuhan, China", coords: [30.5928, 114.3055], note: "Current location / work"},
    {name: "Chongqing, China", coords: [29.5630, 106.5516]},
    {name: "Shiyan, China", coords: [32.6292, 110.7980]},
    {name: "Sydney, Australia", coords: [-33.8688, 151.2093]},
    {name: "Gifu, Japan", coords: [35.4233, 136.7607]},
    {name: "Tokyo, Japan", coords: [35.6762, 139.6503]},
    {name: "Brisbane, Australia", coords: [-27.4698, 153.0251]},
    {name: "Guiyang, China",coords: [26.6470, 106.6302]},
    {name: "Hong Kong, China", coords: [22.3193, 114.1694]}
    ];

  places.forEach(function (place) {
    L.marker(place.coords)
      .addTo(map)
      .bindPopup("<b>" + place.name + "</b>");
  });
});
</script>