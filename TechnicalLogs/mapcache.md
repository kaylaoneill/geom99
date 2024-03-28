# MapCache - GeoPackage

## Instal:
- Go to:
- https://ngageoint.github.io/GeoPackage/
- Download for the relevant computer by clicking that computer icon (I did Windows this time)
- Once downloaded, run and install on the local desktop

## Explore
- Click the "+ create project" button
- Name the project (this time did: Testing_week12"
- Click create
- Once open, need to add geopackage file to it: can add from file or Create New
- Did new file this time
- Import in data layers from the computer first (I did not do this first and could not add a feature layer so don't forget this step)
  - For testing, I added a random shp from my computer
  - For some reason, the shapefiles say they have no data attached to them right now. Will need to look into this

- Adding my own data gave me issues so I am trying to download from the Overpass feature download:
  - Name it
  - Specify what content to download: category
  - Specify bounding box- click edit: I did this by drawing on map. Note anything over 10 sq miles can take several minutes or be too large to process. (My first time was too large. The second time I did below 10       but was still too large).
  - ![image](https://github.com/kaylaoneill/geom99/assets/146447016/7b705e1e-4eb3-4bc0-9847-4387ed2044a4)
  - Clip features and buffed: I did 25%
  - Click Import

- Try 3:
  - Instead of searching a whole category, I did tourism="museum" on search
  - Still did not work.
  
- Add feature layer
  - Name it
  - Select the data source (from the data source files that you have uploaded)
  - Order layers (right now we only have 1)
  - Did not set a bounding box filter this time
  - Click add
  - 
