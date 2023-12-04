---
layout: page
title: Test
subtitle: Interactive map
---
 

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
