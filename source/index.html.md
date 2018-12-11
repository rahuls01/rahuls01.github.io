---
title: Webservices

language_tabs: 

  - json: JSON Request
  - shell: JSON Response
  - python: Python

toc_footers:
  - <a href="https://waterinfo.rws.nl/#!/nav/index/">Website Waterinfo</a>

includes:
  - TutorialLoc
  - TutorialPara
  - MetaDataservice
  - OnlineWaarnemingenservice
  - BulkWaarnemingService
  - WebFeatureServices
  - version
  - errors
  


search: true
---
# Introduction
```python
// Nothing to show
```

```json
// Nothing to show
```

```shell
// Nothing to show
```
<aside class="notice">
Check the following languages  on the right  ------ >
</aside>

The system is intended to access/retrieve  data from the distributie laag through web services. the
data is accessed through five web services (three HTTP JSON web services and two WFS
web service):
  
Webservices |
| ----- |
| MetadataService |
| Online Waarnemingen Service |
| Bulk Waarnemingen Service |
| Web Feature Service |
| Web Mapping Service | 


**Metadata Service** 

The Metadata Service has one function:

Function |
| ----- |
| Ophalen Catalogus |

A request for this service will provide several lists of metadata from the
distributie laag. On the basis of the data in these lists, you can fill the request for other services.

**OnlineWaarnemingenServices**

The OnlineWaarnemingenServices has four functions:

 Function | 
| ----- |
| Ophalen Waarnemingen | 
| Ophalen Laatste Waarnemingen | 
| Ophalen Aantal Waarnemingen | 
| Check Waarnemingen Aanwezig

With a request to the  **Ophalenwaarnemingen service** it's possible to get all observations with the right parameters. These parameters need to relate to **Aquometadata**, **Locatie** and **Periode** where de observations are done. A request to the **OphalenLaasteWaarnemingenService** will return the last obervation. The service **OphalenLaatsteWaarnemingen** returns observations per grouped specified grouping on period. The **CheckWaarnemingenAanwezigService** returns the observations from the distributie laag wich are those that comply with the parameters provided.

**BulkWaarnemingenService**

The BulkWaarnemingenService has one function:

Function |
| ----- | 
| Aanvragen Bulk Waarnemingen

With the **AanvragenBulkWaarnemingen** service an application can be made to a
a server that can be downloaded from a Rijkswaterstaat server at a later time.

**Web Feature Service**

The Web Feature Service has two functions:
  
Function |
| ----- |
| Locaties
| Locaties Met Laatste Waarneming

With the Mapserver, the geometry within the distributie laag is made available through Web
Feature Service. Through the **Web Feature Service** you can find the locaties and locaties in combination with the last 
observation.

**Web Mapping Service**

The Web Mapping Service has three functions:
  
Function | 
| ------ | 
| WMS versie 1.1.0
| WMS versie 1.1.1
| WMS versie 1.3.0

The Mapping service responds to an xml request with a description of the layers.
The Getmap service provides an image of the specified area.
The Getfeature provides the details of a feature per location as an response.

**Dependence**

The web services depend on the distributie laag. When the distributie laag is not functioning properly,
this has an influence on the functioning of the web services. Requests within all web services and the Web Feature Service
make use of the Locatie, Aquometadata and Waarnemingen in the distributie laag.


**Dates**

If you are using dates in the request statements within the services you need to keep the following format:

| Year | Month | Day | Separator | Hours | Minutes | Seconds | Time zone |
| -----| -----| -----| -----| -----| -----| -----| -----| 
| 0000 | 00 | 00 | T | 00 | 00 | 000 | 00:00  | 

For more information on the format <a href = "https://en.wikipedia.org/wiki/ISO_8601#Combined_date_and_time_representations">ISO 8601</a>

## Applications 

When the webservices are used it's possible to use the following applications. This is not a requirement. It's also possible to use your own applications.

### Postman 

| Naam | Link to Documentation | Version
| -----| ------ | ------- |
| Postman | https://www.getpostman.com/ | 6.5.3

Postman can be used to test the POST requests to the webservices. Within Postman there different options wich can be used to make it less hard to understand the services.

### Visual studio Code

| Name | Link to documentation| Version
| -----| ------ | ------- |
| Visual Studio Code | https://code.visualstudio.com/ | darwin stable


Visual Studio Code is a tool that can be used to create different scripts and applications. Within the application its possible to install serveral modules to make it easy to use the webservices.
