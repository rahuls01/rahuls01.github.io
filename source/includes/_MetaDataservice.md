#Metadataservice

The metadata services web service unlocks the distribution layer metadata. On the basis of the request, a
response is build on the basis of the request that is send with the given parameters.
It is important to note that the metadata is not a 1 to 1 copy of how the data is saved in the distribution layer. It's a collection of data based on the parameters in the request that is requested to the service.




##OphalenCatalogus
```python
// Nothing to show check JSON
```

```json
"CatalogusFilter":
	{ 
   	"Grootheden" :True,
    "Parameters":True,
    "Compartimenten":True,
    "Hoedanigheden":True,
    "Eenheden":True,
    "BemonsteringsApparaten" :True,
    "BemonsteringsMethoden":True,
    "BemonsteringsSoorten":True,
    "BioTaxon":True,
    "BioTaxon_Compartimenten":True,
    "MeetApparaten":True,
    "MonsterBewerkingsMethoden":True,
    "Organen":True,
    "PlaatsBepalingsApparaten":True,
    "Typeringen":True,
    "WaardeBepalingstechnieken":True,
    "WaardeBepalingsmethoden":True,
    "WaardeBewerkingsmethoden":True
    }
    
}
```

```shell

{"AquoMetadataLijst": [
 {
    "AquoMetadata_MessageID": 1,
    "Parameter_Wat_Omschrijving": "Waterhoogte Oppervlaktewater t.o.v. Mean Sea Level in cm",
    "Eenheid": {
        "Code": "cm",
        "Omschrijving": "centimeter"
    },
    "Grootheid": {
        "Code": "WATHTE",
        "Omschrijving": "Waterhoogte"
    },
        "Hoedanigheid": {
        "Code": "MSL",
        "Omschrijving": "t.o.v. Mean Sea Level"
    }
 },
```
Methode | Content-Type | URL
--------- | ----------- | -----------
POST | application/json | https://waterwebservices.rijkswaterstaat.nl/METADATASERVICES_DBO/OphalenCatalogus/


Attributes | Values |  Description
--------- | ------ | ----- |  
| Grootheden |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Grootheden that can be used in the webservices |
| Parameters |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Parameters that can be used in the webservices |
| Compartimenten |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Compartimenten that can be used in the webservices |
| Hoedanigheden |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Hoedanigheden that can be used in the webservices |
| Eenheden |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Eenheden that can be used in the webservices |
| BemonsteringsApparaten |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list BemonsteringsApparaten that can be used in the webservices |
| BemonsteringsMethoden |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list BemonsteringsMethoden that can be used in the webservices |
| BemonsteringsSoorten |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list BemonsteringsSoorten that can be used in the webservices |
| BioTaxon |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list BioTaxon that can be used in the webservices |
| BioTaxon_Compartimenten |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list BioTaxon_Compartimenten that can be used in the webservices |
| MeetApparaten |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list MeetApparaten that can be used in the webservices |
| MonsterBewerkingsMethoden |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list MonsterBewerkingsMethoden that can be used in the webservices |
| Organen |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Organen that can be used in the webservices |
| PlaatsBepalingsApparaten |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list PlaatsBepalingsApparaten that can be used in the webservices |
| Typeringen |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list Typeringen that can be used in the webservices |
| WaardeBepalingstechnieken |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list WaardeBepalingstechnieken that can be used in the webservices |
| WaardeBepalingsmethoden |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list WaardeBepalingsmethoden that can be used in the webservices |
| WaardeBewerkingsmethoden |  <a href='/?python#tutorial-values'>make your own list using Tutorial Values </a>  | This list WaardeBewerkingsmethoden that can be used in the webservices |


