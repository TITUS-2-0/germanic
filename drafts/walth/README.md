# Dataset 'Lieder (Auswahl)'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/mhd/walther/walth.htm).

* URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/walth/
* version: unreleased
* date: 2025-03-05

## Citation
```text
Digital version of Lieder (Auswahl) by Walther von der Vogelweide (draft version). By: Jost Gippert, Florian Matter, Julia Neumann. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/walth/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Song | `div@song` | Automatically translated into named div |
| Strophe | `lg@stanza` |  |
| Verse | `l` |  |

### Structural overview
```text
text (@xml:lang=gmh-Latn-x-mhg)
  body
    div (@data-level=1, @n, @type=song, @xml:id) (multiple)
      head (multiple)
      lg (@n, @type=stanza, @xml:id) (multiple)
        l (@n, @xml:id) (multiple)
      [note (@xml:id, @xml:lang=und-Latn-x-general) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="26" xml:id="song-1" type="song" data-level="1">
				<head>Herzeliebez vrôwelîn</head>
				<note xml:id="song-1-note-1" xml:lang="und-Latn-x-general">Cormeau 26</note>
				<lg n="I" type="stanza" xml:id="song-1-lg-1">
					<l n="1" xml:id="song-1-lg-1-l-1">Herzeliebez vrowelîn,</l>
					<l n="2" xml:id="song-1-lg-1-l-2">got gebe dir hiute und iemer guot!</l>
					<l n="3" xml:id="song-1-lg-1-l-3">kund ich baz gedenken dîn,</l>
					<l n="4" xml:id="song-1-lg-1-l-4">des het ich willeclîchen muot.</l>
					<l n="5" xml:id="song-1-lg-1-l-5">Waz mac ich nû sagen mê,</l>
					<l n="6" xml:id="song-1-lg-1-l-6">wan daz dir nieman holder ist? owê, dâ von ist mir vil wê!</l>
				</lg>
				<lg n="II" type="stanza" xml:id="song-1-lg-2">
  ...
```
