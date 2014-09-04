# Metatiedot

Avoimen paikkatiedon löytämisen edellytyksenä on, että paikkatietoaineistot ja -palvelut kuvaillaan metatietojen avulla hakupalveluihin. Kuvailun tulee olla yhteentoimiva yleisesti käytettyjen metatietomallien kanssa. Hakupalvelun avulla tiedon potentiaalinen hyödyntäjä voi löytää aineiston ja arvioida sen soveltuvuutta aiottuun tarkoitukseen.Toki yleisten hakukoneidenkin avulla on mahdollista löytää avointa paikkatietoa, mutta tulokset ovat kovin sattumanvaraisia.

Sisällön osalta paikkatietoaineistojen ja -palvelujen kuvailua ohjeistaa kansainvälinen ISO 19115 -standardi. Standardin soveltaminen on ohjeistettu julkisen hallinnon suosituksessa [JHS 158 Paikkatiedon metatiedot](http://www.jhs-suositukset.fi/suomi/jhs158). Keskeisimpiä metatiedoissa esitettäviä asioita paikkatietoaineistoille ja -palveluille ovat:    

| **Metatietoelementti** | **Esimerkki elementin sisällöstä** |
| aineiston tai -palvelun nimi |  |  
| kuvaileva teksti |  |  
|yksilöivä tunniste (aineistot), palvelun URL-osoite (palvelut)||  
|viittaus on-line lähteeseen, josta aineisto on saatavilla (aineistot), viittaukset palvelun kautta saatavilla olevien aineistojen metatietoihin (palvelut)||
|asiasanat (Yleiseen suomalaiseen ontologiaan -liitetyistä asiasanastoista, jos mahdollista)|| 
|maantieteellinen kattavuus (sijaintia rajaava suorakaide - bounding box)||
|ajallinen ulottuvuus (julkaisu, päivitys ym. päivämäärätiedot)|| 
|viittaus käyttölupaan||
|aineistosta/palvelusta sekä metatiedoista vastaavien osapuolten yhteystiedot||
|metatiedon viimeisin päivitysajankohta||  

JHS 158 -suosituksen mukaisten paikkatiedon metatietojen laatiminen ja liittäminen kansalliseen [Paikkatietohakemisto](http://www.paikkatietohakemisto.fi)-hakupalveluun on useille viranomaisille lakisääteinen tehtävä. Paikkatietohakemistossa myös muut kuin lainsäädännön velvoittamat paikkatiedon tuottajat voivat luoda ja ylläpitää paikkatiedon metatietoja. Metatietoja voidaan myös noutaa Paikkatietohakemistoon muista [CSW-rajapintastandardin](http://en.wikipedia.org/wiki/Catalog_Service_for_the_Web) toteuttavista metatietopalveluista. Tällaisia voivat olla esimerkiksi paikalliset, tietyn aihepiirin kattavat tai organisaatiokohtaiset metatietopalvelut kuten Ilmatieteen laitoksen [FMI catalog](http://catalog.fmi.fi).

Valtiovarainministeriö on käynnistänyt osana Avoimen tiedon ohjelmaa dataportaali –projektin, jonka tehtävänä on toteuttaa kansallisia avoimen tiedon metatietoja kokoava [Avoindata.fi](http://www.avoindata.fi) -portaali. Paikkatietohakemistossa julkaistut "avoindata.fi" -avainsanan sisältämät metatiedot noudetaan automaattisesti Avoindata.fi -palveluun.

## Lyhyesti:
1. Laadi avoimelle paikkatietoaineistolle ja sitä tarjoavalle palvelulle kansallisten suositusten mukaiset tiedot sisältävät metatietokuvailut
2. [Julkaise](Julkaiseminen.md) metatiedot Paikkatietohakemistossa tai ilmoita ylläpidolle rajapinnan osoite, josta metatiedot ovat noudettavissa
3. Lisäämällä "avoindata.fi" -avainsanan Paikkatietohakemistossa oleviin metatietoihin saat avoimet aineistosi ja palvelusi näkyville kansalliseen Avoindata.fi -palveluun

-----
[Palaa sisällysluetteloon](Sisällysluettelo.md)
