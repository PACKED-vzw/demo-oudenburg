# Metadata uit CSV omzetten naar XML

## 1. Sjabloon

Vul het [sjabloon](https://docs.google.com/spreadsheets/d/1XTvK0ADQ-RcQyZlVXnV1Ey06KBhDuytBihRaQmRbrJo/edit?usp=sharing) in Google Sheets in en exporteer dit naar CSV.

## 2. Commando

Een aangepaste versie van [CSV2DC](https://github.com/PACKED-vzw/CSV2DC) wordt gebruikt om een CSV om te zetten naar dublin core XML.

```bash
sh csv2cd.sh -cp .:lib/* CSV2Metadata -i path/to/csv.csv -o path/to/output/folder -c dcterms:identifier
```

Hiermee maak je een Dublin Core XML met het inventarisnummer als bestandsnaam.

(TODO: XSLT voor omzetting)
