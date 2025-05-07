# Dataset 'Tristan'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/mhd/tristan/trist.htm).

* URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/trist/
* version: unreleased
* date: 2025-03-05

## Citation
```text
Digital version of Tristan by Gottfried von Straßburg (draft version). By: Jost Gippert, Florian Matter, Thorsten Parchent, Ralf Schlechtweg-Jahn. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/trist/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Verse | `l` |  |
| Chapter | `milestone@chapter` |  |

### Structural overview
```text
text (@xml:lang=gmh-Latn-x-mhg)
  body
    label (@xml:lang=deu-Latn | fro-Latn) (multiple)
    lg (@n, @type=couplet, @xml:id) (multiple)
      l (@n, @xml:id) (multiple)
    lg (@n, @type=couplet, @xml:id) (multiple)
      l (@n, @xml:id) (multiple)
      label (@xml:lang=deu-Latn | fro-Latn) (multiple)
      [milestone (@n, @unit=chapter, @xml:id) (multiple)]
    [milestone (@n, @unit=chapter, @xml:id) (multiple)]
```

### Structure Example

```xml
<milestone xmlns="http://www.tei-c.org/ns/1.0" unit="chapter" n="1" xml:id="milestone-1"/>
```
