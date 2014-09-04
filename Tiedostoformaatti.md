# Tiedostoformaatit

Paikkatietokäytössä olevia tiedostoformaatteja on lukuisa määrä. Kulloinkin kytetetty formaatti riippuu aineiston tyypistä, käyttötavasta ja käytettävästä ohjelmistosta. Seuraavassa ohjeistetaan tiedostoformaattien käyttöä avoimien paikkatietojen tiedostopalveluissa. Tällöin ohjeistus kohdistuu yleisimpiin ja oletetut käyttötarpeet parhaiten täyttäviksi arvioituihin formaatteihin.

## Vektoriaineistot

Vektoriaineistojen avoimen datan julkaisuissa suositellaan käytetettäväksi seuraavia formaatteja:

| Kohderyhmä ja käyttötapa: | Formaatti: | Huomautukset: |
| :--------- | :-------: | :--------- |
| Aineiston ammattimainen käyttö ja jatkojalostus | **GIS-ohjelmistojen formaatit** | Yleisimmät Suomessa Shape ja TAB |
| Suuren yleisön katselukäyttö | **KML** | Katso alla |
| Sovelluskehittäjät (web) | **GeoJSON** | Katso alla |

Avoimen datan julkaisuformaatti suositellaan valittavaksi kunkin aineiston oletetun käyttäjäkohderyhmän ja käyttötavan mukaan. Ensisijainen minimisuositus on shape-formaatti. Se on yleiskäyttöisin formaatti tiedon tuottajalle ja käyttäjälle ja sen jatkojalostaminen on käyttäjille helpompaa kuin KML- ja GeoJSON-tiedostojen. KML ja GeoJSON ovat kohderyhmilleen helppokäyttöisimpiä ja nopeiten käyttöönotettavia tiedostoformaatteja, mutta näiden pohjalta aineiston muu jatkokäyttö ja -jalostus on hankalampaa kuin perinteisissä paikkatieto-ohjelmien formaateissa.

Aineiston julkaisijan resurssien puitteissa suositellaan julkaistavaksi valmiiksi useampia mahdollisia formaatteja. Kuitenkin valmiiksi tuotettuja useita eri formaattiversioita tärkeämpää on, että data saadaan ylipäätään avatuksi vähintään yhdessä yleisesti tunnetussa ja käyttökelpoisessa formaatissa.

Koordinaatistojen osalta on syytä huomioida, että KML on aina ja GeoJSON:n on oletuksena (ellei muuta määritetä) maantieteellisessä WGS 84 -koordinaatistossa. Lisäksi KML sisältää kohteiden symbologian asetukset GeoJSON:in sisältäessä pelkään datan ilman symbologiaa (ulkoasun määrittely). GIS-ohjelmistojen formaateissa koordinaatiston voi määritellä eri vaihtoehtojen joukosta. GIS-formaateista TAB-sisältää symbologian ja shape ei sisällä symbologiaa.

**GML** ja **OGC GeoPackage** ovat avoimia ohjelmistoriippumattomia formaatteja/stadardeja, mutta ne eivät ole käytännössä levinneet yhtä laajaan käyttöön kuin muut yllä mainitut formaatit.

Linkkejä:
* Shape http://en.wikipedia.org/wiki/Shapefile
* TAB http://en.wikipedia.org/wiki/MapInfo_TAB_format
* KML http://en.wikipedia.org/wiki/Keyhole_Markup_Language
* GeoJSON http://en.wikipedia.org/wiki/GeoJSON
* GML http://en.wikipedia.org/wiki/Geography_Markup_Language
* OGC GeoPackage http://www.geopackage.org/


## Vektoriaineistot – Pistekohteet

Pistemäisten paikkatietokohteiden jakeluun voi käyttää yllä mainittuja formaatteja. Näiden lisäksi yksinkertainen ja suositeltava menetelmä on käyttää CSV-tiedostoja.

CSV on yksinkertainen tekstitiedosto, jossa ominaisuustietokentät ml. koordinaatit erotetaan toisistaan pilkuilla (tai muulla välimerkillä). Eri ohjelmien oletuksena käyttämä kenttien välinen erotin ja desimaalierotin saattaa vaihdella. Jos kenttien erottimena on yleisesti kansainvälisesti käytetty pilkku, tulee julkaisijan tarkistaa, että mahdolliset desimaaliluvut saadaan tunnistettua aineistosta. Tekstitiedoston merkistönä suositellaan käytettäväksi UTF-8 tai jos tästä poiketaan, niin siitä tulisi ilmoittaa tietotuoteselosteessa.


Linkkejä:
* CSV http://fi.wikipedia.org/wiki/CSV

## Rasteriaineistot

Rasteriaineistoilla tarkoitetaan mm. rasterikarttoja ja ortoilmakuvia. Rasteriaineiston avoimen datan julkaisussa suositellaan ensisijaisesti käytettäväksi **TIFF**- tai **PNG**-formaatteja. Mahdollisia formaatteja ovat myös esim. **JPEG**, **JPEG2000**.

Avoimen datan yhteydessä on tarkoituksenmukaista välttää ohjelmistokohtaisia formaatteja sekä mahdollisesti aineiston omistajan omissa käyttöaineistoissa olevia tiilitys- ja pyramidi-/overviewrakenteita, jotka on tuettu mm. TIFF-formaatissa ja kehittyneissä paikkatieto-ohjelmistoissa. Nämä aineistotyypit nopeuttavat aineiston päivittäistä käyttöä organisaation sisällä, mutta avoimen datan yhteydessä ne saattavat hidastaa tai jopa estää aineiston jatkokäytön avoimen datan käyttäjille.

**Rasteriaineistojen asemointi koordinaatistoon (georeferointi)  on käyttäjän kannalta välttämätön tieto, joka tulee aina olla mukana avoimen datan jakelussa.** Ensisijainen ja suositeltava tapa on käyttää World tiedostoja (tfw, pgw, jgw, j2w). Tekstimuotoisena tiedostona se on helposti luettavissa, yleiskäyttöinen ja useiden ohjelmistojen suoraan tukema.

TIFF-formaatti sallii myös tiedoston sisäiset menetelmät asemointitiedon tallentamiseen (GeoTIFF tai kiertomatriisi). Nämä toimivat hyvin organisaation sisäisessä vakioidussa käyttöympäristössä. Avoimen datan yhteydessä näiden käytettävyys voi kuitenkin jäädä vajaaksi, koska käyttäjällä pitäisi olla kehittyneet paikkatieto- tai apuohjelmat asemointitiedon hyödyntämiseen.

Rasterikuvaformaatit sallivat myös erilaiset kuvan pakkausalgoritmit. Rasterikuvia on useita eri tyyppejä:
* 24-bittinen (esim. värilliset ilmakuvat)
* 8-bittinen harmaasävykuva (harmaasävy ilmakuvat)
* 8-bittinen väri-indeksikuva (rasterikartta, jossa yksi värikoodi 0-255 edustaa yhtä RGB-väriarvoa)
* 1-bittinen (musta-valkoinen)

Ohjeen tässä versiossa ei käsitellä kuhunkin aineistotyyppiin suositeltavia formaatteja tai pakkausalgoritmeja. Yleisohjeena on, että pakkaamaton tiedosto avautuu varmimmin useimmissa ohjelmistoissa.

Linkkejä:
* World File http://en.wikipedia.org/wiki/World_file
* TIFF http://fi.wikipedia.org/wiki/TIFF
* PNG http://fi.wikipedia.org/wiki/PNG
* JPEG http://fi.wikipedia.org/wiki/JPEG
* JPEG 2000 http://fi.wikipedia.org/wiki/JPEG_2000


## Laserkeilausaineistot

Laserkeilausaineistoissa yleisesti käytettyjä formaatteja ovat **LAZ** ja *LAS**.

## Toimialakohtaiset standardit

Yleiskäyttöisten formaattien lisäksi on toimialakohtaisia standardeja (formaatteja), joita voi soveltaa myös avoimen datan jakelussa.

| Formaatti: | Käyttö:  | Linkkejä: |
| :--------- | :-------: | :--------- |
| **KuntaGML/KRYSP**	| Asemakaava; Kantakartta; Opastavat tiedot (Opaskartta, Osoitteet, Palvelut, Verkkotopologia); Rakennusvalvonta; Poikkeamispäätös ja suunnittelutarveratkaisu; Yleisen alueen käytön lupa; Ympäristö (Ilmoitukset, Vesihuoltolaki, Maa-ainesluvat, Ympäristöluvat) | http://www.paikkatietopalvelu.fi |
| **InfraModel3**		| Infra-rakentamisen tiedot | http://www.infrabim.fi/inframodel-3 |
| **CityGML**		| Kaupunkimallit | http://www.citygml.org |

## Formaattimuunnosvälineet

Kaupalliset valmisohjelmistot sekä avoimen lähdekoodin ohjelmistot sisältävät tyypillisesti työvälineitä formaattimuunnoksiin. Mikäli käytössö ei ole valmiita välineitä, on yksi mahdollisuus **GDAL/ORG**, mikä on avoimeen lähdekoodiin perustuva ohjelmistokirjasto formaattimuunnoksiin. Nämä muunnokset ovat ajettavissa myös komentoriviltä.

Linkkejä:
* GDAL http://www.gdal.org

## Avoimen paikkatiedon kohdeluokitus ja tietosisältö

Avoimen datan yhteydessä suositellaan käytettävän mahdollisimman selkokielistä kohdeluokituksen nimeämistä ja ominaisuustietojen käyttöä, jotka tulisi olla selostetuna tietotuotemäärittelyssä. Tietotuotteidenmäärittelyä on ohjeistettu JHS suosituksessa JHS 177 Paikkatietotuotteen määrittely.

Avoimen datan tietorakenne tulee olla optimoitu käyttäjälle ja se todennäköisesti eroaa tiedon tuottajan ylläpitojärjestelmän tietorakenteesta. Avoimen datan julkaisun valmistelussa aineistosta poistetaan organisaation sisäiseen käyttöön tarkoitetut tiedot esim. tiedon luojat, muokkaajat (nimitie-toja), luonti- ja muokkauspäivämäärät.

Tässä yhteydessä ei käsitellä lainsäädännöstä ja tie-tosuojasta johtuen vaadittavaa tietojen yleistämistä tms. vaadittua avoimen datan ennakkokäsittelyä. 

Linkkejä:
* JHS 177 Paikkatietotuotteen määrittely http://www.jhs-suositukset.fi/suomi/jhs177

## Lyhyesti:
1. Arvioi ja valitse aineiston ja oletetun käyttäjäryhmän mukainen formaatti.
2. Pyri julkaisemaan vähintään yhden formaatin mukainen aineistoversio tiedostona.
3. Käyttäjäpalautteen ja resurssien mukaan pyri laajentamaan aineistojen ja aineistoversioiden (formaatti, koordinaatisto) valikoimaa.
4. Suunnittele aineistojen myöhempi päivitys ja pyri julkaisemaan päivitykset vähintään kerran vuodessa tai kun aineisto on oleellisesti muuttunut
5. Julkaise aineistoja myös rajapintapalveluissa.

-----
[Palaa sisällysluetteloon](Sisällysluettelo.md)
