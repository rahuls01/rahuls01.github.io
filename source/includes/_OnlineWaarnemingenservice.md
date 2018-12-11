# OnlineWaarnemingenservice
The Onlinewaarnemingen unlocks the distribution layer observations. Based on the request
there observations and information about the number of observations collected and returned.

 Operations | 
| ----- |
| OphalenWaarnemingen | 
| OphalenLaatsteWaarnemingen | 
| OphalenAantalWaarnemingen | 
|  CheckWaarnemingenAanwezig.


## OphalenWaarnemingen 

```python 
// Nothing to show check JSON
```

```json
{"AquoPlusWaarnemingMetadata":
 {"AquoMetadata":{"Compartiment":
    {"Code":"OW"},
        "Eenheid":{"Code":"cm"},
        "MeetApparaat":{"Code":"109"},
        "Grootheid":{"Code":"Hm0"}}},
        "Locatie":{"X":518882.333320247,"Y":5760829.11729589,"Code":"EURPFM"},
        "Periode":{"Begindatumtijd":"2012-01-27T09:00:00.000+01:00",
                   "Einddatumtijd":"2012-01-27T09:01:00.000+01:00"}}
    }
} 
```
```shell
{"WaarnemingenLijst":[
    {"Locatie":{"Locatie_MessageID":78411364,"Coordinatenstelsel":"25831","X":518882.333320247,"Y":5760829.11729589,"Naam":"Europlatform","Code":"EURPFM"},
    "MetingenLijst":[{"Tijdstip":"2012-01-27T09:00:00.000+01:00",
    "Meetwaarde":{"Waarde_Numeriek":152.0},
    "WaarnemingMetadata":{"StatuswaardeLijst":["Ongecontroleerd"],
    "BemonsteringshoogteLijst":["-999999999"],
    "ReferentievlakLijst":["NVT"],
    "OpdrachtgevendeInstantieLijst":["RIKZMON_GOLVEN"],
    "KwaliteitswaardecodeLijst":["00"]}}],
    "AquoMetadata":{"AquoMetadata_MessageID":31234076,
    "Parameter_Wat_Omschrijving":"Significante golfhoogte uit energiespectrum van 30-500 mHz Oppervlaktewater cm",
    "BemonsteringsApparaat":{"Code":"NVT","Omschrijving":
    "Waarde is niet van toepassing"},
    "BemonsteringsMethode":{"Code":"NVT","Omschrijving":
    "Waarde is niet van toepassing"},
    "BemonsteringsSoort":{"Code":"01","Omschrijving":"Rechtstreekse meting"},
    "BioTaxon":{"Code":"NVT","Omschrijving":"NVT"},
    "BioTaxon_Compartiment":{"Code":"NVT","Omschrijving":"NVT"},
    "Compartiment":{"Code":"OW","Omschrijving":"Oppervlaktewater"},
    "Eenheid":{"Code":"cm","Omschrijving":"centimeter"},
    "Grootheid":{"Code":"Hm0","Omschrijving":"Significantegolfhoogte uit energiespectrum van 30-500 mHz"},
    "Hoedanigheid":{"Code":"NVT","Omschrijving":"Waardeis niet van toepassing"},
    "MeetApparaat":{"Code":"109","Omschrijving":"Radar"},
    "MonsterBewerkingsMethode":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
    "Orgaan":{"Code":"NVT","Omschrijving":"Waarde is nietvan toepassing"},
    "Parameter":{"Code":"NVT","Omschrijving":"Waarde isniet van toepassing"},
    "PlaatsBepalingsApparaat":{"Code":"NVT","Omschrijving":
    "Waarde is niet van toepassing"},
    "Typering":{"Code":"NVT","Omschrijving":"Waarde is nietvan toepassing"},
    "WaardeBepalingstechniek":{"Code":"NVT","Omschrijving
    ":"Waarde is niet van toepassing"},
    "WaardeBepalingsmethode":{"Code":"other:F046","Omschrijving":"Freq/tijd analyse energie en richtingen, methodeCIC/GLFPAR"},
    "WaardeBewerkingsmethode":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"}}}],
    "Succesvol":true
    }
}
```
A sample request for retrieving observations in a certain period, which
meet the specified Aquometadata, Locaties and Waarnemingen parameters.

Methode | Content-Type | URL
--------- | ----------- | -----------
POST | application/json | https://waterwebservices.rijkswaterstaat.nl/ONLINEWAARNEMINGENSERVICES_DBO/OphalenWaarnemingen



Attribute | Value | Description
--------- | ------- | -----------
Eenheden | <a href='/?python#tutorial-values'>List using Tutorial Values </a> | This will  show the Eenheden.
Grootheden | <a href='/?python#tutorial-values'>List using Tutorial Values </a> | This will show the Grootheden.
Hoedanigheden | <a href='/?python#tutorial-values'>List using Tutorial Values </a> | This will show the Hoedanigheden.
Compartimenten |  <a href='/?python#tutorial-values'>List using Tutorial Values </a> | This will show the Compartimenten.
Parameters |  <a href='/?python#tutorial-values'>List using Tutorial Values </a>  | This will show the Parameters.
| Meetapparaten |  <a href='/?python#tutorial-values'>List using Tutorial Values </a>  | This list Meetapparaten that can be used in the webservices |
Locatie | <a href='/?python#tutorial-locations'>List using Tutorial locations </a>  | This will show the locations with and without data.
Periode | 0000-00-00T00:00:00.000+01:00 | Time in the format 


## OphalenLaatsteWaarnemingen
```python
//Nothing to show check JSON
```
```json
{"AquoPlusWaarnemingMetadataLijst":[{"AquoMetadata":{"Compartiment":{"Code":"OW"},"Eenheid":{"Code":"cm"},
    "Grootheid":{"Code":"H1/3"}}}],
    "LocatieLijst":[{"X":518882.333320247,"Y":5760829.11729589,"Code":"EURPFM"
    }]
}
```

```shell
{"WaarnemingenLijst":[
{"Locatie":{"Locatie_MessageID":78411364,"Coordinatenstelsel":"25831","X":518882.333320247,"Y":5760829.11729589,"Naam":"Euro platform","Code":"EURPFM"},
"MetingenLijst":[{"Tijdstip":"2012-01-31T23:50:00.000+01:00",
"Meetwaarde":{"Waarde_Numeriek":230.0},
"WaarnemingMetadata":{"StatuswaardeLijst":["Ongecontroleerd"],
"BemonsteringshoogteLijst":["-999999999"],
"ReferentievlakLijst":["NVT"],"OpdrachtgevendeInstantieLijst":["RIKZMON_GOLVEN"],
"KwaliteitswaardecodeLijst":["00"]}}],
"AquoMetadata":{
"AquoMetadata_MessageID":86395137,
"Parameter_Wat_Omschrijving":"Gemiddelde golfhoogte uithoogste 1/3 deel van de golven Oppervlaktewater cm",
"BemonsteringsApparaat":{"Code":"NVT","Omschrijving":
"Waarde is niet van toepassing"},
"BemonsteringsMethode":{"Code":"NVT","Omschrijving":
"Waarde is niet van toepassing"},
"BemonsteringsSoort":{"Code":"01","Omschrijving":"Rechtstreekse meting"},
"BioTaxon":{"Code":"NVT","Omschrijving":"NVT"},
"BioTaxon_Compartiment":{"Code":"NVT","Omschrijving":"NVT"},
"Compartiment":{"Code":"OW","Omschrijving":"Oppervlaktewater"},
"Eenheid":{"Code":"cm","Omschrijving":"centimeter"},
"Grootheid":{"Code":"H1/3","Omschrijving":"Gemiddelde golfhoogte uit hoogste 1/3 deel van de golven"},
"Hoedanigheid":{"Code":"NVT","Omschrijving":"Waardeis niet van toepassing"},
"MeetApparaat":{"Code":"109","Omschrijving":"Radar"},
"MonsterBewerkingsMethode":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
"Orgaan":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
"Parameter":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
"PlaatsBepalingsApparaat":{"Code":"NVT","Omschrijving":
"Waarde is niet van toepassing"},
"Typering":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
"WaardeBepalingstechniek":{"Code":"NVT","Omschrijving
":"Waarde is niet van toepassing"},
"WaardeBepalingsmethode":{"Code":"other:F046","Omschrijving":"Freq/tijd analyse energie en richtingen, methode CIC/GLFPAR"},
"WaardeBewerkingsmethode":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"}}},
{"Locatie":{"Locatie_MessageID":78411364,"Coordinatenstelsel":"25831","X":518882.333320247,"Y":5760829.11729589,"Naam":"Euro platform","Code":"EURPFM"},
"MetingenLijst":[{"Tijdstip":"2012-01-31T23:50:00.000+01:00",
"Meetwaarde":{"Waarde_Numeriek":220.0},
"WaarnemingMetadata":{
"StatuswaardeLijst":["Ongecontroleerd"],
"BemonsteringshoogteLijst":["-999999999"],
"ReferentievlakLijst":["NVT"],
"OpdrachtgevendeInstantieLijst":["RIKZMON_GOLVEN"],
"KwaliteitswaardecodeLijst":["00"]}}],
"AquoMetadata":{
"AquoMetadata_MessageID":83052418,
"Parameter_Wat_Omschrijving":"Gemiddelde golfhoogte uit hoogste 1/3 deel van de golven Oppervlaktewater cm",
"BemonsteringsApparaat":{"Code":"NVT","Omschrijving":
"Waarde is niet van toepassing"},
"BemonsteringsMethode":{"Code":"NVT","Omschrijving":
"Waarde is niet van toepassing"},
"BemonsteringsSoort":{"Code":"01","Omschrijving":"Rechtstreekse meting"},
"BioTaxon":{"Code":"NVT","Omschrijving":"NVT"},
"BioTaxon_Compartiment":{"Code":"NVT","Omschrijving":"NVT"},
"Compartiment":{"Code":"OW","Omschrijving":"Oppervlaktewater"},
"Eenheid":{"Code":"cm","Omschrijving":"centimeter"},
"Grootheid":{"Code":"H1/3","Omschrijving":"Gemiddelde golfhoogte uit hoogste 1/3 deel van de golven"},
"Hoedanigheid":{"Code":"NVT","Omschrijving":"Waardeis niet van toepassing"},
"MeetApparaat":{"Code":"108","Omschrijving":"Golfmeetboei"},
"MonsterBewerkingsMethode":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
"Orgaan":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
"Parameter":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
"PlaatsBepalingsApparaat":{"Code":"NVT","Omschrijving":
"Waarde is niet van toepassing"},
"Typering":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
"WaardeBepalingstechniek":{"Code":"NVT","Omschrijving
```


The following is a sample request for retrieving the last observation that is requested with the
specified Aquometadata, Locaties and Waarnemingen parameters.

Methode | Content-Type | URL
--------- | ----------- | -----------
POST | application/json | https://waterwebservices.rijkswaterstaat.nl/ONLINEWAARNEMINGENSERVICES_DBO/OphalenLaatsteWaarnemingen

Attribute | Description | Value
--------- | ----------- | --------- 
| Compartimenten |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Compartimenten that can be used in the webservices |
| Eenheden |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Eenheden that can be used in the webservices |
| Grootheden |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Grootheden that can be used in the webservices |
LocatieLijst | <a href='/?python#tutorial-locations'>List using Tutorial locations </a>  | This will show the locations with and without data.

<aside class="notice">
with the Attribute LocatieLijst it's possible to give multiple locations within 1 request 
</aside>

## CheckWaarnemingenAanwezig

```python
//Nothing to show check JSON
```

```json
{"AquoMetadataLijst" :
    [{"Compartiment":{"Code":"OW"},"Eenheid":{"Code":"cm"}}],
    "LocatieLijst" : [{"X" :518882.333320247,"Y" :5760829.11729589,"Code":"EURPFM"}],
    "Periode" : {"Begindatumtijd" : "2012-01-16T14:00:00.000+01:00","Einddatumtijd": "2012-01-16T16:00:00.000+01:00"
    }
}
```

```shell
{
    "Succesvol":true,
    "WaarnemingenAanwezig":"true"
    }

When there are no Values:
{
    "Succesvol":true,
    "WaarnemingenAanwezig":"false"
}


```

Below is a sample request for checking if there are observations for one
certain period that meet the specified Aquometadata, Locaties and Waarnemingen parameters.

Methode | Content-Type | URL
--------- | ----------- | -----------
POST | application/json | https://waterwebservices.rijkswaterstaat.nl/ONLINEWAARNEMINGENSERVICES_DBO/CheckWaarnemingen


Atrribute | Value | Description
--------- | ----------- | --------- 
| Compartimenten |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Compartimenten that can be used in the webservices |
| Eenheden |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Eenheden that can be used in the webservices |
Periode | 0000-00-00T00:00:00.000+01:00 | Time in the format 
LocatieLijst | <a href='/?python#tutorial-locations'>List using Tutorial locations </a>  | This will show the locations with and without data.

<aside class="notice">
with the Attribute LocatieLijst it's possible to give multiple locations within 1 request 
</aside>

## OphalenAantalWaarnemingen

```python
//Nothing to show Check JSON
```
```json
{"AquoMetadataLijst" :
    [{"Compartiment":{"Code":"OW"},"Eenheid":{"Code":"cm"}}],
    "Groeperingsperiode" : "Week",
    "LocatieLijst" : [{"X" :518882.333320247,"Y" :5760829.11729589,"Code":"EURPFM"}],
    "Periode" : {"Begindatumtijd" : "2012-01-16T14:00:00.000+01:00","Einddatumtijd": "2012-01-16T16:00:00.000+01:00"
    }
}
```

```shell 
{"AantalWaarnemingenPerPeriodeLijst":[
{"AquoMetadata":{"AquoMetadata_MessageID":30064212,
"Parameter_Wat_Omschrijving":"Significante golfhoogte uitenergiespectrum van 30-500 mHz Oppervlaktewater cm",
"BemonsteringsApparaat":{"Code":"NVT","Omschrijving":
"Waarde is niet van toepassing"},
"BemonsteringsMethode":{"Code":"NVT","Omschrijving":
"Waarde is niet van toepassing"},
"BemonsteringsSoort":{"Code":"01","Omschrijving":"Rechtstreekse meting"},
"BioTaxon":{"Code":"NVT","Omschrijving":"NVT"},
"BioTaxon_Compartiment":{"Code":"NVT","Omschrijving":"NVT"},
"Compartiment":{"Code":"OW","Omschrijving":"Oppervlaktewater"},
"Eenheid":{"Code":"cm","Omschrijving":"centimeter"},
"Grootheid":{"Code":"Hm0","Omschrijving":"Significantegolfhoogte uit energiespectrum van 30-500 mHz"},
"Hoedanigheid":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
"MeetApparaat":{"Code":"108","Omschrijving":"Golfmeetboei"},
"MonsterBewerkingsMethode":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
"Orgaan":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
"Parameter":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
"PlaatsBepalingsApparaat":{"Code":"NVT","Omschrijving":
"Waarde is niet van toepassing"},
"Typering":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"},
"WaardeBepalingstechniek":{"Code":"NVT","Omschrijving
":"Waarde is niet van toepassing"},
"WaardeBepalingsmethode":{"Code":"other:F046","Omschrijving":"Freq/tijd analyse energie en richtingen, methode CIC/GLFPAR"},
"WaardeBewerkingsmethode":{"Code":"NVT","Omschrijving":"Waarde is niet van toepassing"}},
"Locatie":{"Locatie_MessageID":78411364,"Coordinatenstelsel":"25831","X":518882.333320247,"Y":5760829.11729589,"Naam":"Euro platform","Code":"EURPFM"},
"AantalMetingenPerPeriodeLijst":[{"Groeperingsperiode":{"Jaarnummer":2012,"Week":3},"AantalMetingen":21}]
},
```

The following is an example request for retrieving the number of observations about a certain one
period that met the specified Aquometadata, Locaties and Waarnemingen parameters, grouped
over a certain grouping period.

<aside class="notice">
This web service is not used yet and  performance issues are known.
</aside>


Methode | Content-Type | URL
--------- | ----------- | -----------
POST | application/json | https://waterwebservices.rijkswaterstaat.nl/ONLINEWAARNEMINGENSERVICES_DBO/OphalenAantalWaarnemingen


Attribute | Value | Description
--------- | ----------- | --------- 
| Compartimenten |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Compartimenten that can be used in the webservices |
| Eenheden |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Eenheden that can be used in the webservices |
Periode | 0000-00-00T00:00:00.000+01:00 | Time in the format 
LocatieLijst | <a href='/?python#tutorial-locations'>List using Tutorial locations </a>  | This will show the locations with and without data.

<aside class="notice">
with the Attribute LocatieLijst it's possible to give multiple locations within 1 request.
</aside>

