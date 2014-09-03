# Tiedostoformaatit

Paikkatietokäytössä olevia tiedostoformaatteja on lukuisa määrä. Kulloinkin kytetetty formaatti riippuu aineiston tyypistä, käyttötavasta ja käytettävästä ohjelmistosta. Seuraavassa ohjeistetaan tiedostoformaattien käyttöä avoimien paikkatietojen tiedostopalveluissa. Tällöin ohjeistus kohdistuu yleisimpiin ja oletetut käyttötarpeet parhaiten täyttäviksi arvioituihin formaatteihin.

## Vektoriaineistot

Vektoriaineistojen avoimen datan julkaisuissa suositellaan käytetettäväksi seuraavia formaatteja:

| Kohderyhmä ja käyttötapa: | Formaatti: | Huomautukset: |
| :--------- | :-------: | :--------- |
| Aineiston ammattimainen käyttö ja jatkojalostus | **GIS-ohjelmistojen formaatit** | Yleisimmät Suomessa Shape ja TAB |
| Suuren yleisön katselukäyttö | **KML** | Katso alla |
| Sovelluskehittäjät (web) | **GeoJSON** | Katso alla |

Avoimen datan julkaisuformaatti suositellaan valittavaksi kukin aineiston oletetun käyttäjäkohderyhmän ja käyttötavan mukaan. Ensisijainen minimisuositus on shape-formaatti. Se on yleiskäyttöisin formaatti tiedon tuottajalle ja käyttäjälle ja sen jatkojalostaminen on käyttäjille helpompaa kuin KML- ja GeoJSON-tiedostojen. KML ja GeoJSON ovat kohderyhmilleen helppokäyttöisimpiä ja nopeiten käyttöönotettavia tiedostoformaatteja, mutta näiden pohjalta aineiston muu jatkokäyttö ja -jalostus on hankalampaa kuin perinteisissä paikkatieto-ohjelmien formaateissa.

Aineiston julkaisijan resurssien puitteissa suositellaan julkaistavaksi valmiiksi useampia mahdollisia formaatteja. Kuitenkin valmiiksi tuotettuja useita eri formaattiversioita tärkeämpää on, että data saadaan ylipäätään avatuksi vähintään yhdessä yleisesti tunnetussa ja käyttökelpoisessa formaatissa.

Koordinaatistojen osalta on syytä huomioida, että KML on aina ja GeoJSON:n on oletuksena (ellei muuta määritetä) maantieteellisessä WGS 84 -koordinaatistossa. Lisäksi KML sisältää kohteiden symbologian asetukset GeoJSON:in sisältäessä pelkään datan ilman symbologiaa (ulkoasun määrittely). GIS-ohjelmistojen formaateissa koordinaatiston voi määritellä eri vaihtoehtojen joukosta.

Linkkejä:
* Shape http://en.wikipedia.org/wiki/Shapefile
* TAB http://en.wikipedia.org/wiki/MapInfo_TAB_format
* KML http://en.wikipedia.org/wiki/Keyhole_Markup_Language
* GeoJSON http://en.wikipedia.org/wiki/GeoJSON
* OGC GeoPackage http://www.geopackage.org/


## Vektoriaineistot – Pistekohteet
Tulossa

## Rasteriaineistot
Tulossa

## Laserpisteaineistot
Tulossa

## Muut aineistotyypit
Tulossa

## Toimialakohtaiset standardit
Tulossa

## Formaattimuunnosvälineet
Tulossa

## Kohdeluokitus
Tulossa

## Lyhyesti:
1. Arvioi ja valitse aineiston ja oletetun käyttäjäryhmän mukainen formaatti.
2. Pyri julkaisemaan vähintään yhden formaatin mukainen aineistoversio tiedostona.
3. Käyttäjäpalautteen ja resurssien mukaan pyri laajentamaan aineistojen ja aineistoversioiden (formaatti, koordinaatisto) valikoimaa.
4. Suunnittele aineistojen myöhempi päivitys ja pyri julkaisemaan päivitykset vähintään kerran vuodessa tai kun aineisto on oleellisesti muuttunut
5. Julkaise aineistoja myös rajapintapalveluissa.

-----
[Palaa sisällysluetteloon](Sisällysluettelo.md)
