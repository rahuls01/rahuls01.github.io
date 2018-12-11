# BulkWaarnemingService

The BulkWaarnemingenService has one function:

Function |
| ----- | 
| AanvragenBulkWaarnemingen


## AanvragenBulkWaarnemingen

```python
//Nothing to show Check JSON
```

```json
{"Zoekvraag":{"AquoMetadataLijst" :
[{"Grootheid" : {"Code" : "H1/3"},"Eenheid" : {"Code" : "cm"}},{"Compartiment":{"Code" :"OW"},
"Eenheid" : {"Code" :"%"},"Grootheid" : {"Code" :"VERDGGD"},"Parameter" : {"Code" :"O2"}},
{"Compartiment":{"Code" :"OW"},"Eenheid" : {"Code" :"mg/l"},"Parameter" : {"Code" : "O2"}}],"LocatieLijst":[{"X":742469.913149676,"Y":5940708.14824459,"Code" :"HUIBGOT"},{"X":595875.376191307,"Y" : 5790952.82210343,"Code" :"NOORDWK2"},{"X":571670.054611366,"Y":5822651.05560318,"Code" :"IJMDMNTSPS"}],"Periode":{"Begindatumtijd" : "2009-01-01T00:00:00.000+01:00","Einddatumtijd" : "2011-12-31T23:59:59.999+01:00"}},"Email_succes":{"From" :"info@rws.nl","To" : "aanvrager@rws.nl","Subject" : "Aanvraag bestandwaarnemingen","Body" : "Uw bestand met waarnemingen kunt u downloaden via {link_bestand}."},"Email_fout":{"From" :
"info@rws.nl","To" : "aanvrager@rws.nl", "Subject" : "Aanvraag niet gelukt" ,"Body" : "Uw aanvraag voor het bestand
met waarnemingen is mislukt."}, "Email_bevestiging":{"From" :"info@rws.nl","To": "aanvrager@rws.nl","Subject" : "Bevestiging van aanvraag",
"Body":"Uw aanvraag is ontvangen. U ontvangt binnen 24 uur een e-mail met daarin een link voor hetdownloaden van de aanvraag."}}
```

```shell
{
    "Aanvraagcode":"20130207_3",
    "Datumtijdaanvraag":"2013-02-07T10:17:22.814+01:00",
    "Zoekvraag":{
    "AquoMetadataLijst":[
        {"AquoMetadata_MessageID":0,
        "Eenheid":{"Code":"cm"},
        "Grootheid":{"Code":"H1/3"}},
        {"AquoMetadata_MessageID":0,
        "Compartiment":{"Code":"OW"},
        "Eenheid":{"Code":"%"},
        "Grootheid":{"Code":"VERDGGD"},
        "Parameter":{"Code":"O2"}},
        {"AquoMetadata_MessageID":0,
        "Compartiment":{"Code":"OW"},
        "Eenheid":{"Code":"mg/l"},
        "Parameter":{"Code":"O2"}}],
        "LocatieLijst":[
            {"Locatie_MessageID":0,"X":742469.913149676,"Y":5940708.14824459,"Code":"HUIBGOT"},
            {"Locatie_MessageID":0,"X":595875.376191307,"Y":5790952.82210343,"Code":"NOORDWK2"},
            {"Locatie_MessageID":0,"X":571670.054611366,"Y":5822651.05560318,"Code":"IJMDMNTSPS"}],
            "Periode":{"Begindatumtijd":"2009-01-01T00:00:00.000+01:00","Einddatumtijd":"2011-12-31T23:59:59.999+01:00"}},
            "Email_succes":{"From":"info@rws.nl","To":"aanvrager@rws.nl","Subject":"Aanvraag bestandwaarnemingen","Body":"Uw bestand met waarnemingen kunt u downloaden via {link_bestand}."},"Email_fout":{"From":"info@rws.nl","To":"aanvrager@rws.nl","Subject":"Aanvraag niet gelukt","Body":"Uw aanvraag voor het bestand met waarnemingen is mislukt."},"Email_bevestiging":{"From" : "info@rws.nl","To":
            "aanvrager@rws.nl", "Subject" : "Bevestiging vanaanvraag","Body":"Uw aanvraag is ontvangen. U ontvangt binnen 24 uur een e-mail met daarin een link voor het downloaden van de aanvraag."},
        "Succesvol":true}
```
On the right there is a sample request for requesting a Bulk Waarnemingen. This service is different
of the other web services. This has to do with the fact that there is no information about the observations
returned immediately. The request is actually parked in the distribution web services database
after which this data is collected at a later date. This data is based on
various settings that are collected after which a compressed file is generated. When this
file is created the applicant is informed that it can be downloaded from a remote location.
A valid e-mail address must be provided for this purpose. A valid e-mail address meets the
next regular expression (within quotes):

**"^ [a-zA-Z0-9 ._% -] + @ [a-zA-Z0-9 ._% -] + \. [a-zA-Z] {2 , 4} $ ".** 

Methode | Content-Type | URL
--------- | ----------- | -----------
POST | application/json | https://waterwebservices.rijkswaterstaat.nl/BulkWaarnemingenSERVICES_DBO/AanvragenBulkWaarnemingen


Attribute | Value | Description
--------- | ----------- | --------- 
| Grootheden |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Grootheden that can be used in the webservices |
| Eenheden |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Eenheden that can be used in the webservices |
| Compartimenten |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Compartimenten that can be used in the webservices |
LocatieLijst | <a href='/?python#tutorial-locations'>List using Tutorial locations </a>  | This will show the locations with and without data.

<aside class="warning">
These values used in the request and response are not real and should not be used any requests or testing. 
</aside>

<aside class="notice">
with the Attribute LocatieLijst it's possible to give multiple locations within 1 request 
</aside>