# Workflow Oudenburg

Deze repository bewaart code en voorbeelden voor de workflow van de gemeentes Koekelare, Oudenburg en Zedelgem voor de duurzame bewaring van de beelden.

De workflow bestaat uit volgende stappen:

1. het beschrijven in CSV van zowel collectie als stuk en deze omzetten naar XML; hiervoor kan [Google Sheets](https://www.google.com/sheets/about/) gebruikt worden (geen Excel!).
2. Omzetten van de CSV's naar Dublin Core/XML via een aangepaste versie van [CSV2DC](https://github.com/PACKED-vzw/CSV2DC).
3. het beschrijven van de beelden in CSV en de metadata vervolgens inbedden in de beelden
4. bestandsidentificatie van de beeldbestanden via [DROID](http://www.nationalarchives.gov.uk/information-management/manage-information/policy-process/digital-continuity/file-profiling-tool-droid/)
5. creatie van een BagIT met alle bestanden (metadata en beelden) via [Bagger](https://github.com/LibraryOfCongress/bagger)
6. Optioneel: controle van de BagIT op bitrot via [Fixity](https://www.weareavp.com/products/fixity/) (indien BagIT gezipt wordt)

## Gebruik van de workflow

Lees hiervoor de [gebruikershandleiding](https://github.com/PACKED-vzw/demo-oudenburg/wiki).

## Inhoud

* [Bagger](Bagger): custom beschrijvingsprofiel voor de BagITs en een voorbeeldbag
* [DROID](DROID): voorbeeld van een resultaat van DROID
* [ExifTool](Exiftool): uitleg en voorbeeld voor het gebruik van ExifTool
* [Fixity](Fixity/Fixity_Reports): voorbeelden van rapporten van Fixity
* [Metadata](Metadata): voorbeelden en uitleg om de stukken te beschrijven in CSV en ze vervolgens om te zetten naar XML
