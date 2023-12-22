---
layout: home
title: Lausanne Brain Atlas
subtitle: An exploratory analysis of brain structure and environmental parameters
cover-img: "/assets/img/temp.webp"
---

## Motivation

&nbsp;&nbsp;&nbsp;&nbsp; Our brain is our most specialized organ and it is responsible for the complex sensory perception of our environment. But those 14-16 billion neurons are in fact quite fragile and prone to multiple diseases and cortical thinning. Pesticides, air pollutants, metal accumultaion or excessive noise were all shown to have a negative impact during the brain development or during adulthood. 

&nbsp;&nbsp;&nbsp;&nbsp; In this context, it is important to explore the relationships between the brain structure and its environment. This can be achieved by analyzing spatial trends in brain regions volume variations over maps. With the help of those tools, a better visual grasp and comprehension of the spatiality allows for a further investigation of a potential link to an environmental variable.

## Goal

&nbsp;&nbsp;&nbsp;&nbsp; This project aims to build an atlas of the brain structure in Lausanne, helping in the vizualization of otherwise opaque data. Its second goal is to demonstrate a type of analysis making use of this data with the case of heavy metals and their ties with neurodegenaration.

## Literature review

Review on ties between brain and environmental factors in the litterature

## Dataset description

&nbsp;&nbsp;&nbsp;&nbsp; Lorem


## Maps visualization: Getis 

### Density map
<iframe src="maps/map_dense.html" width="100%" height="500px"></iframe>

### Point map
<iframe src="maps/map_points.html" width="100%" height="500px"></iframe>



### Interactive TIV point map test

**Spatial lag selection**
<select id="variableSelect">
    <option value="CG400_X_F2_F2_TIV_adj">400m</option>
    <option value="CG500_X_F2_F2_TIV_adj">500m</option>
    <option value="CG600_X_F2_F2_TIV_adj">600m</option>
    <option value="CG800_X_F2_F2_TIV_adj">800m</option>
</select>

<!-- Container to display the map -->
<div id="mapContainer"></div>

<!-- Script to handle map display based on user selection -->
<script>
    function displayMap() {
        var selectedVariable = document.getElementById("variableSelect").value;
        
        // Code to display the map based on the selectedVariable
        var iframe = document.createElement('iframe');
        iframe.src = "maps/map_points_" + selectedVariable + ".html";
        iframe.width = "90%";
        iframe.height = "400px";
        
        // Replace the content of mapContainer with the updated map
        var mapContainer = document.getElementById("mapContainer");
        mapContainer.innerHTML = '';
        mapContainer.appendChild(iframe);
    }

    document.getElementById("variableSelect").addEventListener("change", displayMap);

    displayMap();
</script>



### Density map Left Subcallosal area

**Spatial lag selection**
<select id="variableSelect1">
    <option value="CL400_X_F2_F2_LeftSCASubcallosalArea_adj">400m</option>
    <option value="CL500_X_F2_F2_LeftSCASubcallosalArea_adj">500m</option>
    <option value="CL600_X_F2_F2_LeftSCASubcallosalArea_adj">600m</option>
    <option value="CL800_X_F2_F2_LeftSCASubcallosalArea_adj">800m</option>
</select>

<!-- Container to display the map -->
<div id="mapContainer1"></div>

<!-- Script to handle map display based on user selection -->
<script>
    function displayMap1() {
        var selectedVariable = document.getElementById("variableSelect1").value;
        
        // Code to display the map based on the selectedVariable
        var iframe = document.createElement('iframe');
        iframe.src = "maps/LISA_map_density_" + selectedVariable + ".html";
        iframe.width = "90%";
        iframe.height = "400px";
        
        // Replace the content of mapContainer with the updated map
        var mapContainer = document.getElementById("mapContainer1");
        mapContainer.innerHTML = '';
        mapContainer.appendChild(iframe);
    }

    document.getElementById("variableSelect1").addEventListener("change", displayMap1);

    displayMap1();
</script>


<style>
.myDiv {
  width: 100%;
  height: 1000px;
  padding: 10px;
  border: 5px solid gray;
  margin: 0;
}
</style>

<div class="myDiv">
    <div class="timeline">
      <div class="container left">
        <div class="content">
          <h2>2017</h2>
          <p>Lorem ipsum..</p>
        </div>
      </div>
      <div class="container right">
        <div class="content">
          <h2>2016</h2>
          <p>Lorem ipsum..</p>
        </div>
      </div>
    </div>
</div>
