# Dataset 'The Middle High German Books on The Great Alexander: Basler Alexander'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/mhd/a_basler/a_bas.htm).

* URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/a_bas/
* version: unreleased
* date: 2025-03-05

## Citation
```text
Digital version of The Middle High German Books on The Great Alexander: Basler Alexander by Lamprecht (draft version). By: Jost Gippert, Stefanie Heine, Florian Matter, Daniela Reichert, Ralf Schlechtweg-Jahn. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/a_bas/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Chapter | `div@chapter` | Automatically translated into named div |
| Verse | `l` |  |
| Author | `div@author` | Automatically translated into named div |
| Version | `div@version` | Automatically translated into named div |

### Structural overview
```text
text (@xml:lang=gmh-Latn-x-mhg)
  body
    div (@data-level=1, @n, @type=chapter, @xml:id) (multiple)
      head (@xml:lang=deu-Latn) (multiple)
      div (@data-level=2, @xml:id) (multiple)
        l (@n, @xml:id) (multiple)
      div (@data-level=2, @xml:id) (multiple)
        p (@xml:id) (multiple)
          ref (@target=lxtext=A_BASLER&lx1=Alex.&lx2=180 | lxtext=A_BASLER&lx1=Alex.&lx2=180w | lxtext=A_BASLER&lx1=Alex.&lx2=190 | lxtext=A_BASLER&lx1=Alex.&lx2=190w | lxtext=A_BASLER&lx1=Alex.&lx2=84 | lxtext=A_BASLER&lx1=Alex.&lx2=84f, @xml:id) (multiple)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="2" xml:id="chapter-1" type="chapter" data-level="1">
				<head xml:lang="deu-Latn">Nectanabus wird aus Ägypten vertrieben</head>
				<div xml:id="chapter-1-div-1" data-level="2">
					<l n="1" xml:id="chapter-1-div-1-l-1">[Z]uͦ Egiptten Nectanibus küng was,</l>
					<l n="2" xml:id="chapter-1-div-1-l-2">als ich von im geschriben las;</l>
					<l n="3" xml:id="chapter-1-div-1-l-3">in astronimy sinem rich</l>
					<l n="4" xml:id="chapter-1-div-1-l-4">was er und sin gelich</l>
					<l n="5" xml:id="chapter-1-div-1-l-5">niendert noch in nigramacye</l>
					<l n="6" xml:id="chapter-1-div-1-l-6">die wont im eigentlichen by.</l>
					<l n="7" xml:id="chapter-1-div-1-l-7">eins tages kam es also</l>
					<l n="8" xml:id="chapter-1-div-1-l-8">daz dem künge Nettanibo</l>
					<l n="9" xml:id="chapter-1-div-1-l-9">botten wurden gesant</l>
  ...
```
