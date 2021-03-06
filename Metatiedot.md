# Metatiedot

Avoimen paikkatiedon löytämisen edellytyksenä on, että paikkatietoaineistot ja -palvelut kuvaillaan metatietojen avulla hakupalveluihin. Kuvailun tulee olla yhteentoimiva yleisesti käytettyjen metatietomallien kanssa. Hakupalvelun avulla tiedon potentiaalinen hyödyntäjä voi löytää aineiston ja arvioida sen soveltuvuutta aiottuun tarkoitukseen.Toki yleisten hakukoneidenkin avulla on mahdollista löytää avointa paikkatietoa, mutta tulokset ovat kovin sattumanvaraisia.

Sisällön osalta paikkatietoaineistojen ja -palvelujen kuvailua ohjeistaa kansainvälinen ISO 19115 -standardi. Standardin soveltaminen on ohjeistettu julkisen hallinnon suosituksessa [JHS 158 Paikkatiedon metatiedot](http://www.jhs-suositukset.fi/suomi/jhs158). Keskeisimpiä metatiedoissa esitettäviä asioita paikkatietoaineistoille ja -palveluille ovat:    

**Metatietoelementti** | **Esimerkki elementin sisällöstä** 
---------------------- | -------------------------------------
Aineiston tai -palvelun nimi |  *Kuntajako*  
Kuvaileva teksti | *Kuntajako on Maanmittauslaitoksen kerran vuodessa tuottama koko Suomen kuntajakoa kuvaava aineisto, josta tehdään vektori- ja rasterimuotoiset tuotteet...* 
Yksilöivä tunniste (aineistot), palvelun URL-osoite (palvelut) | *FI.100314* 
|Viittaus on-line lähteeseen, josta aineisto on saatavilla (aineistot), viittaukset palvelun kautta saatavilla olevien aineistojen metatietoihin (palvelut) | *http://www.maanmittauslaitos.fi/digituotteet/kuntajako*
Asiasanat (Yleiseen suomalaiseen ontologiaan -liitetyistä asiasanastoista, jos mahdollista)| *Hallinnolliset yksiköt, avoindata.fi* 
Maantieteellinen kattavuus (sijaintia rajaava suorakaide - bounding box) | *19.08317359,31.58672881,59.45414258,70.09229553(EPSG:4326)*
Ajallinen ulottuvuus (julkaisu, päivitys ym. päivämäärätiedot) | *2011-10-12(Luonti)* 
Viittaus käyttölupaan| *http://www.maanmittauslaitos.fi/avoindata_lisenssi_versio1_20120501*
Aineistosta/palvelusta sekä metatiedoista vastaavien osapuolten yhteystiedot | *Maanmittauslaitos,sähköpostiosoite*
Metatiedon viimeisin päivitysajankohta | *2014-05-15T16:27:48*  

JHS 158 -suosituksen mukaisten paikkatiedon metatietojen laatiminen ja liittäminen kansalliseen [Paikkatietohakemisto](http://www.paikkatietohakemisto.fi)-hakupalveluun on useille viranomaisille lakisääteinen tehtävä. Paikkatietohakemistossa myös muut kuin lainsäädännön velvoittamat paikkatiedon tuottajat voivat luoda ja ylläpitää paikkatiedon metatietoja. Metatietoja voidaan myös noutaa Paikkatietohakemistoon muista [CSW-rajapintastandardin](http://en.wikipedia.org/wiki/Catalog_Service_for_the_Web) toteuttavista metatietopalveluista. Tällaisia voivat olla esimerkiksi paikalliset, tietyn aihepiirin kattavat tai organisaatiokohtaiset metatietopalvelut kuten Ilmatieteen laitoksen [FMI catalog](http://catalog.fmi.fi).

Valtiovarainministeriö on käynnistänyt osana Avoimen tiedon ohjelmaa dataportaali –projektin, jonka tehtävänä on toteuttaa kansallisia avoimen tiedon metatietoja kokoava [Avoindata.fi](http://www.avoindata.fi) -portaali. Paikkatietohakemistossa julkaistut "avoindata.fi" -avainsanan sisältämät metatiedot noudetaan automaattisesti Avoindata.fi -palveluun.

## Lyhyesti:
1. Laadi avoimelle paikkatietoaineistolle ja sitä tarjoavalle palvelulle kansallisten suositusten mukaiset tiedot sisältävät metatietokuvailut
2. [Julkaise](Julkaiseminen.md) metatiedot Paikkatietohakemistossa tai ilmoita ylläpidolle rajapinnan osoite, josta metatiedot ovat noudettavissa
3. Lisäämällä "avoindata.fi" -avainsanan Paikkatietohakemistossa oleviin metatietoihin saat avoimet aineistosi ja palvelusi näkyville kansalliseen Avoindata.fi -palveluun

-----
[Palaa sisällysluetteloon](Sisällysluettelo.md)
