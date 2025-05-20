# Dataset 'Predigten'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/mhd/berthreg/berth.htm).

* URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/berth/
* version: unreleased
* date: 2025-03-04

## Citation
```text
Digital version of Predigten by Berthold von Regensburg (draft version). By: Jost Gippert, Harald Knaus, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/berth/, visited on <insert date>)
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
      head (@xml:lang=deu-Latn | lat-Latn) (multiple)
      head (multiple)
      p (@xml:id) (multiple)
        s (@n, @xml:id) (multiple)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="2" xml:id="chapter-1" type="chapter" data-level="1">
				<head xml:lang="deu-Latn">1. Predigt</head>
				<head>Die ander.
Von den funf phunden</head>
				<head xml:lang="lat-Latn">D[n]e quinque talenta</head>
				<p xml:id="chapter-1-p-1">
					<s n="4" xml:id="chapter-1-p-1-s-1">Wer ist der wîse kneht, der getriuwe kneht, dem sîn herre sîn guot enpfalch, und er im dâ mit getriuwelîche wirbet, sô sprichet er: 'nû wis frô, getriuwer kneht, dû bist getriuwe gewesen über ein wenic guotes, unde dar umbe wil ich dich nû setzen über allez mîn guot.</s>
					<s n="5" xml:id="chapter-1-p-1-s-2">Nû wis frô, getriuwer kneht!</s>
					<s n="6" xml:id="chapter-1-p-1-s-3">gang in die freude dînes herren': wer ist nû dirre wîse kneht unde der getriuwe kneht?</s>
					<s n="7" xml:id="chapter-1-p-1-s-4">Den dürfen wir niht verre suochen: daz ist der guote sant Alexius, des tac man hiute an etelîcher stat begêt in der kristenheit.</s>
					<s n="8" xml:id="chapter-1-p-1-s-5">Wan er ist ein nôthelfer unde was eins fürsten sun von Rôme, ein rehter Rômaere, und ez hete sîn vater grôze rîcheit, und er gab im eine gemahelen.</s>
					<s n="9" xml:id="chapter-1-p-1-s-6">Von der lief er und wolte gote dienen unde daz ewige leben erwerben.</s>
  ...
```
