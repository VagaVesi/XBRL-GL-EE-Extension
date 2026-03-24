EST: XBRL GL Taksonoomia laiendus

Lisandunud on viis lisavälja:
- identifierCodeType (string, optional) - identifitseeriva koodi liik (võimalik väljade loetelu klassifikaatoris)
- transactionPartyType (string, optional) - tehingu osapoole liik (võimalik väljade loetelu klassifikaatoris)
- sourceId (string, optional) - andmeallika id
- version (string, optional) - viide andmesektsiooni kirjelduse versioonile
- isApproved (boolean, optional) - andmesektsiooni kinnitamise info
Lisandunud 2026-03:
- additionalCategory - isikule täiendava tekstilise väljana kategooria lisamine


Lisatud väljad asuvad kaustas: 
EU-Extension/XBRL-GL-REC-2015-03-25/gl/ext/

Laiendustega andmefaili näidis asub kaustas:
EU-Extension/XBRL-GL-REC-2015-03-25/gl/ids/

Valideerimiseks tuleb kasutada schemat:
EU-Extension/XBRL-GL-REC-2015-03-25/gl/plt/case-c-b-m-e/gl-plt-2015-03-25.xsd

Laiendustest on mõjutatud järgnevad schemad:
gl-bus-content-2015-03-25.xsd
gl-cor-content-2015-03-25.xsd
gl-ext-content-2015-03-25.xsd

ENG: XBRL GL Taksonomy extension 

Four additional fields have been added:
- identifierCodeType (string, optional) - type of identification code 
- transactionPartyType (string, optional) - type of transaction party 
- sourceId (string, optional) - data source id if multiple sources
- version (string, optional) - reference to dataset version if several versions
- isApproved (boolean, optional) - bit fo dataset approval


The added fields are located in the folder:
EU-Extension/XBRL-GL-REC-2015-03-25/gl/ext/

A sample data file with extensions is located in the folder:
EU-Extension/XBRL-GL-REC-2015-03-25/gl/ids/

The schema must be used for validation:
EU-Extension/XBRL-GL-REC-2015-03-25/gl/plt/case-c-b-m-e/gl-plt-2015-03-25.xsd

The following schemas are affected by the extensions:
gl-bus-content-2015-03-25.xsd
gl-cor-content-2015-03-25.xsd
gl-ext-content-2015-03-25.xsd

Extension draft updated at 03.04.2025 by Kaido Vetevoog