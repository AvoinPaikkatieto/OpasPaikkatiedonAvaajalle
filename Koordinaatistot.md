#Koordinaatistot ja korkeusjärjestelmät

## Koordinaatistot

Koordinaatistoja ja korkeusjärjestelmiä esitellään yksityiskohtaisemmin useissa eri internetlähteissä, joihin on linkkejä tämän kohdan lopussa. Yksityiskohtaisten kuvausten osalta lukijaa pyydetään tutustumaan näihin lähteisiin. Lyhyesti tiivistettynä avoimen datan yhteydessä voidaan käyttää seuraavia koordinaatistoja käyttötapauksesta riippuen:

**ETRS-TM35FIN (EPSG:3067)**

ETRS-TM35FIN on käytössä valtakunnallisissa kartastotöissä ja siten ensisijainen koordinaatisto valtakunnallisiin aineistoihin. 

**ETRS89 (EPSG:4258)**

ETRS89 on geodeettinen järjestelmä (aik. maantieteelliset koordinaatit) joissa koordinaatit esitetään leveys- ja pituusasteina (latitudi,longitudi). Näiden koordinaattien käyttö on yleistä kansainvälisissä kartta- ja navigointikäytössä, jolloin ei voida toimia kansallisissa koordinaatistoissa.

Kartta- ja navigointipalveluiden yhteydessä mainitaan usein käytettävän **WGS84**-koordinaatistoa. Eurooppalainen ETRS89 (EPSG:4258) on käytännössä yhtenevä amerikkalaistuaustaisen WGS84:n (EPSG:4326) kanssa eli koordiaatit ova käytännössä samat.

WGS84 koordinaatisto 

Paikkatietoformaateista on syytä huomioida mm. KML, GeoJSON ovat 

**ETRS-GKn-kaistat (EPSG:3873 - EPSG:3885)**

GK-kaistat paikallisissa aineistoissa 
n=19-31



WGS-84 ja ETRS-89 maantieteellinen ovat käytännössä yhteneviä

EPSG-koodit tunnisteina

KKJ, VVJ ja paikalliset ovat vanhentuneita => Vältetään

**Yleistä:**
* Eri koordinaatistot tunnistetaan kansainvälisellä **EPSG**-koodilla. ETRS-TM35FIN:n tunniste on EPSG:3067.
* Kaikki edellä mainitut koordinaatistot perustuvat samaan ETRS89-datumiin, joka käytännössä tarkoittaa, että em. koordinaatistojen välillä pystytään paikkatieto-ohjelmistoilla tekemään matemaattisesti tarkat koordinaatistomuunnokset. Muunnoksissa ei esiinnny vanhoille koordinaatistoille tyypillisiä.


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
