# Dataset 'Minor Old Saxon Monuments'

![Static Badge](https://img.shields.io/badge/TEI_validation-failing-red)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/asachs/klasdkm/klasd.htm).

* URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/klasd/
* version: unreleased
* date: 2025-01-11

## Citation
```text
Digital version of Minor Old Saxon Monuments (draft version). By: Jost Gippert, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/klasd/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Text | `div@text` | Automatically translated into named div |
| Page | `pb` |  |
| Line | `lb` |  |
| Section | `div@section` | Automatically translated into named div |
| Paragraph | `div@paragraph` | Automatically translated into named div |
| Manuscript | `div@manuscript` | Automatically translated into named div |
| Ms. page | `pb@manuscript` |  |
| Ms. line | `lb@manuscript` |  |

### Structural overview
```text
text (@xml:lang=osx-Latn)
  body
    div (@data-level=1, @n, @type=text, @xml:id) (multiple)
      div (@data-level=3, @type=manuscript | paragraph | section, @xml:id) (multiple)
      [pb (@n) (multiple)]
      [foreign (@xml:lang=deu-Latn | lat-Latn) (multiple)]
        facsimile (@xml:id) (multiple)
          surface (@xml:id) (multiple)
            graphic (@url=contra_nessia_spurih_2_Dorow_Denkmaeler_Anh_2.jpg | gallee_IIIb_Essen_Heberolle.jpg | gallee_IIIc_Duess_Beda_Hom.jpg | gallee_IIId_Duess_Beichte.jpg | gallee_VI_Wien_Beschw_188.jpg | gallee_XIIb_Sang_878_321_facs_Arx.jpg | gallee_XIa_Vatic_577_6b.jpg | http://web.uni-marburg.de/hosting/mr/mrfd/Trier_SB_Hs_40_1018_8%b0_Bl_19v.jpg | http://www.e-codices.unifr.ch/de/csg/0878/321/medium) (multiple)
        [foreign (@xml:lang=deu-Latn) (multiple)]
      [lb (@n) (multiple)]
      [pb (@type=manuscript) (multiple)]
      [pb (@n, @type=manuscript) (multiple)]
    div (@data-level=1, @n, @type=text, @xml:id)
      div (@data-level=3, @type=manuscript | paragraph | section, @xml:id) (multiple)
      facsimile (@xml:id)
        surface (@xml:id)
          graphic (@url=gallee_IXa_Bernb_Dess_1a_5-11.jpg)
      [pb (@n) (multiple)]
      [foreign (@xml:lang=deu-Latn) (multiple)]
      [pb (@n, @type=manuscript) (multiple)]
      [lb (@n) (multiple)]
      [pb (@type=manuscript)]
    div (@data-level=1, @n, @type=text, @xml:id)
      facsimile (@xml:id)
        surface (@xml:id)
          graphic (@url=ielithes.jpg)
      [foreign (@xml:lang=deu-Latn)]
      [pb (@n)]
      [lb (@n) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="Schs.Taufgel." xml:id="text-1" type="text" data-level="1">
				<pb n="W3"/>
				<div xml:id="text-1-manuscript-1" type="manuscript" data-level="3">Vat.lat._577</div>
				<foreign xml:lang="deu-Latn">I. Taufgelöbnis</foreign>
				<foreign xml:lang="deu-Latn">Cod. Pal. (Vatic.). lat. 577, p. 6 <foreign xml:lang="deu-Latn">v</foreign>
					<facsimile xml:id="text-1-facsimile-1">
						<surface xml:id="text-1-facsimile-1-surface-1">
							<graphic url="gallee_XIa_Vatic_577_6b.jpg"/>
						</surface>
					</facsimile>
				</foreign>
				<lb n="3"/>
  ...
```
