

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
