EST: XBRL GL Taksonoomia laiendus (EE-Extension 2026-03-31)

Laiendusega lisanduvad järgmised andmeväljad andmekirjesse:

1. entrySourceId (string, optional). Andmeallika ID. Kasutatakse juhul kui andmeid saadetakse mitmest allikast.
2. entrySourceCount (int, optional). Andmeallikate arv kokku.
3. periodExtraIdentifier (string, optional). Sama perioodi sees esitatavate tehingute anmete eristamiseks (nt pankroti protsessi tehingute eristamiseks).
4. identifierEmployeeCategory (string, optional). Vabatekstiline väli töötaja kategooria täpsustamiseks.
5. identifierBirthDate (date, optional). Eraisiku sünnikuupäev.
6. entryVersion (string, optional) Andmesektioonile versioonile viide. Kui ei saadeta versiooni infot, siis vaikimisi versioon 1.0

Lisatud andmeväljad asuvad kaustas: 
EE-Extension/XBRL-GL-REC-2015-03-25/gl/ext/

Laiendustega andmefaili näidis asub kaustas:
EE-Extension/XBRL-GL-REC-2015-03-25/gl/ids/

Valideerimiseks tuleb kasutada schemat:
EE-Extension/XBRL-GL-REC-2015-03-25/gl/plt/case-c-b-m-e/gl-plt-2015-03-25.xsd

Laiendustest on mõjutatud järgnevad schemad:
gl-cor-content-2015-03-25.xsd
gl-ext-content-2026-03-31.xsd

ENG: XBRL GL Taxonomy Extension (EE-Extension 2026-03-31)

The extension adds the following fields to data entry:

1. entrySourceId (string, optional). Data source ID. Used when data is sent from multiple sources.
2. entrySourceCount (int, optional). Total number of data sources.
3. periodExtraIdentifier (string, optional). For distinguishing transaction data submitted within the same period (e.g., for distinguishing bankruptcy process transactions).
4. identifierEmployeeCategory (string, optional). Free text field for specifying employee category.
5. identifierBirthDate (date, optional). Private person's birth date.
6. entryVersion (string, optional). Reference to data section version. If no version info is sent, defaults to version 1.0

The added data fields are located in folder:
EE-Extension/XBRL-GL-REC-2015-03-25/gl/ext/

A sample data file with extensions is located in folder:
EE-Extension/XBRL-GL-REC-2015-03-25/gl/ids/

For validation, use the schema:
EE-Extension/XBRL-GL-REC-2015-03-25/gl/plt/case-c-b-m-e/gl-plt-2015-03-25.xsd

The following schemas are affected by the extensions:
gl-cor-content-2015-03-25.xsd
gl-ext-content-2026-03-31.xsd
