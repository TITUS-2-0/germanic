# Dataset 'Das Buch der Natur'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/mhd/konrmeg/konrm.htm).

* URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/konrm/
* version: unreleased
* date: 2025-03-06

## Citation
```text
Digital version of Das Buch der Natur by Konrad von Megenburg (draft version). By: Jost Gippert, Florian Matter, Koyka Stoyanova. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/konrm/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Book | `div@book` | Automatically translated into named div |
| Chapter / Strophe | `chapter` |  |
| Page | `pb` |  |
| Line | `lb` |  |

### Structural overview
```text
text (@xml:lang=gmh-Latn-x-mhg)
  body
    div (@data-level=1, @type=prologue, @xml:id)
      lg (@n, @type=stanza, @xml:id) (multiple)
        l (@n, @xml:id) (multiple)
      [pb (@n) (multiple)]
    div (@data-level=1, @n, @type=book, @xml:id) (multiple)
      head (multiple)
        [lb (@n) (multiple)]
        [foreign (@xml:lang=und-Latn-x-general) (multiple)]
      p (@xml:id) (multiple)
        [lb (@n) (multiple)]
        [pb (@n) (multiple)]
        [foreign (@xml:lang=grc-Grek | lat-Latn) (multiple)]
      div (@data-level=2, @n, @type=chapter, @xml:id) (multiple)
        head (multiple)
          [lb (@n) (multiple)]
        p (@xml:id) (multiple)
          [lb (@n) (multiple)]
          [foreign (@xml:lang=grc-Grek | lat-Latn) (multiple)]
          [pb (@n) (multiple)]
        [lb (@n) (multiple)]
        [milestone (@n, @unit=chapter, @xml:id, @xml:lang=und-Latn-x-general) (multiple)]
      div (@data-level=2, @n, @type=chapter, @xml:id)
        head
          [lb (@n)]
        [lb (@n)]
        [milestone (@n, @unit=chapter, @xml:id, @xml:lang=und-Latn-x-general)]
      [pb (@n)]
      [lb (@n) (multiple)]
      [milestone (@n, @unit=book, @xml:id, @xml:lang=und-Latn-x-general) (multiple)]
    div (@data-level=1, @n, @type=book, @xml:id) (multiple)
      head (multiple)
        [lb (@n) (multiple)]
      div (@data-level=2, @n, @type=chapter, @xml:id) (multiple)
        head (multiple)
          [lb (@n) (multiple)]
        p (@xml:id) (multiple)
          [lb (@n) (multiple)]
          [foreign (@xml:lang=grc-Grek | lat-Latn) (multiple)]
          [pb (@n) (multiple)]
        [lb (@n) (multiple)]
        [milestone (@n, @unit=chapter, @xml:id, @xml:lang=und-Latn-x-general) (multiple)]
      [lb (@n) (multiple)]
      [milestone (@n, @unit=book, @xml:id, @xml:lang=und-Latn-x-general) (multiple)]
    div (@data-level=1, @n, @type=book, @xml:id)
      head
        [lb (@n)]
      p (@xml:id)
        [lb (@n) (multiple)]
        [pb (@n) (multiple)]
        [foreign (@xml:lang=lat-Latn) (multiple)]
      [lb (@n)]
      [milestone (@n, @unit=book, @xml:id, @xml:lang=und-Latn-x-general)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" xml:id="prologue-1" type="prologue" data-level="1">
				<pb n="1"/>
				<lg n="1" type="stanza" xml:id="prologue-1-lg-1">
					<l n="1" xml:id="prologue-1-lg-1-l-1">Ain wirdig weibes krôn,</l>
					<l n="2" xml:id="prologue-1-lg-1-l-2">in welhem klaid man die ansiht,</l>
					<l n="3" xml:id="prologue-1-lg-1-l-3">sô sint ir tugentleicheu werc an kainem end verhandelt;</l>
					<l n="4" xml:id="prologue-1-lg-1-l-4">si stêt geladen schôn</l>
					<l n="5" xml:id="prologue-1-lg-1-l-5">(diu wârhait pilleich ir des giht)</l>
					<l n="6" xml:id="prologue-1-lg-1-l-6">reht als ain engadischer reb, ob der sein fruht niht [wandelt.</l>
				</lg>
				<lg n="2" type="stanza" xml:id="prologue-1-lg-2">
					<l n="1" xml:id="prologue-1-lg-2-l-7">Sam tuot diu edel kunst:</l>
  ...
```
