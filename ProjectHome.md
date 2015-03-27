This project is split up into three parts:

# P0 - Tools #
Based on libmpr there will be some tools (or "a tool") to easily extract and calibrate small, single GroundOverlays for Google Earth.

# P1 - Server based #
Some tools will be provided to transform the mpr-Maps to Google Earth readable files (PNG, GIF or JPG), calibrate them (because Austrian-TOPO Maps are not in WGS84), generate Superoverlay-kml-files and copy them into a directory structure in your webserver. (Version 1 will use a database, Apache and PHP, version 2 will be only on harddisk; also local harddisk possible)

# P2 - Local usage #
A little C++ Webserver with libmpr and some png-library included gets the KML- and Map-image-requests from Google Earth, reads the corresponding map-parts from the Austrian-Map-CD, transforms them to PNG, JPG or GIF pictures and returns them immediately to Google Earth. (Version 2 will have a Cache for the generated pictures)


# Future Use #
Maybe we can get this project work with all type of maps (mainly for those which are not WGS84, and those with the .mpr / .mph map-files) like the German TOP50, etc...