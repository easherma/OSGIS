# Loading from Databases

## Database Connections

## PostGIS
Clicking on "Watch file" -- e.g. if you have the file open in another
window, QGIS will automatically update the version

* Working with Postgres

o We downloaded PostgreSQL from enterprisedb.com o The name "PostgreSQL" has its origins in being a system came after the INteractive Graphics REtrieval System ("Ingres") system. Thus "Post-Ingres" or "Postgres" for short, although the official name still is PostgreSQL.

o We have an installed template

o From in QGIS, can click on the +Postgres button (with the elephant) on the left

* We point to our template, port, username and password

* The outcome is that we have established a connection and can access the information here (although we only have a template schema so far, and not data!)

o Now, when we save layers, we can save it to our DB

* E.g., reproject a layer, choose to save it to a database, select the schema and pick a name...

o Within PostGIS we have the ability to index geometries for our layers which speeds recall and query for spatial operations, as compared to a flat file

o When opening a totally new project, the PostGIS connect will persist, and can even bring in its tables

* One consideration though is permissions, where we may or may not want to allow users to make changes to centrally-accessible

o Can use PostGIS scripting for queries, e.g. "SELECT ST_BUFFER(ST_TRANSFORM("geom", 3435), 300) FROM potholes"

* This command reprojects the data, then creates a buffer. Here, we don't need to create something for each intermediate step. In effect, QGIS can then just become a viewer rather than a tool.

* Could also add CREATE TABLE buffer AS (.) around the above to create a new table. Just need to refresh the connection for this to reappear.

* Or, could add SELECT * FROM someothertable WHERE someothertable.geom INTERSECTS (.) to use the buffer as a subquery to an operation that identifies the intersection

* Operations are remarkably fast

* There are ways to install query builder plugins in QGIS to write queries here rather than having to jump out of QGIS and back into PostGIS

## SpatialLite

## GeoPackage
