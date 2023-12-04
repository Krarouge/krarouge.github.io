---
layout: home
title: Geobrain project Lausanne
subtitle: Providing an atlas of the brain in Lausanne
cover-img: "/assets/img/temp.webp"
---

## Motivation

&nbsp;&nbsp;&nbsp;&nbsp; Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. 

&nbsp;&nbsp;&nbsp;&nbsp; Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

## Goal

&nbsp;&nbsp;&nbsp;&nbsp; This project aims to ...

## Research questions

- What are the goals ?

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
