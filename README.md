Testing if the order of things in XML files is stable in QT6-based QGIS builds.

https://github.com/qgis/QGIS/issues/29192

The files in the repo are:
- `world.qgs`: `world` easter egg's layer loaded in a project, project saved
- `world.qml`: `world` easter egg layer's style exported as QML
- `world.qlr`: `world` easter egg layer exported as QGIS layer definition file

The files were created with:

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0//EN" "http://www.w3.org/TR/REC-html40/strict.dtd">
<html><head><meta http-equiv="Content-Type" content="text/html; charset=utf-8" /></head><body>

QGIS version | 3.38.1-Grenoble | QGIS code branch | Release 3.38
-- | -- | -- | --
Qt version | 5.15.14
Compiled against Python | 3.12.4 | Running against Python | 3.12.5
GDAL/OGR version | 3.9.1
PROJ version | 9.4.1
EPSG Registry database version | v11.006 (2024-03-13)
GEOS version | 3.12.2-CAPI-1.18.2
Compiled against SQLite | 3.46.0 | Running against SQLite | 3.46.1
PDAL version | 2.7.2
PostgreSQL client version | 16.3
SpatiaLite version | 5.1.0
QWT version | 6.3.0
QScintilla2 version | 2.14.1
OS version | Manjaro Linux
  |   |   |
Active Python plugins
plugin_reloader | 0.11
MetaSearch | 0.3.6
db_manager | 0.1.20
grassprovider | 2.12.99
processing | 2.12.99

</body></html>

In the pull requests you can see what other versions of QGIS do to these files. Please feel welcome to add more pull requests for more comparisons if you want. To me it does not seem necessary though.
