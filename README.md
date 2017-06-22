# vbb-stations

Here you can find lists of stations in Berlin which are operated by Berliner Verkehrsbetriebe (BVG) or S-Bahn Berlin GmbH. The files are in JSON format.

## File Description

### [all-stations-with-operators.json](all-stations-with-operators.json)

In these file are all stations operated by BVG (Berliner Verkehrsbetriebe) or S-Bahn Berlin GmbH.

```
[
  [
    "900000100003", // 12 digit VBB id
    "S+U Alexanderplatz Bhf (Berlin)", // name of the station
    ["1", "796"] // array with id's of the operators (agency_id)
  ]
]
```

The agency's are:

```
{
	id: '796',
	name: 'Berliner Verkehrsbetriebe',
	url: 'http://www.bvg.de',
	timezone: 'Europe/Berlin',
	language: 'de',
	phone: null
},
{
	id: '1',
	name: 'S-Bahn Berlin GmbH',
	url: 'http://www.s-bahn-berlin.de',
	timezone: 'Europe/Berlin',
	language: 'de',
	phone: null
}
```

### [operated-by-bvg.json](operated-by-bvg.json)

```
[
  [
    "009023302", // 9 digit VBB id
    "U Adenauerplatz (Berlin)", // name of the station
    "Adenauerplatz" // clean name of the station
  ]
]   
```

### [operated-by-sbahn-berlin-gmbh.json](operated-by-sbahn-berlin-gmbh.json)

like operated-by-bvg.json

## Todo

### New Stations

#### BVG (Berliner Verkehrsbetriebe)

| Name                                     |     opens     |
| ---------------------------------------- | :-----------: |
| [Museumsinsel](https://de.wikipedia.org/wiki/U-Bahnhof_Museumsinsel) | expected 2019 |
| [Rotes Rathaus](https://de.wikipedia.org/wiki/U-Bahnhof_Rotes_Rathaus) | expected 2019 |
| [Unter den Linden](https://de.wikipedia.org/wiki/U-Bahnhof_Unter_den_Linden) | expected 2019 |

#### S-Bahn Berlin GmbH

| Name                                     | opens |
| ---------------------------------------- | :---: |
| [Flughafen Berlin-Brandenburg](https://de.wikipedia.org/wiki/Bahnhof_Flughafen_Berlin_Brandenburg) |  😅   |
| [Perleberger Brücke](https://de.wikipedia.org/wiki/Bahnhof_Berlin_Perleberger_Br%C3%BCcke) |   ?   |
| [Waßmannsdorf](https://de.wikipedia.org/wiki/Bahnhof_Wa%C3%9Fmannsdorf) |   ?   |

## Errors

If you find an error feel free to create a *pull request*.

## Sources

- [Wikipedia/Liste der Berliner U-Bahnhöfe](https://de.wikipedia.org/wiki/Liste_der_Berliner_U-Bahnh%C3%B6fe)
- [Wikipedia/Liste der Stationen der S-Bahn Berlin](https://de.wikipedia.org/wiki/Liste_der_Stationen_der_S-Bahn_Berlin)
- VBB-Fahrplandaten (GTFS-Format)
