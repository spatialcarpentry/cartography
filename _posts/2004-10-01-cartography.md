---
title: "Compose a map"
layout: post
category: Show your Results
tags: [cartography, exercise]
tagline: "making print-based maps"
---

{% include JB/setup %}

#### Pre-requisites:

1. Spatial Analysis

#### Objective:

- Create a print-based (static, non-interactive) map in QGIS.

#### Exercise: Map composition

<!--
#### Data:

iRods access: <br>&nbsp;&nbsp;&nbsp;``/iplant/home/shared/Spatial-bootcamp/cartography/compose-a-map``

- [geo_coded.tif](link-to-geo-coded)
- [dem-washington.tif](link-to-dem)
-->
----

#### Create a map of Washington rock strength in QGIS

<ol>
<li>
Import <b>wa_landslide_suscept.tif</b> and <b>wa_hillshade.tif</b> through on of the following methods:<br><br>
iRods:<br>&nbsp;&nbsp;&nbsp;<code>/iplant/home/shared/aegis/Spatial-bootcamp/cartography/compose-a-map/wa_landslide_suscept.tif</code><br><br>&nbsp;&nbsp;&nbsp;<code>/iplant/home/shared/aegis/Spatial-bootcamp/cartography/compose-a-map/wa_hillshade.tif</code><br><br>
Download and <b>Add Raster Layer</b><img src="{{BASE_PATH}}{{ASSET_PATH}}/images/add-raster.png"/>:<br>
<a href="http://de.iplantcollaborative.org/dl/d/F92F0BD2-59A8-4AA0-9B2D-8A3814E636B4/wa_landslide_suscept.tif">wa_landslide_suscept.tif</a><br>
<a href="http://de.iplantcollaborative.org/dl/d/7DAE3EB8-C4B1-4A73-89AE-5E0B90F5E74B/wa_hillshade.tif">wa_hillshade.tif</a><br><br>
These are the same rasters that were created in earlier exercises.<br><br>
<img data-featherlight="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-1.png" src="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-1.png"/>
</li>
<li>Prepare data for composition:<br>
We'll start with <b>wa_geo_coded</b>, be sure this layer is moved to the top of the layer list: <em>Click-hold-drag wa_geo_coded (layer list) above wa_hillshade</em>.<br><br>
<img data-featherlight="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-2.png" src="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-2.png"/>
</li>
<li>Style <b>wa_landslide_suscept</b>:<br>
<ol>
<li>Open <b>wa_geo_coded</b> style properties and select <b>Singleband Pseudocolor</b>.</li>
<li>Import the <b>wa_landslide_suscept.txt</b> color map file from the <b>Landslide exercise</b>. Remember use the <img src="{{BASE_PATH}}{{ASSET_PATH}}/images/add-style.png"/> to import the color map file.<br><br>Or download here: <a href="http://de.iplantcollaborative.org/dl/d/E150205F-323F-4EC0-92CC-B321D7B04101/wa_landslide_suscept.txt">wa_landslide_suscept.txt</a> and import.
<br><br><img data-featherlight="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-3.png" src="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-3.png"/>
<br><br>
Click APPLY and OK once satisfied with the style.<br><br>
<img data-featherlight="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-4.png" src="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-4.png"/>
</li>
<li>
It looks good, but let's make it look better.<br><br>
Increse <b>transparency</b> of <b>wa_geo_coded</b> by opening the wa_geo_coded properties and selecting the <b>Transparency</b> tab. Increase the <b>Global transparency</b> to 50%:<br><br>
<img data-featherlight="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-5.png" src="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-5.png"/><br><br>
Click APPLY and OK to save changes.<br><br>
Much better!<br><br>
</li>
</ol>
</li>
<li>Making the map:<br>
<ol>
<li>Open the <b>Print Composer</b>: <em>Menu Bar > Project > New Print Composer</em></li>
<li>Composing a new map requires a title, enter your title whem prompted.<br><br>
The Print Composer opens in a new application window, you will still be able to work in your current project while making a map.<br><br></li>
<li>You must add a map layer for visualizing. The <b>Add Map</b> tool will require you to create a bounding box to fit the map. Adjust the bounding box as needed.<br><br>
To add a map layer: <em>Menu Bar > Layout > Add Map</em><br><br>
<img data-featherlight="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-6.png" src="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-6.png"/>
</li>
<li>Explore tools by hovering over the toolbar icon or go to <em>Menu Bar > Layout</em> to see the names of each layout tool.</li>
<li>Add a legend: <em>Menu Bar > Layout > Add Legend</em><br><br>
Notice how names and values are not appropriate for a final map. You want to the reader to fully understand what they're reading.<br><br>
<img data-featherlight="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-7.png" src="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-7.png"/><br><br>
Notice the <b>Item Properties</b> tab on the right of the screen. Select an item on the map to activate its properties. Here we are able to make necessary changes such as the legend title, or delete items from the legend.<br><br>
Design the map to however you'd like. See the map below as a reference.<br><br>
Just be sure to consider key elements of a map:<br>
<ol>
<li>Legend</li>
<li>Attribution</li>
<li>Scale</li>
<li>North arrow</li>
</ol>
<img data-featherlight="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-8.png" src="{{BASE_PATH}}{{ASSET_PATH}}/images/compose-8.png"/>
</li>
</ol>
</li>
<li>Export map:<br>
The final step of the process is to export your map to a file, as an Image, PDF, or SVG.<br><br>Decide how you want your map to be shared and select the most appropriate option.<br><br>
<img data-featherlight="{{BASE_PATH}}{{ASSET_PATH}}/images/wa_landslide_suscept.png" src="{{BASE_PATH}}{{ASSET_PATH}}/images/wa_landslide_suscept.png"/>
</li>
</ol>


