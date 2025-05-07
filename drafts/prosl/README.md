# Dataset 'Prosalancelot'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/germ/mhd/proslan1/prosl.htm).

* URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/prosl/
* version: unreleased
* date: 2025-03-05

## Citation
```text
Digital version of Prosalancelot (draft version). By: Jost Gippert, Harald Knaus, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/germanic/tree/main/drafts/prosl/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Sentence | `s` |  |
| Page | `pb` |  |

### Structural overview
```text
text (@xml:lang=gmh-Latn-x-mhg)
  body
    div (@data-level=1, @type=book, @xml:id) (multiple)
      head (@xml:lang=deu-Latn) (multiple)
      p (@xml:id) (multiple)
        s (@n, @xml:id) (multiple)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" xml:id="book-1" type="book" data-level="1">
				<head xml:lang="deu-Latn">DIE SCHMERZENREICHE KÖNIGIN</head>
				<p xml:id="book-1-p-1">
					<s n="1" xml:id="book-1-p-1-s-1">In der marcken von Galla und von der Mynnren Brytanien warn zwen konig by alten zyten, die waren gebrudere von vatter und von mutter, und sie hatten zwo schwester zu wybe.</s>
					<s n="2" xml:id="book-1-p-1-s-2">Der eyn von den zweyn konigen hieß Ban, und der ander konig was geheyßen Bohort von Gaules; und der konig Ban was ein alt man, und syn wyp was ein junge frauw und was von all der welt geminnet.</s>
					<s n="3" xml:id="book-1-p-1-s-3">Und sie hatten nymant miteinander gewunnen dann ein junges knebelin kleyn, und was geheißen Lancelot syn zuname, wann er was getauffet Galaad; und wie er ward geheißen Lancelot, das sol das buch vil wol hernach gesagen, wann wir haben es yczo keyn stadt, wann wir múßen nu volgen der gerechten zal als wir begunnen han.</s>
					<s n="4" xml:id="book-1-p-1-s-4">Sie spricht das der konig Ban hett ein nachgebur, des lant an syn lant stieß an die syten zu Berrone wert, das da was geheißen das Wúst Lant; und syn nachgebur was geheißen Claudas, und der was herre von Bohorges und von dem land allumb.</s>
					<s n="5" xml:id="book-1-p-1-s-5">Der Claudas was ein konig und was vil gut riechter und vil wise und was ein verreter und was man des koniges von Gaune, das man nu heißet Franckrich.</s>
					<s n="6" xml:id="book-1-p-1-s-6">Das lant von Claudas rych was geheißen Wúste, wann es allein gewústet was von Uterpandragone und von Aramunde, der da was herre von Wenigen Brytanien, das da hieß Hocri zu zunamen.</s>
					<s n="7" xml:id="book-1-p-1-s-7">Der Aramunt hatt under im Gaune und Bonewig und alles das lant biß an die marck von Alverne und von Galbonie, und solt under im haben das rych von Bohorges, wann Claudas engunde es im nicht noch enwolt im dheynen dienst geben, wann er haßset den konig von Gaune.</s>
					<s n="8" xml:id="book-1-p-1-s-8">Und zu den zyten was Gaule underthan zu Rome und gab dar dienst.</s>
					<s n="9" xml:id="book-1-p-1-s-9">Da enwart nymand konig, er enwúrd darzu erkorne.</s>
  ...
```
