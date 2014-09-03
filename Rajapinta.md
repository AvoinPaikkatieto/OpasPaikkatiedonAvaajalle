# Rajapinnat

Rajapinnoilla tarkoitetaan tässä erilaisia katselu- ja latausrajapintoja paikkatietoaineistoihin. Tietotekniikassa käytetään usein nimitustä [ohjelmointirajapinta](http://fi.wikipedia.org/wiki/Ohjelmointirajapinta) (API, Application programming interface). Paikkatietotekniikassa on Inspire-direktiivin käyttöönoton myötä yleistyneet erilaiset rajapintapalvelut.

## Ensisijaiset rajapinnat
Paikkatietoaineistojen ensisijaiset rajapintateknologiat perustuvat [OGC](http://www.opengeospatial.org/):n (Open Geospatial Consortium) määrittelemiin rajapintoihin.

Rasterimuotoiset karttakuvapalvelut perustuvat seuraaviin rajapintoihin:
* [WMS](http://en.wikipedia.org/wiki/Web_Map_Service) (Web Map Service)
* [WMTS](http://en.wikipedia.org/wiki/Web_Map_Tile_Service) (Web Map Tile Service)

[JHS 180](http://www.jhs-suositukset.fi/suomi/jhs180):n [liitteessä 1](http://docs.jhs-suositukset.fi/jhs-suositukset/JHS180_liite1/JHS180_liite1.html) on tarkemmin suositeltu suomalaisten karttakuvapalvelujen toteuttamista.

Hilamuotoisen paikkatiedon jakeluun käytetään [WCS](http://en.wikipedia.org/wiki/Web_Coverage_Service) (Web Coverage Service) -rajapintaa. Hilamuotoisia paikkatietoja ovat esimerkiksi rasterimuotoinen korkeusmalli ja satelliittikuvat.

Vektorimuotoisten aineistojen rajapintapalveluna toimii [WFS](http://en.wikipedia.org/wiki/Web_Feature_Service) (Web Feature Service). Tämän rajapinnan suomalaiset suositukset ovat [JHS 180](http://www.jhs-suositukset.fi/suomi/jhs180):n [liitteessä 2](http://docs.jhs-suositukset.fi/jhs-suositukset/JHS180_liite1/JHS180_liite2.html) (nimeltään kyselypalvelu). 

On huomattavaa, että WFS ei sovellu laajojen paikkatietoaineistojen toimittamiseen. Tällöin on tarpeellista toteuttaa [paikkatietojen tiedostopalvelu](http://docs.jhs-suositukset.fi/jhs-suositukset/JHS180_liite3/JHS180_liite3.html) (JHS180, Liite 3).

## Toissijaiset rajapinnat
Paikkatiedon tuottajat voivat erityistarpeita varten tuottaa myös muita rajapintapalveluita. Esimerkiksi REST/JSON/GeoJSON -teknologiat soveltuvat hyvin paikkatietoaineistojen suorakäyttöön. On kuitenkin huomattava, että tässä dokumentissa mainitut ensisijaiset rajapinnat ovat lakisääteisiä tehtäviä, toissijaiset rajapinnat (vain) parempaa palvelua.

-----
[Palaa sisällysluetteloon](Sisällysluettelo.md)
