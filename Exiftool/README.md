# Used commands

## Prerequisites

CSV containing all the metadata. Format of the CSV should be like this:

```csv
SourceFile,XMP-dc:Identifier,XMP-dc:Title-nl,XMP-dc:Description-nl,XMP-dc:Coverage
/absolute/path/to/images,foto number,Title of your picture in Dutch,Description of your picture in Dutch,begin and end date
```

XMP supports multilangual description and title fields in DC. Add `-en` of `-fr` to Title and/or Description to add English or French titles and descriptioons (e.g. `XMP-dc:Title-nl` means that your title is in Dutch).

[Example](Exiftool/metadata.csv)

## Embed metadata

Use following command to embed the metadata in your pictures:

```bash
exiftool -csv=path/to/csv path/to/folder/images -overwrite_original
```

## Write out the metadata of your pictures

You can write out the embedded metadata in a CSV file.

```bash
exiftool -csv /path/to/folder/images > wanted/path/of/file.csv
```

You can also only write out the embedded XMP metadata in an XML file.


```bash
exiftool -xmp -b /path/to/image/file > wanted/path/of/file.xml
```