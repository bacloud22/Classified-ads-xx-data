# listings-data
This is a temporary repository for **Listings** datasets

# datasets Licensing
Care about each data license. So with each dataset file, a license file named **LICENSE-dataset-x.md** must be included. In case of absence of license, mention it in a **LICENSE-dataset-x.md** file (so it suits *dataset-x* file that resides in the same folder).

## Why temporary
Because Github is not meant for hosting raw data.

We can use this as a mean of versioning datasets knowing that geographical data and others (tags data, language specific data, translations...) for **Listings** website are normally very tiny JSON data.

Naturally, I also use this to improve data quality (like country and subdivisions delimitations precision) for my other repository **Listings**. I suggest that other forks of **Listings** repo use new forks of this repository for their datasets, but also can suggest additions to this repository.

## Nature of data
As a starter, we have

data/  
├─ geo/  
├─ locales/  
├─ taxonomy/  
├─ raw/  

All data must be in JSON format (or geojson) except data in raw that can be other types like: Vector, Raster...

## Files naming
Just mention correctly geographical area in the filename, in ISO code ?

## File size
Do not exceed 3 MB per file (3 MB is huge for the nature of files described above). If the file exceeds 3 MB, you can try to lower the precision (of geolocation points for example). We do not want to use Github for Hosting!!!

## Deploy
You can use [permanent links to files](https://docs.github.com/en/github/managing-files-in-a-repository/managing-files-on-github/getting-permanent-links-to-files) for **Listings** repositories forks only for development environments. This is a temporary repository.