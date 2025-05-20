

### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Chapter | `div@chapter` | Automatically translated into named div |
| Page | `pb@edition-king[main='yes']` |  |
| Line | `lb@edition-king[main='yes']` |  |
| Manuscript page | `pb@manuscript` |  |
| Manuscript line | `lb@manuscript` |  |
| Page ed. Piper | `pb@edition-pip` |  |
| Sec. ms. page | `pb@manuscript-2` |  |
| Tert. ms. page | `pb@manuscript-3` |  |

### Structural overview
```text
text (@xml:lang=goh-Latn)
  body
    div (@data-level=1, @n, @type=chapter, @xml:id) (multiple)
      p (@xml:id) (multiple)
        [lb (@main=yes, @n, @type=edition-king) (multiple)]
        [lb (@n, @type=manuscript) (multiple)]
        [foreign (@xml:lang=lat-Latn) (multiple)]
        [lb (@break=no, @main=yes, @n, @type=edition-king) (multiple)]
        [pb (@facs=#K296r | #K296v | #K297r | #L60va | #L60vb | #L61rb | #L61va, @n, @type=manuscript-2) (multiple)]
        [lb (@break=no, @n, @type=manuscript) (multiple)]
        [pb (@main=yes, @n, @type=edition-king) (multiple)]
        [pb (@break=no, @n, @type=edition-pip)]
        [pb (@n, @type=edition-pip | manuscript-3) (multiple)]
        [pb (@break=no, @facs=#L61vb, @n, @type=manuscript-2)]
      [pb (@main=yes, @n, @type=edition-king) (multiple)]
      [pb (@n, @type=edition-pip)]
      [pb (@facs=#K295v | #L60rb | #L61ra | #N50v_1, @n, @type=manuscript-2) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="chapter-1" type="chapter" data-level="1">
				<pb main="yes" type="edition-king" n="331"/>
				<pb type="edition-pip" n="851"/>
				<pb type="manuscript-2" n="L60rb" facs="#L60rb"/>
				<pb type="manuscript-2" n="K295v" facs="#K295v"/>
				<p xml:id="chapter-1-p-1">
					<lb main="yes" type="edition-king" n="35"/>
					<lb type="manuscript" n="35"/>An_demo <foreign xml:lang="lat-Latn">regulari monachordo</foreign>
					<lb main="yes" type="edition-king" n="36"/>
					<lb type="manuscript" n="36"/>uuerden ze erist finf-zehen buohsta-<lb main="yes" type="edition-king" n="37" break="no"/>
					<lb type="manuscript" n="37"/>ba . fure also manigen seitun . unte<pb type="manuscript-2" n="L60va" facs="#L60va"/>
					<lb main="yes" type="edition-king" n="1"/>
  ...
```
