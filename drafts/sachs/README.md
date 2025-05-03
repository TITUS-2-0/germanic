# Dataset 'Der Sachsenspiegel'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/mhd/sachssp/sachs.htm).

* URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/sachs/
* version: unreleased
* date: 2025-03-05

## Citation
```text
Digital version of Der Sachsenspiegel (draft version). By: Jost Gippert, Harald Knaus, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/sachs/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Chapter | `div@chapter` | Automatically translated into named div |
| Paragraph | `p` |  |

### Structural overview
```text
text (@xml:lang=gmh-Latn-x-mhg)
  body
    div (@data-level=1, @n, @type=book, @xml:id)
      head (@xml:lang=deu-Latn)
      p (@xml:id)
        [lb (@n) (multiple)]
    div (@data-level=1, @n, @type=book, @xml:id) (multiple)
      head (@xml:lang=deu-Latn)
      div (@data-level=2, @n, @type=chapter, @xml:id) (multiple)
        p (@n, @xml:id) (multiple)
        p (@xml:id) (multiple)
          [lb (@n) (multiple)]
      head (multiple)
    div (@data-level=1, @n, @type=book, @xml:id)
      head (@xml:lang=deu-Latn)
      p (@xml:id)
        [lb (@n)]
      div (@data-level=2, @n, @type=chapter, @xml:id)
        head (@xml:lang=lat-Latn)
        p (@xml:id)
          [lb (@n)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="Vorr." xml:id="book-1" type="book" data-level="1">
				<head xml:lang="deu-Latn">[Vorrede von der Herren Geburt]</head>
				<p xml:id="book-1-p-1">
					<lb n="1"/>Nu vernemet umme der herren gebort vonme lande zu Sachsen.<lb n="2"/>Der markgreve von Brandenburg, der markgreve von Myszen, der von Anehalt, der von Orlemunde, der von Brenen, dise vursten sint alle Swaben. Under den vrien herren sint Swaben: der von Hakeborne, der von Gemzen unde der von Muchele. Under des riches schephen sint Swaben: der von Tribule, der von Edelerstorf, Heinrich Judas von Snetlingen, der voit Albrecht von Spandow, Alverich unde Conat von Snetlingen, Schapen kint von Jersleuen, Anne von Irkestorf, Herman von Meringen, Heidolfes kindere von Winnunge unde der von Sedorf. Diz sint alle Swaben. Der lantgreve von Doringen iz ein Vranke, der von Reynstein, der von Blankenborg, der burcgreve von Wittin, der von Klodene, der von Krosuke, der von Kotebus, diz sint alle Vranken. Der von Bruneswig, der von Luneburg, der von Poppenburg, der von Osterburg unde der von Aldenhusen, diz sint alle Swaben. Der von Warnungerode, der von Arnsteyn, der von Besenrode, der von Hademersleve, der burcgreve von Gevekenstein, der toumvoit von Halbirstat, der von Zuzelitz, der von Liechtenberg unde der von Dobin, diz sint alle geborne Swaben.
<lb n="3"/>Der herzoge von Luneburg unde sin geslechte sint geborne Sachsen, unde darzu alle vrie herren unde schephen, die zu Sachsen wonaftig sint, unde die mir kundig sint bi miner zit, sunder de hir vor benomet sint. Welch bischof von deme riche belent iz mit vanlene binnen deme lande zu Sachsen unde den herschilt dar abe hat, der heizit ein Sachse, von welchem lande her bortig si, unde muz wol orteil vinden unde orteils volgen unde vorspreche sin zu lenrechte unde zu lantrechte vor deme riche obir itlichen man, deme ez an den lip adir an de hant nicht en get, unde anders nirgen zu lantrechte noch zu lenrechte.</p>
			</div>
```
