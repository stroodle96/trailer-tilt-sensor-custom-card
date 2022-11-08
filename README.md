<!---                 [![hacs_badge](https://img.shields.io/badge/HACS-Custom-41BDF5.svg)](https://github.com/hacs/integration)              --->
# trailer-tilt-sensor-custom-card
Custom home assistant lovelace card showing tilt of trailer.

This is a fork of the [Van tilt card by @CF209](https://github.com/CF209/van-tilt-sensor-custom-card).  I modified it to be for Travel Trailers. 

# Installation
To install the card, create a new folder in your "homeassistant/www/" directory called "trailer-tilt-card" and download the files to this directory. Then in Home Assistant go to Configuration - Lovelace Dashboards - Resources and click "Add Resource". Enter "/local/trailer-tilt-card/trailer-tilt-card.js" for the URL and "JavaScript Module" for the type and click create. Back in your main dashboard, you can now manually add the new card with the following code:

type: 'custom:trailer-tilt-card'<br>
entity_x: sensor.tt_filtered_x_angle<br>
entity_y: sensor.tt_filtered_y_angle<br>

![alt text](https://github.com/stroodle96/trailer-tilt-sensor-custom-card/blob/main/img/card_screenshot.png)
