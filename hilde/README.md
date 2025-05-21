# Dataset 'Hildebrandlied'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/ahd/hildebrd/hilde.htm).

* URL: https://titus2.uni-frankfurt.de/dataset/hilde
* version: 0.1.0
* date: 2025-05-20

## Citation
```text
Digital version of Hildebrandlied (v0.1.0). By: Jost Gippert, Rolf-Jürgen Jacob, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://titus2.uni-frankfurt.de/dataset/hilde, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Verse | `ab@verse` |  |
| Page of ms. | `pb@manuscript` |  |
| Line of ms. | `lb@manuscript` |  |

### Structural overview
```text
text (@xml:lang=goh-Latn)
  body
    ab (@n, @type=verse, @xml:id) (multiple)
      [lb (@n, @type=manuscript) (multiple)]
      [pb (@facs=#p76v, @n, @type=manuscript)]
    [pb (@facs=#p1r, @n, @type=manuscript)]
    [lb (@n, @type=manuscript)]
```

### Structure Example

```xml
<pb xmlns="http://www.tei-c.org/ns/1.0" type="manuscript" n="1r" facs="#p1r"/>
```
