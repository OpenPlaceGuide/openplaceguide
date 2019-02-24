# OpenBusinessMap

OpenBusinessMap will be a free and open source business directory, based on the OpenStreetMap project.
It combines data from the OpenStreetMap project, as well as additional information about businesses.

## User Stories

* As a business owner I want to present my information on a website

* As a business owner I want to control the information shown in the business directory and website

* As a user and business owner I am interested in accurate data in OpenStreetMap.

## Data

### OpenStreetMap

* Name (in all available languages)
* Location data
* Opening Times

### OpenBusinessMap

* All the additional data, see components below

## Componets (draft)

### OBM-directory

* Link to OSM Point (Special negative ids, containing non public items, are supported)
* Services offered
* Products offered
* Makes offered
* Pictures
* Videos
* Micropage content, multilinguage
* Editing of all data, push data to the OpenStreetMap servers which belongs there (with or without further review)

### OBM-integrity
* Caching latest OpenStreetMap data
* ability to LOCK to reviewed data version of the OSM data
* Send out notifications in case of changes for approval

### OBM-website

* Website displaying this information

### OBM-wp

* Wordpress Widget showing the OpenStreetMap based information, encouraging editing the data in OSM, instead of the page itself
