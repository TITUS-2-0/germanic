# Dataset 'Edda'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/anord/edda/edda.htm).

* URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/edda/
* version: unreleased
* date: 2025-01-08

## Citation
```text
Digital version of Edda (draft version). By: Fabrizio Ducci, Jost Gippert, Florian Matter, Sigurdur H. Palsson, David Stifter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/edda/, visited on <insert date>)
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
text (@xml:lang=non-Latn)
  body
    div (@data-level=1, @n, @type=song, @xml:id) (multiple)
      head (multiple)
      lg (@n, @type=stanza, @xml:id) (multiple)
        l (@n, @xml:id) (multiple)
    div (@data-level=1, @n, @type=song, @xml:id) (multiple)
      lg (@n, @type=stanza, @xml:id) (multiple)
        l (@n, @xml:id) (multiple)
        [note (@xml:id, @xml:lang=deu-Latn) (multiple)]
    div (@data-level=1, @n, @type=song, @xml:id) (multiple)
      head (multiple)
        [lb (@n) (multiple)]
      lg (@n, @type=stanza, @xml:id) (multiple)
        l (@n, @xml:id) (multiple)
      p (@xml:id) (multiple)
        [lb (@n) (multiple)]
    div (@data-level=1, @n, @type=song, @xml:id) (multiple)
      head (multiple)
      div (@data-level=2, @type=preface, @xml:id) (multiple)
        head (multiple)
          [foreign (@xml:lang=lat-Latn)]
        p (@xml:id) (multiple)
          [lb (@n) (multiple)]
      div (@data-level=2, @type=wrapper, @xml:id) (multiple)
        lg (@n, @type=stanza, @xml:id) (multiple)
          l (@n, @xml:id) (multiple)
      div (@data-level=2, @type=preface, @xml:id) (multiple)
        p (@xml:id) (multiple)
          [lb (@n) (multiple)]
      div (@data-level=2, @type=wrapper, @xml:id) (multiple)
        lg (@n, @type=stanza, @xml:id) (multiple)
          l (@n, @xml:id) (multiple)
        p (@xml:id) (multiple)
          [lb (@n) (multiple)]
      [note (@xml:id, @xml:lang=und-Latn-x-general)]
        [lb (@n)]
      [milestone (@facs=#facs-1, @unit=ref, @xml:id)]
    div (@data-level=1, @n, @type=song, @xml:id)
      lg (@n, @type=stanza, @xml:id) (multiple)
        l (@n, @xml:id) (multiple)
        [note (@xml:id, @xml:lang=deu-Latn) (multiple)]
      p (@xml:id)
        [lb (@n)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="Vsp." xml:id="song-1" type="song" data-level="1">
				<head>VǪLOSPÁ</head>
				<lg n="1" type="stanza" xml:id="song-1-lg-1">
					<l n="1" xml:id="song-1-lg-1-l-1">Hlióðs bið ec allar helgar kindir,</l>
					<l n="2" xml:id="song-1-lg-1-l-2">meiri oc minni, mǫgo Heimdalar;</l>
					<l n="3" xml:id="song-1-lg-1-l-3">vildo, at ec, Valfǫðr, vel fyrtelia</l>
					<l n="4" xml:id="song-1-lg-1-l-4">forn spiǫll fira, þau er fremst um man.</l>
				</lg>
				<lg n="2" type="stanza" xml:id="song-1-lg-2">
					<l n="1" xml:id="song-1-lg-2-l-5">Ec man iǫtna, ár um borna,</l>
					<l n="2" xml:id="song-1-lg-2-l-6">þá er forðom mic fœdda hǫfðo;</l>
					<l n="3" xml:id="song-1-lg-2-l-7">nío man ec heima, nío íviði,</l>
  ...
```
