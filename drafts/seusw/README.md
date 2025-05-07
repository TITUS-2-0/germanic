# Dataset 'Das Buch der Wahrheit'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/mhd/seuswahr/seusw.htm).

* URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/seusw/
* version: unreleased
* date: 2025-03-05

## Citation
```text
Digital version of Das Buch der Wahrheit by Heinrich Seuse (draft version). By: Jost Gippert, Harald Knaus, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/seusw/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Chapter | `div@chapter` | Automatically translated into named div |
| Sentence | `s` |  |

### Structural overview
```text
text (@xml:lang=gmh-Latn-x-mhg)
  body
    div (@data-level=1, @n, @type=chapter, @xml:id) (multiple)
      head (multiple)
        [lb (@n) (multiple)]
      p (@xml:id) (multiple)
        s (@n, @xml:id) (multiple)
          [foreign (@xml:lang=lat-Latn)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="I." xml:id="chapter-1" type="chapter" data-level="1">
				<head>
					<lb n="1"/>Von inrelicher gelazenheite und von guͦtem underscheide, der ze habenne ist in vernunftikeite</head>
				<p xml:id="chapter-1-p-1">
					<s n="2" xml:id="chapter-1-p-1-s-1">
						<foreign xml:lang="lat-Latn">»Ecce enim veritatem dilexisti, incerta et occulta sapientie tue manifestasti michi.«</foreign>
					</s>
					<s n="3" xml:id="chapter-1-p-1-s-2">Es waz ein mensche in Christo, der hatte sich in sinen iungen tagen geuͤbet nach dem ussern menschen uf ellú dú stúke, da sich anvahendú menschen pflegent ze uͤbenne, und beleip aber der inr mensch ungeuͤbt in sin selbs \ nehsten gelazenheit, und bevand wol, daz im neiswaz gebrast, er enwiste aber nit waz.</s>
					<s n="4" xml:id="chapter-1-p-1-s-3">Und do er daz langú zit und vil iaren getreib, do wart im eins males ein inker, in deme er wart getriben zuͦ im selben, und ward in im gesprochen also: Du solt wissen, daz inrlichú gelazenheit bringet den menschen zuͦ der nehsten warheit.</s>
					<s n="5" xml:id="chapter-1-p-1-s-4">Nu waz im dis edel wort dennoch wild und unbekant, und hatte doch vil minne darzuͦ, und wart uf daz selbe und des glich gar vestiklich getriben - ob er vor sime tode iemer dar zuͦ me^ochte komen -, daz er daz selb bloz erkandi und ze grunde ervolgti.</s>
					<s n="6" xml:id="chapter-1-p-1-s-5">Also kam er darzuͦ, daz er wart gewarnet und wart ime fúr geworfen, \ daz in dem schine des selben bildes verborgen legi valscher grunt ungeordenter friheit und bedecket legi grozer schade der heiligen kristenheit.</s>
					<s n="7" xml:id="chapter-1-p-1-s-6">Und hier abe erschrak er und gewan etlich zit einen widerstoz des inren ruͦfes in im selben.</s>
  ...
```
