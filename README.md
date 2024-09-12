Testing if the order of things in XML files is stable in QT6-based QGIS builds.

https://github.com/qgis/QGIS/issues/29192

The files in the repo are:
- `world.qgs`: `world` easter egg's layer loaded in a project, project saved
- `world.qml`: `world` easter egg layer's style exported as QML
- `world.qlr`: `world` easter egg layer exported as QGIS layer definition file

The files were created with:

QGIS version 3.39.0-Master
QGIS code revision bda5dfd99b
Qt version 6.7.2
Python version 3.12.5
GDAL/OGR version 3.9.1
PROJ version 9.4.1
EPSG Registry database version v11.006 (2024-03-13)
GEOS version 3.12.2-CAPI-1.18.2
SQLite version 3.46.1
PostgreSQL client version No support
SpatiaLite version No support
QWT version 6.3.0
QScintilla2 version 2.14.1
OS version Manjaro Linux

In the pull requests you can see what other versions of QGIS do to these files. Please feel welcome to add more pull requests for more comparisons if you want. To me it does not seem necessary though.
