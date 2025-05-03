# Dataset 'Parzival'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/mhd/parzival/parzi.htm).

* URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/parzi/
* version: unreleased
* date: 2025-03-06

## Citation
```text
Digital version of Parzival by Wolfram von Eschenbach (draft version). By: Jost Gippert, Florian Matter, Richard Schrodt. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/parzi/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Chapter | `div@chapter` | Automatically translated into named div |
| Verse | `l` |  |

### Structural overview
```text
text (@xml:lang=gmh-Latn-x-mhg)
  body
    div (@data-level=1, @n, @type=chapter, @xml:id) (multiple)
      div (@data-level=2, @xml:id) (multiple)
        l (@n, @xml:id) (multiple)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="chapter-1" type="chapter" data-level="1">
				<div xml:id="chapter-1-div-1" data-level="2">
					<l n="1" xml:id="chapter-1-div-1-l-1">Ist zwîvel herzen nâchgebûr,</l>
					<l n="2" xml:id="chapter-1-div-1-l-2">daz muoz der sêle werden sûr,</l>
					<l n="3" xml:id="chapter-1-div-1-l-3">gesmæhet und gezieret</l>
					<l n="4" xml:id="chapter-1-div-1-l-4">ist swâ sich parrieret</l>
					<l n="5" xml:id="chapter-1-div-1-l-5">unverzaget mannes muot,</l>
					<l n="6" xml:id="chapter-1-div-1-l-6">als agelstern varwe tuot.</l>
					<l n="7" xml:id="chapter-1-div-1-l-7">der mac dennoch wesen geil,</l>
					<l n="8" xml:id="chapter-1-div-1-l-8">wande an im sint beidiu teil,</l>
					<l n="9" xml:id="chapter-1-div-1-l-9">des himels und der helle.</l>
					<l n="10" xml:id="chapter-1-div-1-l-10">der unstæte geselle</l>
  ...
```
