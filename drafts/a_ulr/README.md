# Dataset 'The Middle High German Books on The Great Alexander''

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/mhd/a_ulrich/a_ulr.htm).

* URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/a_ulr/
* version: unreleased
* date: 2025-03-07

## Citation
```text
Digital version of The Middle High German Books on The Great Alexander' by Ulrich von Eschenbach (draft version). By: Jost Gippert, Stefanie Heine, Florian Matter, Ralf Schlechtweg-Jahn. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/a_ulr/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Chapter | `Book` |  |
| Book | `Chapter` |  |
| Verse | `l` |  |
| Author | `div@author` | Automatically translated into named div |

### Structural overview
```text
text (@xml:lang=gmh-Latn-x-mhg)
  body
    div (@data-level=1, @n, @type=book, @xml:id) (multiple)
      div (@data-level=2, @n, @type=chapter, @xml:id) (multiple)
        head (@xml:lang=deu-Latn) (multiple)
        lg (@n, @type=stanza, @xml:id) (multiple)
          l (@n, @xml:id) (multiple)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="book-1" type="book" data-level="1">
				<div n="Prol." xml:id="book-1-chapter-1" type="chapter" data-level="2">
					<head xml:lang="deu-Latn">Prolog</head>
					<lg n="1" type="stanza" xml:id="book-1-chapter-1-lg-1">
						<l n="1" xml:id="book-1-chapter-1-lg-1-l-1">Gott hêrre, ân anegenge got,</l>
						<l n="2" xml:id="book-1-chapter-1-lg-1-l-2">rîcher künic Sâbâot,</l>
					</lg>
					<lg n="2" type="stanza" xml:id="book-1-chapter-1-lg-2">
						<l n="3" xml:id="book-1-chapter-1-lg-2-l-3">immer und êwic dîn gebot</l>
						<l n="4" xml:id="book-1-chapter-1-lg-2-l-4">vor aller engestlîcher nôt</l>
					</lg>
					<lg n="3" type="stanza" xml:id="book-1-chapter-1-lg-3">
  ...
```
