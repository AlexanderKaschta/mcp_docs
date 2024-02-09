# File formats

This file should give an overview over the different file formats used in MCP.

## Places and Locations

**File type** `JSON`

### Structure

```json title="Example file"
[
  {
    "name": "Karlsruhe-Innenstadt",
    "addresses": [
      {
        "name": "Kaiserstraße",
        "area": "Marktplatz",
        "id": 1
      },
      {
        "name": "Zirkel",
        "area": "",
        "id": 2
      },
      {
        "name": "Karl-Friedrich-Straße",
        "area": "",
        "id": 3
      }
    ],
    "objects": [
      {
        "name": "Postgalerie",
        "houseNumber": "217",
        "description": "Einkaufszentrum",
        "address": 1
      }
    ]
  }
]
```

## Mission Keywords

**File type** `CSV`

### Structure

```text
Keyword,Synonyms
Alkoholvergiftung,"Alkohol, C2, C2-Intox"
Fraktur,Knochenbruch
Schnittverletzung,
```

## Mission Resources

**File type** `CSV`

### Structure

```text
Name,Type
Auto A,KTW
Auto B,NKTW
Auto C,RTW
```