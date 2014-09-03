# Rajapinnat

Rajapinnoilla tarkoitetaan tässä erilaisa katselu- ja suorasaantirajapintoja paikkatietoaineistoihin. Tietotekniikassa käytetään usein nimitustä [ohjelmointirajapinta](http://fi.wikipedia.org/wiki/Ohjelmointirajapinta) (API, Application programming interface). Paikkatietotekniikassa on Inspire-direktiivin käyttöönottossa yleistyneet erilaiset rajapintapalvelut.

## Ensisijaiset rajapinnat
Paikkatietoaineistojen ensisijaiset rajapintateknologiat perustuvat [OGC](http://www.opengeospatial.org/):n (Open Geospatial Consortium) määrittelemiin rajapintoihin.

Rasterimuotoiset karttakuvapalvelut perustuvat seuraaviin rajapintoihin:
* [WMS](http://en.wikipedia.org/wiki/Web_Map_Service) (Web Map Service)
* [WMTS](http://en.wikipedia.org/wiki/Web_Map_Tile_Service) (Web Map Tile Service)
* [WCS](http://en.wikipedia.org/wiki/Web_Coverage_Service) (Web Coverage Service)

[JHS 180](http://www.jhs-suositukset.fi/suomi/jhs180):n [liitteessä 1](http://docs.jhs-suositukset.fi/jhs-suositukset/JHS180_liite1/JHS180_liite1.html) on tarkemmin suositeltu suomalaisten karttakuvapalvelujen toteuttamista.

Vektorimuotoisten aineistojen rajapintapalveluna toimii [WFS](http://en.wikipedia.org/wiki/Web_Feature_Service) (Web Feature Service). Tämän rajapinnan suomalaiset suositukset ovat [JHS 180](http://www.jhs-suositukset.fi/suomi/jhs180):n [liitteessä 2](http://docs.jhs-suositukset.fi/jhs-suositukset/JHS180_liite1/JHS180_liite2.html) (nimeltään kyselypalvelu). 

On huomattavaa, että WFS ei sovellu laajojen paikkatietoaineistojen toimittamiseen. Tällöin on tarpeellista toteuttaa [paikkatietojen tiedostopalvelu](http://docs.jhs-suositukset.fi/jhs-suositukset/JHS180_liite3/JHS180_liite3.html).




* Pakolliset rajapinnat
  * WMS, WFS
  * WCS (?)


* Muut "web" rajapinnat
  * REST
  * JSON / GeoJSON (vai ovatko tiedostoformaatteja?)

-----
[Palaa sisällysluetteloon](Sisällysluettelo.md)
