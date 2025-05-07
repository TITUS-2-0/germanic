# Dataset 'Das Buch von Troja'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/mhd/troja/troja.htm).

* URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/troja/
* version: unreleased
* date: 2025-03-05

## Citation
```text
Digital version of Das Buch von Troja (draft version). By: Jost Gippert, Harald Knaus, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/troja/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Book | `div@book` | Automatically translated into named div |
| Sentence | `s` |  |
| Page | `pb` |  |
| Line | `lb` |  |

### Structural overview
```text
text (@xml:lang=gmh-Latn-x-mhg)
  front (@xml:id)
    p (@xml:id)
      [pb (@n)]
      [lb (@n)]
      [foreign (@xml:lang=lat-Latn)]
  body
    div (@data-level=1, @n, @type=book, @xml:id) (multiple)
      head (multiple)
      p (@xml:id) (multiple)
        s (@n, @xml:id) (multiple)
          [lb (@n) (multiple)]
          [pb (@n) (multiple)]
          [foreign (@xml:lang=deu-Latn | lat-Latn) (multiple)]
        [lb (@n) (multiple)]
  back (@xml:id)
    div (@data-level=1, @type=commentary, @xml:id)
      l (@xml:id) (multiple)
    div (@data-level=1, @type=date, @xml:id, @xml:lang=lat-Latn)
      p (@xml:id)
        seg (@n, @xml:id) (multiple)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="book-1" type="book" data-level="1">
				<head>Ditz buch sagt, wie troy die statt erstört ward</head>
				<p xml:id="book-1-p-2">
					<s n="1" xml:id="book-1-p-2-s-1">Ain künkreich hiezz Thesalia in dem land zu Romany.</s>
					<s n="2" xml:id="book-1-p-2-s-2">die lüt in dem land hiezzend Mirmidones.</s>
					<s n="3" xml:id="book-1-p-2-s-3">von den selben lüten schreibt man in sant Matheus legend.</s>
					<s n="4" xml:id="book-1-p-2-s-4">daz selb land haizzt man ietz Aprutz.</s>
					<s n="5" xml:id="book-1-p-2-s-5">zu den zeiten waz in dem selben land ain küng edler und gewaltiger<lb n="5"/>gehaizzen Peleus, und sein weib diu hiezz Thedida.</s>
					<s n="6" xml:id="book-1-p-2-s-6">von den zwaien geborn ward der sterkst und fraidist aller mann der do hiezz Achilles, der mit seinem leib vor der stat Troy grozz manhait begangen hät.</s>
					<s n="7" xml:id="book-1-p-2-s-7">in dem selben land zu Aprutz leit diu stat Theti, diu den namen hät von der küngin Thetida.</s>
					<s n="8" xml:id="book-1-p-2-s-8">der selb küng Peleus het ainen bruder (hiez Eson), der waz elter dann er und waz nu von alter daran komen, daz er sich vor alter nit moht gerüren, und im diu augen nu vergangen warend, also daz er unnütz waz zu ainem küng, und verzeh sich dez cepters dez reichs zu Thesalia, und gab ez uff seinen bruder Peleo.</s>
					<s n="9" xml:id="book-1-p-2-s-9">der selb küng Eson het ainen sun hiezz Jason, der waz ain stoltzer frölich jüngling und der sich in allen sachen zoch nach mänlicher ritterschaft und aller zuht.</s>
  ...
```
