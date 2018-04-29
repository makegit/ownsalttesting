# Intro

Löysin tämänlaisen alustan jolla voidaan kirjotella sujuvasti markdown tekstejä. 

[terokarvinen](http://terokarvinen.com/2018/aikataulu-%E2%80%93-palvelinten-hallinta-ict4tn022-4-ti-5-ke-5-loppukevat-2018-5p#h5 "tero karvisen blog")
 Tehtävänä olisi seurvaavat jotka tein teron blogin sivulta.
 
 
h5
Poikkeuksellisesti pidempi palautusaika w18 perjantaina 2018-05-04 12:00 asti. Vappupäivänä ei ole opetusta. Hauskaa Wappua!

A) Valitse aihe omaksi kurssityöksi ja varaa se kommenttina aikataulusivun perään.

B) Julkaise raportti MarkDownilla. Jos käytät GitHub:ia, se tekee muotoilun automaattisesti “.md”-päätteisiin dokumentteihin.

C) Aja oma Salt-tila suoraa git-varastosta. Voit joko tehdä tilan alusta lähtien itse tai forkata sirottimen.


Kolmen tehtävän verran olisi tehtävää.

# A kohdalla keksiä projekti saltistack aiheena

Oma projektejana teen raspberry pi 3 saltstack asennus hallinta kuntoon. Lisäksi laitetaan siihen jonkin tyyppinen hyödyllinen käyttö.

Projektin jälkeen raspberry pi voisi hallita salt kautta internetin kautta mistäpäin tahansa. Tämä on erittäin tärkeää koska yleensä raspberry pi on sen tyyppisten verkkojen takana jolla jonkin tyyppisiä rajoitteita.

### raspberry pi normaali verkko haasteet

* Internettiin ei ole 24/7 pääsy
* yhteys internettiin on kaista rajoituksia
    * portit ei ole yleensä internettiin päin auki raspberry pi nähden.
    * internet yhteys auki vain satunnaisesti tai tiettyina aikoina.
    * palomuurien takana.
    * puhelin datayhteyksien takana tai vastaavan oman yhteys tyypin takana.

Eli verkkot joihinka raspberry pi yleensä käytössä ja integroidaan on sellaiset että raspberry pi ei ole selvää että mitä kaikkea pitäisi etukäteen huomioida että sitä pääsisi etäkäyttämään esim. ssh yli. Tähän salt on erinomainen mutta siinäkin siihen käytetään yleensä vähän epätyyppilisesti, jotenka se sopii erinomaisesti projektikseni.

Lisäksi tehdään vaikka sense-hat hyödyntäen sellainen syteemi että sillä voidaan kerätä sen sensoreista data ja kerrotaan sille uusi teksti mikä kirjotellaan led paneeliin. Lisäksi tehdään state saltin puolelle jolla raspberry pi asentuu ja konfiguroi joitakin ohjelmia siihen käytettäväksi. Tähän joudutaan soveltamaan tosin jotain erikoista syteemiä koska raspbberry pi ei ole täysin verorinen arkkitehtuuria debianista ja siihen omat repositorit.

Eli raspberry pi joitaan lopussa ylläpitoa, hallita ja hakia tietoa jota raspberry pi kerää ympäristöstään. Salt toimii täydellisesti tämäkin tyyppiseen toimintaa raspberry pi jätetään tehtävät joita sitten käy päästyään salt masteriin yhetyteen niin tekemässä sille määrätyt tehtävät.






### B kohdalla  tehdä tämä dokumentti markdown hyödyntäen

**Tässä tämä on! valmiina alustana**

haluisin opetella tekemään markdown kunnolla. Siis markdown dokumenteihin on tiettyjä tapoja tehdä dokumenttiin otsikoiti, alaotsikointi, lihavointia, kursoroitia, listoja, tauluja ja oikeastaa kaikki mitä tekstien kirjoittamiseen tarvitsee.

Yksin kertaisesti mitenkä tämä alusta tein oli kopion vain

[demo.showdownjs.com](http://demo.showdownjs.com/ "Alustaan linkki") sitten opettelin vaan käyttämään ja tässä sitä kirjoitellaan. Tosin sillä erotuksella että laitoin tämän läksy sivun sitten **oletus** tektiksi.

[showdownjs.com](http://showdownjs.com/ "showdownjs") Tämän javasript vaan muuntaa markdown tekstit suoraan html ja tulostaa ne tuohon viereen.

## kokeillaan vähän markdown käytössä

Nopeasti tällä voidaan tehdä tekstejä laittaa sitten sille kaikki sen vaativat muokkaukset ja lisäkset joita luoettelin aikasemmin. lisäksi tämän tekstin lopussa löytyy mitä kaikkea voidaan tehdä kun käytössä on markdown ja showdownjs.

```md
Laatikoiti jolla voidaan erotella se kohta mitä juuri tarvitaa.

tähän voidaan sitten kappaloida eri laisia asioita koodia tai mahdollisesti lainauksia tai muuta vastaavaa.
```

**lihavointikin onnituus!**

~~yliviivaus voidaan tehdä~~

:smile: jonkin tyyppiset hymiöt onnistuvat todennäköisesti kaikki ascii merkitöstä löytyvät hymiöt.

* pallolistaus
+ pallolistaus
- pallolistaus

1. numero listaus
2. numero listaus
3. numero listaus


 - [x] Tehtävä listaus tehdyksi
 - [ ] Tehtävä listaus tekemättömäksi
 
![markdwn](https://png.icons8.com/ios/1600/markdown.png "markdown")

