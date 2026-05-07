EST: XBRL GL Taksonoomia laiendus (EE-Extension 2026-03-31)

Nimeruumid (namespaces):
- gl-ext: https://xbrl.eesti.ee/XBRL-GL-EXT-2026-03-31
- gl-plt: https://xbrl.eesti.ee/XBRL-GL-EXT-2026-03-31/plt
- gl-cor, gl-bus, gl-muc, gl-gen: standardne XBRL GL (http://www.xbrl.org/int/gl/...)

Laiendusega lisanduvad järgmised andmeväljad andmekirjesse:

1. entrySourceId (string, optional). Andmeallika ID. Kasutatakse juhul kui andmeid saadetakse mitmest allikast.
2. entrySourceCount (int, optional). Andmeallikate arv kokku.
3. periodExtraIdentifier (string, optional). Sama perioodi sees esitatavate tehingute andmete eristamiseks (nt pankroti protsessi tehingute eristamiseks).
4. identifierEmployeeCategory (string, optional). Vabatekstiline väli töötaja kategooria täpsustamiseks.
5. identifierBirthDate (date, optional). Eraisiku sünnikuupäev.
6. entryVersion (string, optional). Andmesektsioonile versioonile viide. Kui ei saadeta versiooni infot, kasutatakse vaikimisi versiooni 1.0 (vaikeväärtus rakendub andmete vastuvõtja poolel).

Lisatud andmeväljad asuvad kaustas:
gl/ext/

Laiendustega andmefailide näidised asuvad kaustas:
gl/ids/
- MTA_KMD_APA_XBRL_GL_naidis_20260427.xml (KMD APA näidis, valideerub schema'ga case-c-b-e)
- SA_PALK_XBRLGL_XML_naidis_20241211_ext.xml (palga ja tööjõu näidis, valideerub schema'ga case-c-b-m-e)

Valideerimiseks kasutatavad schemad (entry points):
- gl/plt/case-c-b-e/gl-plt-2026-03-31.xsd
  (cor + bus + ext, ilma muc-ta — KMD APA jaoks)
- gl/plt/case-c-b-m-e/gl-plt-2026-03-31.xsd
  (cor + bus + muc + ext — palga ja tööjõu andmete jaoks)

Laiendustest on mõjutatud järgnevad schemad:
- gl-cor-content-2026-03-31.xsd
- gl-ext-content-2026-03-31.xsd

Näide xsi:schemaLocation ja schemaRef kasutamisest XML failis:
  <xbrll:schemaRef xlink:href="https://xbrl.eesti.ee/XBRL-GL-EXT-2026-03-31/gl/plt/case-c-b-e/gl-plt-2026-03-31.xsd" xlink:arcrole="http://www.w3.org/1999/xlink/properties/linkbase" xlink:type="simple"/>
  xsi:schemaLocation="https://xbrl.eesti.ee/XBRL-GL-EXT-2026-03-31 https://xbrl.eesti.ee/XBRL-GL-EXT-2026-03-31/gl/plt/case-c-b-e/gl-plt-2026-03-31.xsd"
Nimeruumi URI (https://xbrl.eesti.ee/XBRL-GL-EXT-2026-03-31) on identifikaator, mitte allalaadimise URL — see jääb alati samaks.


ENG: XBRL GL Taxonomy Extension (EE-Extension 2026-03-31)

Namespaces:
- gl-ext: https://xbrl.eesti.ee/XBRL-GL-EXT-2026-03-31
- gl-plt: https://xbrl.eesti.ee/XBRL-GL-EXT-2026-03-31/plt
- gl-cor, gl-bus, gl-muc, gl-gen: standard XBRL GL (http://www.xbrl.org/int/gl/...)

The extension adds the following fields to data entry:

1. entrySourceId (string, optional). Data source ID. Used when data is sent from multiple sources.
2. entrySourceCount (int, optional). Total number of data sources.
3. periodExtraIdentifier (string, optional). For distinguishing transaction data submitted within the same period (e.g., bankruptcy process transactions).
4. identifierEmployeeCategory (string, optional). Free text field for specifying employee category.
5. identifierBirthDate (date, optional). Private person's birth date.
6. entryVersion (string, optional). Reference to data section version. If no version info is sent, version 1.0 is assumed (the default is applied on the receiver side).

The added data fields are located in folder:
gl/ext/

Sample data files with extensions are located in folder:
gl/ids/
- MTA_KMD_APA_XBRL_GL_naidis_20260427.xml (KMD APA sample, validates against case-c-b-e)
- SA_PALK_XBRLGL_XML_naidis_20241211_ext.xml (payroll/labour cost sample, validates against case-c-b-m-e)

Validation entry-point schemas:
- gl/plt/case-c-b-e/gl-plt-2026-03-31.xsd
  (cor + bus + ext, no muc — used for KMD APA)
- gl/plt/case-c-b-m-e/gl-plt-2026-03-31.xsd
  (cor + bus + muc + ext — used for payroll/labour cost data)

Schemas affected by the extensions:
- gl-cor-content-2026-03-31.xsd
- gl-ext-content-2026-03-31.xsd

Example of xsi:schemaLocation and schemaRef usage in an XML file:
  <xbrll:schemaRef xlink:href="https://xbrl.eesti.ee/XBRL-GL-EXT-2026-03-31/gl/plt/case-c-b-e/gl-plt-2026-03-31.xsd" xlink:arcrole="http://www.w3.org/1999/xlink/properties/linkbase" xlink:type="simple"/>
  xsi:schemaLocation="https://xbrl.eesti.ee/XBRL-GL-EXT-2026-03-31 https://xbrl.eesti.ee/XBRL-GL-EXT-2026-03-31/gl/plt/case-c-b-e/gl-plt-2026-03-31.xsd"
The namespace URI (https://xbrl.eesti.ee/XBRL-GL-EXT-2026-03-31) is an identifier, not a download URL — it always stays the same.
