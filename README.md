# nyc-geosupport-esri-workshop <a href="http://www.dvginteractive.com/" target="_blank" align="right"><img src="http://www.dvginteractive.com/wp-content/themes/dvg/images/logob@2x.png" width="10%" ></a>
Support documentation and resources for [dvg](http://www.dvginteractive.com/) hosted "using NYC Geosupport in esri apps" workshop at Microsoft Technology Center 3/1/2017.

## News
3/23/2017 - Going forward, **dvg** will not be supporting the "NYCGeoClientGeoREST" software. Instead, a new application called **locateNYC** will be provided as a replacement. The functionality will be the same, but will support **batch geocoding** and other functionality. Once it's released, I will post here where to find it. 

## NYCGeoClientGeoREST hosting
If you would like to host your own instance, you must deploy to IIS. Visual Studio 2015 or above is required. Don't forget to add your API keys to the **Web.config** file. You'll also need to install required NuGet packages. The **dvg** repo can be found here [https://github.com/DataVisionGroup/geoclient-esri](https://github.com/DataVisionGroup/geoclient-esri) (**Note: this repository is currently undergoing some maintenence, so it will unavailable temporarily**).

The original **esri** repo is at [https://github.com/Patterns-Practices/NYCGeoClientGeoREST](https://github.com/Patterns-Practices/NYCGeoClientGeoREST). Please note that this repository is not maintained or supported in any way by esri. It is intended for educational/development purposes only.

**Instructions**
1.  Clone the repo, or download as a .zip file and unzip.
2.  Get an `app_id` and `app_key` from the NYC Developer Portal and insert it into the keys in the `Web.config` file
3.  Build the solution in Visual Studio 2015 (or above). This will install package dependencies.
4.  Debug the solution to make sure it works
5.  Deploy to IIS (8 or above).


## NYCGeoClientGeoREST endpoint
**dvg** - [https://dvgnycgeoclientgeorest.azurewebsites.net/GeocodeServer](https://dvgnycgeoclientgeorest.azurewebsites.net/GeocodeServer)

There is no SLA for this endpoint, and it may be unavailable at any time. Please use both in a testing/development capacity. If you plan to use the **dvg NYCGeoClientGeoREST** endpoint regularly or need more capacity, please let **dvg** know and we may be able to accommodate.

## ArcGIS Online
An ArcGIS Online (**AGO**) account is a requirement for registering the **NYCGeoClientGeoREST** REST endpoint. If you have an ArcGIS Desktop licence, an **AGO** account comes with it! The URL for your organization will be formatted like this - **http://[your organization].maps.arcgis.com/home/**. You can also get your own FREE development **AGO** account by signing up here [https://developers.arcgis.com/](https://developers.arcgis.com/). **Note** - this account is different from your esri global account. Don't use your esri global credentials!!

## Geoclient
In order to use Geoclient, you must register with the [NYC Developer Portal](https://developer.cityofnewyork.us/) for API keys. General info can be found at [https://developer.cityofnewyork.us/api/geoclient-api](https://developer.cityofnewyork.us/api/geoclient-api), and API doc can be found here [https://api.cityofnewyork.us/geoclient/v1/doc](https://api.cityofnewyork.us/geoclient/v1/doc).

If you plan on hosting Geoclient, you can find the source at NYC GitHub repo, at [https://github.com/CityOfNewYork/geoclient](https://github.com/CityOfNewYork/geoclient).

## Geosupport
Using Geosupport locally is possible on multiple platforms. Please see the download page here [https://www1.nyc.gov/site/planning/data-maps/open-data/dwn-gde-home.page](https://www1.nyc.gov/site/planning/data-maps/open-data/dwn-gde-home.page). GOAT is available here [http://a030-goat.nyc.gov/goat/Default.aspx](http://a030-goat.nyc.gov/goat/Default.aspx)

## Contact/Issue/Bugs
Please submit an issue for any support concerns or questions about the workshop (or anything else). For individual issues please email @EdFarrell at [efarrell@dvginteractive.com](efarrell@dvginteractive.com) or [info@dvginteractive.com](info@dvginteractive.com). You can submit and issue for this repository here [https://github.com/DataVisionGroup/nyc-geosupport-esri-workshop/issues](https://github.com/DataVisionGroup/nyc-geosupport-esri-workshop/issues).

## Credits
The workshop would not be possible (or relevant) without years of effort by NYC DoITT and DCP to build and support the Geosupport system and the Geoclient API. This workshop was sponsored by dvg and esri. 
