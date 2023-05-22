---
layout: "default"
description: ""
id: "kehittamisperiaatteet"
status: "Ehdotus"
---
# Kaavamääräyslajit kehittämisperiaatteeissa

## Yhdyskuntarakenteen laajenemissuunta

```Yhdyskuntarakenteen laajemissuunta```-kaavamääräyslaji saa ```numeerisen arvon```, joka kertoo laajenemisen suunnan asteina.  Kaavakohteen ```geometria```-attribuutin arvon tulee olla pistemäinen tai viivamainen.

## Kaupunki- tai kylakuvallisesti kehitettava alue

```Kaupunki- tai kylakuvallisesti kehitettava alue```-kaavamääräyslaji voi toimia itsenäisesti tai saada   ```vapaatekstikenttä arvon``` . Kaavakohteen ```geometria```-attribuutin arvon tulee olla pistemäinen tai aluemainen.

## Kehittämisvyöhyke

Maakuntakaavoissa usein käytetyt strategiset kehittämisperiaatteet voidaan kuvata ```Kehittämisvyöhyke```-kaavamääräyslajilla, joka saa ```vapaatekstikenttä arvon```. Sen arvona voi esiintyä mm. seuraavaa, myös muunlaiset arvot ovat sallittuja:

- Ekologinen kehittämisvyöhyke / kohdealue
- Energiahuollon / energiantuotannon kehittämisvyöhyke / kohdealue
- Kaupan ja/tai palveluiden kehittämisvyöhyke / kohdealue
- Kaupunkikehittämisen kehittämisvyöhyke / kohdealue
- Keskustatoimintojen kehittämisvyöhyke / kohdealue
- Liikenteen kehittämisvyöhyke / kohdealue
- Maaseudun kehittäminen
- Matkailun vetovoima-alue 
- Matkailun ja virkistyksen kehittämisvyöhyke / kohdealue
- Taajamatoimintojen kehittämisvyöhyke / kohdealue
- Teollisuuden ja logistiikan kehittämivyöhyke / kohdealue
- Uusiutuvan energian ja bioteollisuuden kehittämisalue / kohdealue
- Yhdyskuntateknisen huollon kehittämisalue / kohdealue

Kehittämisvyöhykettä kuvaavan kaavakohteen ```geometria```-attribuutin arvon tulee olla aluemainen tai pistemäinen. 

# Lisätiedonlajit kehittämisperiaatteissa

## Yhteystarve

```Yhteystarve``` voi olla jonkin Kaavamääräys-koodin lisätiedonlajina, jolloin voidaan muodostaa yhteystarpeita. Kaavakohteen ```geometria```-attribuutin arvon tulee olla viivamainen.

Esimerkkejä: 

Kaavamääräyryhmän otsikko **Joukkoliikenteen kehittämistarve**, sisältää Kaavamääräyslajin ```Joukkoliikenteen alue```ja sen Lisätiedonlajin ```Yhteystarve```.

Kaavamääräyryhmän otsikko **Johdon, putken tai linjan yhteystarve** voidaan muodostaa liittämällä kaavakohteeseen määräys ```Johto, putki tai linja```ja sen Lisätiedonlajin ```Yhteystarve```.

Kaavamääräyryhmän otsikko **Viheryhteystarve** voidaan muodostaa liittämällä kaavakohteeseen määräys ```Viheralue```sekä lisätieto ```Yhteystarve```.

Kaavamääräyryhmän otsikko **Virkistysyhteystarve** voidaan muodostaa liittämällä kaavakohteeseen määräys ```Ulkoilu- tai virkistysreitti```sekä lisätieto ```Yhteystarve```.

Erityyppiset **Tieliikenteen yhteystarpeet** saadaan kuvattua väylän toiminnallista luokkaa parhaiten kuvaavan määräyskoodin kuten```Valtatie``` ja listätieto ```Yhteystarve```.

## Eheytettävä tai tiivistettävä

```Eheytettävä tai tiivistettävä``` voi olla jonkin Kaavamääräys-koodin lisätiedonlajina, jolloin voidaan muodostaa eheytettävän tai tiivistettävän alueen. Kaavakohteen ```geometria```-attribuutin arvon tulee olla aluemainen tai pistemäinen.

