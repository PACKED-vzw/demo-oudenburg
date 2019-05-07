# Metadata uit CSV omzetten naar XML

## 1. Sjabloon

Vul het [sjabloon](https://docs.google.com/spreadsheets/d/1XTvK0ADQ-RcQyZlVXnV1Ey06KBhDuytBihRaQmRbrJo/edit?usp=sharing) in Google Sheets in en exporteer dit naar CSV.

## 2. Commando

CSV2DC wordt gebruikt om een CSV om te zetten naar dublin core XML. 

```bash
sh csv2cd.sh -cp .:lib/* CSV2Metadata -i path/to/csv.csv -o path/to/output/folder -c dcterms:identifier -r description -p dcds -n http://www.dublincore.org/schemas/xmls/2008/09/01/dc-ds-xml/dcds.xsd
```

Hiermee maak je een Dublin Core XML met dcds:description als root element en met het inventarisnummer als bestandsnaam.
