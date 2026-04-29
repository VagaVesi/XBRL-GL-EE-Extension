# XBRL GL taksonoomia laiendus (EE-Extension 2026-03-31)

[Avaleht](https://xbrl.eesti.ee/) / XBRL GL taksonoomia laiendus 2026-03-31

## Mis on XBRL GL?

XBRL GL (Global Ledger Taxonomy Framework) on rahvusvaheline standardne
taksonoomia detailsete raamatupidamise ja äritehingute andmete vahetamiseks.
Erinevalt aruandluse-kesksetest XBRL taksonoomiatest on XBRL GL mõeldud
tehingu-tasemel andmete (pearaamatu kanded, palgaarvestus, müügi- ja ostuarved
jms) struktureeritud edastamiseks süsteemide vahel või andmete vastuvõtjale.

Lisainformatsioon ametlikult XBRL Internationalilt:
<https://www.xbrl.org/the-standard/what/gl/>

Käesolev laiendus põhineb XBRL GL REC 2015-03-25 versioonil ja on kohandatud
Eesti aruandluse vajadustele (nt MTA KMD APA, SA palk ja tööjõud).

## Laienduse kohta

### Nimeruumid (namespaces)

- `gl-ext`: `https://xbrl.eesti.ee/gl/ext/2026-03-31`
- `gl-plt`: `https://xbrl.eesti.ee/gl/plt/2026-03-31`
- `gl-cor`, `gl-bus`, `gl-muc`, `gl-gen`: standardne XBRL GL
  (`http://www.xbrl.org/int/gl/...`)

### Lisanduvad andmeväljad

- `entrySourceId` (string, optional) — andmeallika ID. Kasutatakse juhul kui
  andmeid saadetakse mitmest allikast.
- `entrySourceCount` (int, optional) — andmeallikate arv kokku.
- `periodExtraIdentifier` (string, optional) — sama perioodi sees esitatavate
  tehingute andmete eristamiseks (nt pankroti protsessi tehingute eristamiseks).
- `identifierEmployeeCategory` (string, optional) — vabatekstiline väli töötaja
  kategooria täpsustamiseks.
- `identifierBirthDate` (date, optional) — eraisiku sünnikuupäev.
- `entryVersion` (string, optional) — andmesektsiooni versioonile viide. Kui ei
  saadeta versiooni infot, kasutatakse vaikimisi versiooni 1.0 (vaikeväärtus
  rakendub andmete vastuvõtja poolel).

### Valideerimiseks kasutatavad schemad (entry points)

- `2026-03-31/gl/plt/case-c-b-e/gl-plt-2026-03-31.xsd`
  cor + bus + ext, ilma muc-ta — KMD APA jaoks
- `2026-03-31/gl/plt/case-c-b-m-e/gl-plt-2026-03-31.xsd`
  cor + bus + muc + ext — palga ja tööjõu andmete jaoks

### Näidisfailid

- [MTA_KMD_APA_XBRL_GL_naidis_20260427.xml](2026-03-31/gl/ids/MTA_KMD_APA_XBRL_GL_naidis_20260427.xml)
  — KMD APA näidis (valideerub case-c-b-e)
- [SA_PALK_XBRLGL_XML_naidis_20241211_ext.xml](2026-03-31/gl/ids/SA_PALK_XBRLGL_XML_naidis_20241211_ext.xml)
  — palga ja tööjõu näidis (valideerub case-c-b-m-e)

### Näide xsi:schemaLocation kasutamisest

```xml
xsi:schemaLocation="https://xbrl.eesti.ee/gl/plt/2026-03-31 ../plt/case-c-b-e/gl-plt-2026-03-31.xsd"
```

### Avaldamise märkus

Näidisfailides on `schemaRef` ja `xsi:schemaLocation` hrefid suhtelised teed,
mis töötavad ainult lokaalse kausta struktuuriga. Kui taksonoomia on avaldatud
aadressil `https://xbrl.eesti.ee/gl/...`, peavad andmete edastajad asendama
suhtelised teed absoluutsete URLidega:

```xml
<xbrll:schemaRef xlink:href="https://xbrl.eesti.ee/gl/ext/2026-03-31/gl/plt/case-c-b-e/gl-plt-2026-03-31.xsd" .../>
xsi:schemaLocation="https://xbrl.eesti.ee/gl/plt/2026-03-31 https://xbrl.eesti.ee/gl/ext/2026-03-31/gl/plt/case-c-b-e/gl-plt-2026-03-31.xsd"
```

Nimeruumi URI (`https://xbrl.eesti.ee/gl/plt/2026-03-31`) jääb samaks — see on
identifikaator, mitte allalaadimise URL.

---

**Allalaadimine:** Kogu taksonoomia laiendus pakitud kujul —
[xbrl-gl-ee-ext-2026-03-31.zip](zip/xbrl-gl-ee-ext-2026-03-31.zip)

Täielik tehniline kirjeldus: [README.txt](README.txt)

---

*XBRL GL EE-Extension 2026-03-31*
