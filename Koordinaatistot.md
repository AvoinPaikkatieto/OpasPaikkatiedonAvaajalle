#Koordinaatistot ja korkeusjärjestelmät

## Koordinaatistot

Koordinaatistoja ja korkeusjärjestelmiä esitellään yksityiskohtaisesti useissa eri internetlähteissä, joihin on linkkejä tämän kohdan lopussa. Yksityiskohtaisten kuvausten osalta lukijaa pyydetään tutustumaan näihin lähteisiin.

Lyhyesti tiivistettynä avoimen datan yhteydessä voidaan käyttää seuraavia koordinaatistoja käyttötapauksesta riippuen:

**ETRS-TM35FIN (EPSG:3067)**

ETRS-TM35FIN on käytössä valtakunnallisissa kartastotöissä ja on siten ensisijainen koordinaatisto valtakunnallisiin aineistoihin. 

**ETRS89 (EPSG:4258)**

ETRS89 on geodeettinen järjestelmä (aikaisemmin kutsuttu myös nimellä maantieteelliset koordinaatit), joissa koordinaatit esitetään leveys- ja pituusasteina (latitudi,longitudi). Näiden koordinaattien käyttö on yleistä kansainvälisessä kartta- ja navigointikäytössä, jolloin ei voida toimia kansallisissa karttaprojektioissa (koordinaatistoissa) vaan toimitaan koordinaateilla vertausellipsoidin pinnalla.

Kartta- ja navigointipalveluiden yhteydessä mainitaan usein käytettävän **WGS84**-koordinaatistoa. Eurooppalainen ETRS89 (EPSG:4258) on käytännössä yhtenevä amerikkalaistuaustaisen WGS84:n (EPSG:4326) kanssa eli koordinaatit ova käytännössä samat paikkatietojen yhteiskäytön vaatimalla tarkkuudella.

Paikkatietoformaateista KML on aina WGS84-koordinaatistossa ja GeoJSON oletuksena WGS84:ssä ellei muuta mainita.

Geodeettisen järjestelmän koordinaattien erityipiirteinä on, että sama koordinaattipari voidaan esittää eri muodossa eri yksiköillä. **Asteen desimaalit ovat suositeltava esitysmuoto avoimelle datalle** ja ne ovat käytössä esim karttapalveluissa sijainnin osoittavissa URL:eissa. Minuutit ja sekunnit esitysmuoto on käytössä mm. GPS paikannuksessa.

| Esitysmuoto: | Latitudi: | Longitudi: |
| ---          | :-------: | :--------: |
| **Asteen desimaalit** | 61.50493836 | 23.74319821 |
| Minuutin desimaalit | 61° 30.296' | 23° 44.592' |
| Sekunnin desimaalit | 61°30' 17.778'' | 23° 44' 35.514'' |


**ETRS-GKn (EPSG:3873 - EPSG:3885)**

ETRS-GKn koordinaatistot ovat käytössä Suomemassa kunta ja seutukuntatasolla. Lisäksi mittaustarkkuutta vaativivat kartoitustehtävät tehdään ETRS-GKn koordinaatistossa. ETRS-GKn-kaistoja on Suomen yli yhden asteen välein siten, että n=19-31 aluetta sivuavan keskimeridiaanin (pituuspiiri) mukaosesto. Esimerkiksi Tampereella on käytössä ETRS-GK24 (EPSG:3878).

**Muut koordinaatistot**

Aikaisemmin yleisesti käytetyt KKJ-, VVJ- ja paikalliset koordinaatistot ovat avoimen datan kannalta käytännössä vanhentuneita, joten niiden käyttöä tulisi välttää avoimessa datassa.

**Yleistä:**
* Eri koordinaatistot tunnistetaan kansainvälisellä **EPSG**-koodilla. ETRS-TM35FIN:n tunniste on EPSG:3067.
* Kaikki edellä mainitut koordinaatistot perustuvat samaan ETRS89-datumiin, joka käytännössä tarkoittaa, että em. koordinaatistojen välillä pystytään paikkatieto-ohjelmistoilla tekemään matemaattisesti tarkat koordinaatistomuunnokset. Muunnoksissa ei esiinny vanhojen koordinaatistojen epätarkkuuuksista johtuvia muunnosvirheitä.
* Rasteriaineistojen osalta on syytä huomioida:
  * Rasteriaineistojen jälkikäteen tehty koordinaatistomuunnos tuottaa usein ulkoasultaan heikentyneen lopputuloksen. Rasterijulkaisu pitäisi siten pyrkiä tekemään siten suoraan lopullisen käyttkoordinaatistoon.
  * Rasteriaineistot soveltuvat parhaiten julkaistaviksi tasokoordinaatistoon ja projektioon, jossa mittayksiköinä on metriä/pikseli. Geodeettinen järjestelmä (maantieteellinen koordinaatisto), jossa mittayksikkö olisi astetta/pikseli, mitä käytännössä ei käytetä.


## Korkeusjärjestelmät
Kartta- ja paikkatietoaineiston korkeusjärjestelmänä tulisi käyttää **N2000**-korkeusjärjestelmää, joka on valtakunnallinen suositus. Aikaisempien N60, N43, NN sekä paikallisten korkeusjärjes-telmien käyttöä tulee välttää vanhentuneina.

Linkkejä:
* JHS 180 Paikkatiedon sisältöpalvelut, liite 1, kohta 2 http://docs.jhs-suositukset.fi/jhs-suositukset/JHS180_liite1/JHS180_liite1.pdf
* Koordinaatti- ja korkeusjärjestelmät, Maanmittauslaitos http://www.maanmittauslaitos.fi/kartat/koordinaatit/koordinaatti-korkeusjarjestelmat
* JHS 153 ETRS89-järjestelmän mukaiset koordinaatit Suomessa http://www.jhs-suositukset.fi/suomi/jhs153
* JHS 154 ETRS89 -järjestelmään liittyvät karttaprojektiot, tasokoordinaatistot ja karttalehtijako http://www.jhs-suositukset.fi/suomi/jhs154
* JHS 163 Suomen korkeusjärjestelmä N2000 http://www.jhs-suositukset.fi/suomi/jhs163
* EPSG http://www.epsg-registry.org ja http://www.epsg.org/


-----
[Palaa sisällysluetteloon](Sisällysluettelo.md)
