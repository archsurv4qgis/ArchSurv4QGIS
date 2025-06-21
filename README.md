ArchSurv4QGIS (AS4QGIS) is an open source solution for automated archaeological feature drawings from in-field GNSS / totalstation point measurements via QGIS.

It is designed as an adjustable ".model3" algorithm pipeline.

------------------------------------------------------------------

What is ArchSurv4QGIS?
AS4QGIS works on the basis of point data exported as delimited text from a surveying device. 

ArchSurv4QGIS processes 10-character pointID-strings: e. g. '0001A03001'
- feature '1'
- line container / point property 'A'
- shape type '03'
- sequence number '001'


Depending on the entered "shape type", AS4QGIS generates four output datasets:
- polygons.shp
- polylines.shp
- pointdata.shp
- vertices.shp


shape type spectrum:
feature | '01' - heights, '02' - polyline, '03' - polygon, '33' - closed polyline
sample | '51' - sample point, '52' - sample polyline, '53' - sample polygon
posthole | '06' / '61' - buffered point measurement
finds | '71' - find point, '72' - find polyline, '73' - find polygon
3D markers | '81' - 3D marker point
trench | '91' - fixed point, '92' - trench polyline, '93' trench polygon
section nails | '00' - section nail point


Three distinct variations of the same algorithm pipeline are available:

1 | Archimedes

2 | Chronos

3 | Chimaira


AS4QGIS is free to use and fully customizable.
