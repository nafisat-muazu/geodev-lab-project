# My Project Brief

## The Question

Which primary health centers in Kogi State are located within 5km of a river and are therefore at higher risk of flood related disruption?

## The Data I Need and the Source Link
Nigeria administrative boundary (NGA_admin1): https://data.humdata.org/dataset/cod-ab-nga
GRID3 NGA Health Facilities: https://data.humdata.org/dataset/grid3-nga-health-facilities-v2-0
Waterways_lines shapefile (hotosm_nga_waterways_lines):  https://data.humdata.org/dataset/bfc37dc6-42da-4334-9d4b-bd37d3916306

# Method
Load the Nigeria boundary, health facility points and river lines into QGIS.
Extracted Kogi State from the Nigeria boundary.
Clip the health facility and river layers to the Kogi State boundary.
Create a 5km buffer around the river layer.
Run a spatial join to select health facilities that fall within the 5km buffer.
Symbolize the output: facilities within 5km of a river in red (at risk) and facilities outside the buffer in black (safe).

# Result
A map showing primary health centers across Kogi State split into two categories: those within 5km of a river (flagged red as at risk) and those beyond 5km
(shown in black as safe). This gives Geodev Lab Africa and Kogi State health stakeholders a quick visual reference for facilities that may need flood contingency planning.
