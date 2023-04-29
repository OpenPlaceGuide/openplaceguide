# OpenPlaceGuide

OpenPlaceGuide (OPG) will be a free and open source business directory, based on the OpenStreetMap project.
It combines data from the OpenStreetMap project, as well as additional information about businesses.

    Open Business Map - OpenStreetMap-based business directory
    Copyright (C) 2019-2023  Bandira Addis Map Entertainment PLC, Addis Ababa

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU Affero General Public License as published
    by the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU Affero General Public License for more details.  

## Organization

This is the main organizational repository without any code. Check the [issues](https://github.com/OpenPlaceGuide/openplaceguide/issues) section for details.

## Vision

Creating a modern OpenStreetMap based website with the functionality of www.addismap.com, fully Open Source.

## User Stories

* As a business owner I want to present my information on a website

* As a business owner I want to control the information shown in the business directory and website

* As a user and business owner I am interested in accurate data in OpenStreetMap.

* AS a tourist I want to find information about places and businesses in a city easily.

* As a business guide facilitator I want to earn money by helping business to get on my business guide page via adding them to OpenStreetMap and use the raised money to sustain OpenStreetMap mapping.

## Introduce yourself!

OpenPlaceGuide is in an early phase - we look for contributors and partners. [Introduce yourself](https://github.com/OpenPlaceGuide/openplaceguide/discussions/15)

## Data

### OpenStreetMap

* Name (in all available languages)
* Classification
* Location data
* Opening Times

### OpenPlaceGuide

* All the additional data, see components below

## Components (draft)

### [OPG-discover](https://github.com/OpenPlaceGuide/discover-cf-worker)

The purpose of this module is to discover OPG websites based on a location.
OPG uses a federated approach. Anybody can add the area they are responsible for (in terms of moderating the business information)
and 3rd party websites can discover those pages.

The API is centrally hosted at cloudflare and reachable at [https://discover.openplaceguide.org/](https://discover.openplaceguide.org/)

### [OPG-directory](https://github.com/OpenPlaceGuide/data)

* Link to OSM Object, or multiple OSM objects (for chains / banks etc., i.e. branches)
* Services offered
* Products offered
* Makes offered
* Pictures
* Videos (mostly as YouTube / Vimeo etc. links) ?
* Menu cards (pictures as well as structured, text based information)
* Micropage content, multilingual
* Mapillary Links
* Editing of all data, push data to the OpenStreetMap servers which belongs there (with or without further review)

The current idea is to keep the directory information in a GitHub repository and allow everybody to make pull requests to add new business information.

Adding businesses / shooting photos / writing texts can be additionally done as a paid service. Businesses offering this, shall invest into generally mapping the area they are active in OpenStreetMap.


### [OPG-pages](https://github.com/OpenPlaceGuide/opg-pages)

* Website displaying this information
* Proper SEO for the business pages
* Support subdomain, path (or own domain?)
* Proper Rich Snippets

### OPG-integrity

* Caching latest OpenStreetMap data
* ability to LOCK to reviewed data version of the OSM data
* Send out notifications in case of changes for approval

### OPG-wp

* Wordpress Widget showing the OpenStreetMap based information, encouraging editing the data in OSM, instead of the page itself, Kick-start pagegenerator -> From Micropage to WordPress website

## Related projects / Acknowledgements / Contributions

* For the main page we plan to use and contribute(d) to [OsmAPP](https://osmapp.org/)
* For reviews we plan to use and contribute(d) to [Mangrove](https://mangrove.reviews/)
* Tile server [OPG Africa Tiles](https://africa.tiles.openplaceguide.org/) - a [Makina Maps](https://github.com/makina-maps/makina-maps) instance - for African projects is sponsored  by [BAME PLC](https://addismap.com/bandira).
* As default we use the [Overpass Server by KUMI](https://overpass.kumi.systems/)
* And of course all this would not be possible without [OpenStreetMap](https://osm.org)
