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
<select id="variableSelectTIV">
    <option value="CG400_X_F2_F2_TIV_adj">400m</option>
    <option value="CG500_X_F2_F2_TIV_adj">500m</option>
    <option value="CG600_X_F2_F2_TIV_adj">600m</option>
    <option value="CG800_X_F2_F2_TIV_adj">800m</option>
</select>

<!-- Container to display the map -->
<div id="mapContainerTIV"></div>

<!-- Script to handle map display based on user selection -->
<script>
    function displayMapTIV() {
        var selectedVariableTIV = document.getElementById("variableSelectTIV").value;
        
        // Code to display the map based on the selectedVariable
        var iframeTIV = document.createElement('iframe');
        iframeTIV.src = "maps/map_points_" + selectedVariableTIV + ".html";
        iframeTIV.width = "90%";
        iframeTIV.height = "400px";
        
        // Replace the content of mapContainer with the updated map
        var mapContainerTIV = document.getElementById("mapContainerTIV");
        mapContainerTIV.innerHTML = '';
        mapContainerTIV.appendChild(iframe);
    }

    document.getElementById("variableSelectTIV").addEventListener("change", displayMap);

    displayMapTIV();
</script>


<!
### Density map Right Accumbens

**Spatial lag selection**
<select id="variableSelectGRA">
    <option value="CG400_X_F2_F2_RightAccumbensArea_adj">400m</option>
    <option value="CG500_X_F2_F2_RightAccumbensArea_adj">500m</option>
    <option value="CG600_X_F2_F2_RightAccumbensArea_adj">600m</option>
    <option value="CG800_X_F2_F2_RightAccumbensArea_adj">800m</option>
</select>

<!-- Container to display the map -->
<div id="mapContainerGRA"></div>

<!-- Script to handle map display based on user selection -->
<script>
    function displayMapGRA() {
        var selectedVariableGRA = document.getElementById("variableSelectGRA").value;
        
        // Code to display the map based on the selectedVariable
        var iframeGRA = document.createElement('iframe');
        iframeGRA.src = "maps/map_density_" + selectedVariableGRA + ".html";
        iframeGRA.width = "90%";
        iframeGRA.height = "400px";
        
        // Replace the content of mapContainer with the updated map
        var mapContainerGRA = document.getElementById("mapContainerGRA");
        mapContainerGRA.innerHTML = '';
        mapContainerGRA.appendChild(iframe);
    }

    document.getElementById("variableSelectGRA").addEventListener("change", displayMapGRA);

    displayMapGRA();
</script>

### Density map Left Accumbens

**Spatial lag selection**
<select id="variableSelectGLA">
    <option value="CG400_X_F2_F2_LeftAccumbensArea_adj">400m</option>
    <option value="CG500_X_F2_F2_LeftAccumbensArea_adj">500m</option>
    <option value="CG600_X_F2_F2_LeftAccumbensArea_adj">600m</option>
    <option value="CG800_X_F2_F2_LeftAccumbensArea_adj">800m</option>
</select>

<!-- Container to display the map -->
<div id="mapContainer"></div>

<!-- Script to handle map display based on user selection -->
<script>
    function displayMap() {
        var selectedVariableGLA = document.getElementById("variableSelectGLA").value;
        
        // Code to display the map based on the selectedVariable
        var iframe = document.createElement('iframe');
        iframe.src = "maps/map_density_" + selectedVariableGLA + ".html";
        iframe.width = "90%";
        iframe.height = "400px";
        
        // Replace the content of mapContainer with the updated map
        var mapContainer = document.getElementById("mapContainer");
        mapContainer.innerHTML = '';
        mapContainer.appendChild(iframe);
    }

    document.getElementById("variableSelectGLA").addEventListener("change", displayMap);

    displayMap();
</script>


### Density map Right Subcallosal area

**Spatial lag selection**
<select id="variableSelect">
    <option value="CG400_X_F2_F2_RightSCASubcallosalArea_adj">400m</option>
    <option value="CG500_X_F2_F2_RightSCASubcallosalArea_adj">500m</option>
    <option value="CG600_X_F2_F2_RightSCASubcallosalArea_adj">600m</option>
    <option value="CG800_X_F2_F2_RightSCASubcallosalArea_adj">800m</option>
</select>

<!-- Container to display the map -->
<div id="mapContainer"></div>

<!-- Script to handle map display based on user selection -->
<script>
    function displayMap() {
        var selectedVariable = document.getElementById("variableSelect").value;
        
        // Code to display the map based on the selectedVariable
        var iframe = document.createElement('iframe');
        iframe.src = "maps/map_density_" + selectedVariable + ".html";
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
<select id="variableSelect">
    <option value="CG400_X_F2_F2_LeftSCASubcallosalArea_adj">400m</option>
    <option value="CG500_X_F2_F2_LeftSCASubcallosalArea_adj">500m</option>
    <option value="CG600_X_F2_F2_LeftSCASubcallosalArea_adj">600m</option>
    <option value="CG800_X_F2_F2_LeftSCASubcallosalArea_adj">800m</option>
</select>

<!-- Container to display the map -->
<div id="mapContainer"></div>

<!-- Script to handle map display based on user selection -->
<script>
    function displayMap() {
        var selectedVariable = document.getElementById("variableSelect").value;
        
        // Code to display the map based on the selectedVariable
        var iframe = document.createElement('iframe');
        iframe.src = "maps/map_density_" + selectedVariable + ".html";
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


## Maps visualization: LISA

### Density map Right Accumbens

**Spatial lag selection**
<select id="variableSelect">
    <option value="CG400_X_F2_F2_RightAccumbensArea_adj">400m</option>
    <option value="CG500_X_F2_F2_RightAccumbensArea_adj">500m</option>
    <option value="CG600_X_F2_F2_RightAccumbensArea_adj">600m</option>
    <option value="CG800_X_F2_F2_RightAccumbensArea_adj">800m</option>
</select>

<!-- Container to display the map -->
<div id="mapContainer"></div>

<!-- Script to handle map display based on user selection -->
<script>
    function displayMap() {
        var selectedVariable = document.getElementById("variableSelect").value;
        
        // Code to display the map based on the selectedVariable
        var iframe = document.createElement('iframe');
        iframe.src = "maps/LISA_map_density_" + selectedVariable + ".html";
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

### Density map Left Accumbens

**Spatial lag selection**
<select id="variableSelect">
    <option value="CG400_X_F2_F2_LeftAccumbensArea_adj">400m</option>
    <option value="CG500_X_F2_F2_LeftAccumbensArea_adj">500m</option>
    <option value="CG600_X_F2_F2_LeftAccumbensArea_adj">600m</option>
    <option value="CG800_X_F2_F2_LeftAccumbensArea_adj">800m</option>
</select>

<!-- Container to display the map -->
<div id="mapContainer"></div>

<!-- Script to handle map display based on user selection -->
<script>
    function displayMap() {
        var selectedVariable = document.getElementById("variableSelect").value;
        
        // Code to display the map based on the selectedVariable
        var iframe = document.createElement('iframe');
        iframe.src = "maps/LISA_map_density_" + selectedVariable + ".html";
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


### Density map Right Subcallosal area

**Spatial lag selection**
<select id="variableSelect">
    <option value="CG400_X_F2_F2_RightSCASubcallosalArea_adj">400m</option>
    <option value="CG500_X_F2_F2_RightSCASubcallosalArea_adj">500m</option>
    <option value="CG600_X_F2_F2_RightSCASubcallosalArea_adj">600m</option>
    <option value="CG800_X_F2_F2_RightSCASubcallosalArea_adj">800m</option>
</select>

<!-- Container to display the map -->
<div id="mapContainer"></div>

<!-- Script to handle map display based on user selection -->
<script>
    function displayMap() {
        var selectedVariable = document.getElementById("variableSelect").value;
        
        // Code to display the map based on the selectedVariable
        var iframe = document.createElement('iframe');
        iframe.src = "maps/LISA_map_density_" + selectedVariable + ".html";
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
<select id="variableSelect">
    <option value="CG400_X_F2_F2_LeftSCASubcallosalArea_adj">400m</option>
    <option value="CG500_X_F2_F2_LeftSCASubcallosalArea_adj">500m</option>
    <option value="CG600_X_F2_F2_LeftSCASubcallosalArea_adj">600m</option>
    <option value="CG800_X_F2_F2_LeftSCASubcallosalArea_adj">800m</option>
</select>

<!-- Container to display the map -->
<div id="mapContainer"></div>

<!-- Script to handle map display based on user selection -->
<script>
    function displayMap() {
        var selectedVariable = document.getElementById("variableSelect").value;
        
        // Code to display the map based on the selectedVariable
        var iframe = document.createElement('iframe');
        iframe.src = "maps/LISA_map_density_" + selectedVariable + ".html";
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
>
