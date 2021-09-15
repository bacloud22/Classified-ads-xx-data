# Classified-ads-xx-data
This is a temporary repository for [**Classified-ads-48**](https://github.com/bacloud14/Classified-ads-48) and its forks datasets

# datasets Licensing
Care about each data license. So with each dataset file, a license file named **LICENSE-dataset-x.md** must be included. In case of absence of license, mention it in a **LICENSE-dataset-x.md** file (so it suits *dataset-x* file that resides in the same folder).

## Why temporary
Because Github is not meant for hosting raw data.

We can use this as a mean of versioning datasets knowing that geographical data and others (tags data, language specific data, translations...) for [**Classified-ads-xx**](https://github.com/bacloud14/Classified-ads-48) website are normally very tiny JSON data.

Naturally, I also use this to improve data quality (like country and subdivisions delimitations precision) for my other repository [**Classified-ads-48**](https://github.com/bacloud14/Classified-ads-48). I suggest that other forks of [**Classified-ads-48**](https://github.com/bacloud14/Classified-ads-48) repo use new forks of this repository for their datasets, but also can suggest additions to this repository.

## Nature of data
As a starter, we have

data/  
├─ geo/  
├─ locales/  
├─ taxonomy/  
├─ raw/  

All data must be in JSON format (or geojson) except data in raw that can be other types like: Vector, Raster...

### Metadata
To be read in [**Classified-ads-xx**](https://github.com/bacloud14/Classified-ads-48), metadata should be:

- `feature.properties.name_{lang}` must exist.
- ...

## Files naming
Just mention correctly geographical area in the filename, in ISO code ?

## File size
Do not exceed 3 MB per file (3 MB is huge for the nature of files described above). If the file exceeds 3 MB, you can try to lower the precision (of geolocation points for example). We do not want to use Github for Hosting!!!

## Deploy
You can use [permanent links to files](https://docs.github.com/en/github/managing-files-in-a-repository/managing-files-on-github/getting-permanent-links-to-files) for [**Classified-ads-xx**](https://github.com/bacloud14/Classified-ads-48) repositories only for development environments. This is a temporary repository.

## Other tools and ressoures
These tools and ressources can be used to generate data for this repository (please care about licenses and attribution when necessary).  
Some represent raw data that I couldn't verify myself. If someone is sure, please push to this repository.
- India data: [data](https://github.com/geohacker/india) (it must be down-sized)
- France data: https://france-geojson.gregoiredavid.fr/
- Italy data: https://github.com/openpolis/geojson-italy
- Spain data: [here](https://github.com/codeforgermany/click_that_hood/blob/master/public/data/spain-provinces.geojson)
- USA data: [here](https://public.opendatasoft.com/explore/dataset/us-state-boundaries/table/?location=3,41.04622,-77.60742&basemap=jawg.streets) and [here](https://eric.clst.org/tech/usgeojson/)
- Japan data: [data](https://github.com/dataofjapan/land/blob/master/japan.geojson)
- Germany data: [data](https://github.com/isellsoap/deutschlandGeoJSON)
- UK data: [data](https://github.com/martinjc/UK-GeoJSON)
- ...

### Tools
- Read, create and modify GEOJSON data https://geojson.io/
- Convert to GEOJSON:  
  - https://www.convertcsv.com/csv-to-geojson.htm
  - https://ogre.adc4gis.com/ 
  - https://mygeodata.cloud/converter/kml-to-geojson


**(some are to be verified, down-sized, and modified)**

## Contribution
As always, all my repositories are firstcomers friendly ! 

As I am always learning, please do not hesitate to open any new issue (like better code, readability, modularity and best practice, performance, better UI or even functionality enhancements...).

- Enrich with other datasets
- Optimize delimitations 
- Enrich languages (`feature.properties.name_{lang}`)
- Make a web-page and host this
