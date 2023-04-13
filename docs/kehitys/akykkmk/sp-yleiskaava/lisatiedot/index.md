---
layout: "default"
description: ""
id: "lisatiedot"
status: "Ehdotus"
---

# Kaavamääräyksen lisätiedot
{:.no_toc}

## Tyyppi
Kaavamääräyksen tarkempi tyypittely. Ryhmittelyotsikko, vain [Alakoodeja](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar) käytetään.

### Pääkäyttötarkoitus
Kaavamääräyksen lisätiedolla [Pääkäyttötarkoitus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/paakayttotarkoitus) annotoidaan [Aluevarauksille](../aluevaraukset/index.md) annettuista [Kaavamääräyksistä](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavamaarays/) pääkäyttötarkoitus. Pääkäyttötarkoituksella tarkoitetaan sitä käyttötarkoitusta, johon suhteellisesti suurin osa alueen käytöstä on tarkoitettu. 

{% include common/clause_start.html type="req" id="sp-yk/paakayttotarkoitus" %}
[Aluevarausten](../aluevaraukset/index.md) [Kaavamääräyksistä](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavamaarays/) yhdelle tai useammalle on merkittävä [Lisätiedoksi](https://tietomallit.suomi.fi/model/rytj-kaava/Lisatieto/) [Pääkäyttötarkoitus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/paakayttotarkoitus), riippuen siitä, onko [Kaavakohteelle](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/) osoitettu osuudeltaan yhtäsuureksi tarkoitettuja käyttötarkoituksia.
{% include common/clause_end.html %}

### Poisluettava käyttötarkoitus
Kaavamääräyksen ```lisatieto```-attribuutin arvoina saa esiintyä nolla tai useampi [Lisätieto](https://tietomallit.suomi.fi/model/rytj-kaava/Lisatieto/) jonka laji on [Poisluettava käyttötarkoitus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/poisluettavaKayttotarkoitus), ja jonka ```arvo```-attribuutin arvoina on yksi tai useampi [Koodiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Koodiarvo/) jotka viittaavat [Kaavamääräyslaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji)-koodiston koodeihin, jotka sisältyvät ```Käyttötarkoitus```-määrityshierarkiaan. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

Poisluettavat käyttötarkoituslajit tulee valita siten, että ne kohdistuvat ```arvo```-attribuuttien avulla valittuun yleispiirteisempään joukkoon käyttötarkoituksia pois lukien niistä osan.

Esimerkkejä: 
* [Toimitilojen alue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/toimitilojenAlue) pois lukien [Tuotantorakennusten alue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/tuotantorakennustenAlue).

### Vaihtoehtoinen
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/vaihtoehtoinen>

Esimerkkejä
* ```Vaihtoehtoinen tielinjaus``` voidaan kuvata tien toiminnallista luokkaa kuvaavan kaavamääräyksen, esim. [Valtatie](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/valtatie) ja lisätiedon [vaihtoehtoinen](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/vaihtoehtoinen>) yhdistelmällä.

{% include common/tip.html content="```Ohjeelliset tielinjaukset``` ja vastaavat ohjeelliset kaavamääräykset muodostetaan Kaavakohteen ```sijainninSitovuus``` -attribuutin arvon ```Ohjeellinen``` avulla." %}

{% include common/clause_start.html type="rec" id="sp-yk/suos-vaihtoehtoinen-liittyva-kohde" %}
[Kaavakohteen](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/), johon liittyy lisätieto vaihtoehtoinen, assosiaation [Liittyvä kohde](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/6e080c6a-bb00-4d7f-b095-215f7c902e19) tulee viitata näiden vaihtoehtoista maankäyttöä kuvaaviin Kaavakohteisiin. Assosiaation ```rooli```-attribuutin arvon tulee ilmaista, että liittyvä kohde on vaihtoehtoinen."s
{% include common/clause_end.html %}

## Merkittävyys
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/merkittavyys>

Ryhmittelyotsikko, vain [Alakoodeja](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar) käytetään.

Merkittävyys-lisätiedon alakoodien avulla voidaan täsmentää kaavamääräyksen kuvaaman maankäytön tai sen perusteena olevien arvojen merkittävyyttä, maantieteellisin laajuuksin kuvattuna.

Esimerkkejä:<br>
* ``` Maakunnallisesti arvokas maisema-alue``` voidaan muodostaa liittämällä kaavakohteeseen määräys [Maisemallisesti arvokas alue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/maisemallisestiArvokasAlue) sekä lisätieto [Maakunnallinen](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/maakunnallinen).

* ```Alueverkon pyöräilyreitti``` voidaan muodostaa liittämällä kaavakohteeseen määräys [Pyöräilyreitti](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/pyorailyReitti) sekä lisätieto [Alueellinen](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/alueellinen). Vastaavasti ```Seutuverkon pyöräilyreitti``` voidaan muodostaa vaihtamalla lisätieto koodiin [Seudullinen](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/seudullinen).

## Tarve
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/tarve>

Yleiskaavoissa käytetään paljon jotakin tunnistettua tarvetta kuvaavia kaavamääräyksiä. Tällaiset muodostetaan [Kaavamääräyslaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji)-koodien ja [Tarve](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/tarve)-luokan lisätietokoodien yhdistelminä.

Esimerkkejä:<br>
* ```Johdon, putken tai linjan yhteystarve``` voidaan muodostaa liittämällä kaavakohteeseen määräys [Johto, putki tai linja](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/JohtoPutkiTaiLinja) sekä lisätieto [Yhteystarve](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/yhteystarve). 

* ```Viheryhteystarve``` voidaan muodostaa liittämällä kaavakohteeseen määräys [Ekologinen yhteys](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/ekologinenYhteys) sekä lisätieto [Yhteystarve](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/yhteystarve). Samoin esim. ```virkistysyhteystarve``` voidaan kuvata koodien [Ulkoilu- tai virkistysreitti](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/ulkoiluTaiVirkistysReitti) ja [Yhteystarve](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/yhteystarve) yhdistelmänä.

* Erityyppiset ```tieliikenteen yhteystarpeet``` saadaan kuvattua väylän toiminnallista luokkaa parhaiten kuvaavan määräyskoodin (esim. [Valtatie](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/valtatie)) ja lisätiedon [Yhteystarve](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/yhteystarve) yhdistelmänä.

## Ympäristömuutoksen laji
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/ymparistomuutoksenLaji>

Ryhmittelyotsikko, vain [Alakoodeja](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar) käytetään.

Ympäristömuutoksen laji -ryhmän lisätietokoodein voidaan täsmentää, miten kaavamääräyksen kuvaama maankäyttö eroaa suhteessa kaavan laadinnan ajanhetkellä olemassa olevaan, kaavakohteen alueella sijaitsevaan maankäyttöön.

Esimerkkejä:

* Määräys [Valtatie](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/valtatie) + lisätieto [Uusi](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/uusi>) = ```Uusi valtatie```.

* Määräys [Asuinpientaloalue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/asuinpientaloalue) + lisätieto [Pienin toimenpitein kehitettävä](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/pieninToimenpiteinKehitettava>) = ```Pienin toimenpitein kehitettävä asuinpientaloalue```.

## Maankäyttörajoitus

### Rakentamisrajoitus (yleiskaava)
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/rakentamisrajoitusYleiskaava>

{% include common/clause_start.html type="req" id="sp-yk/vaat-rakentamisrajoitus-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä nolla tai useampi [Tekstiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Tekstiarvo/) (yksi kullakin kielellä), joka täydentää kaavamääräystietoa.  Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

### Määräaikainen rakentamisrajoitus
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/maaraaikainenRakentamisrajoitus>

{% include common/clause_start.html type="req" id="sp-yk/vaat-maara-aikainen-rakentamisrajoitus-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä joko
* yksi [Numeerinen arvo](https://tietomallit.suomi.fi/model/rytj-kaava/NumeerinenArvo/) joka kuvaa sen kaavan hyväksymisestä alkavan ajanjakson pituuden, jona aikana käyttö on kielletty. Numeerisen arvon  on toteutettava [Integer](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/dokumentaatio/#integer)-rajapinta. Yksikkönä vuosi (```v```), tai kuukausi (```kk```) tai
* yksi [Ajanhetkiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Ajanhetkiarvo/) joka kuvaa päivämäärän, johon saakka käyttö on kielletty.
Muun tyyppiset arvot eivät ole sallittuja.

Lisäksi ```arvo```-attribuutin arvoina saa esiintyä yksi tai useampi [Tekstiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Tekstiarvo/) (yksi kullakin kielellä), joka täydentää kaavamääräystietoa.

Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

### Toimenpiderajoitus
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/toimenpiderajoitus>

{% include common/clause_start.html type="req" id="sp-yk/vaat-toimenpiderajoitus-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä nolla tai useampi [Tekstiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Tekstiarvo/) (yksi kullakin kielellä), joka täydentää kaavamääräystietoa.  Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

### Rakennuksen purkamiskielto
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/rakennuksenPurkamiskielto>

{% include common/clause_start.html type="req" id="sp-yk/vaat-purkamisrajoitus-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä nolla tai useampi [Tekstiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Tekstiarvo/) (yksi kullakin kielellä), joka täydentää kaavamääräystietoa. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Rakentamisen ohjaus
### Rakennusluvan peruste
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/rakennusluvanPeruste>

Rakennuslupa rakennuksen rakentamiseen voidaan MRL:n [137 §:n](https://www.finlex.fi/fi/laki/ajantasa/1999/19990132#L19P137) 1 momentissa säädetyn estämättä myöntää, jos oikeusvaikutteisessa yleiskaavassa on erityisesti määrätty kaavan tai sen osan käyttämisestä rakennusluvan myöntämisen perusteena. Määräys ei voi koskea aluetta, jolla maankäytön ohjaustarve edellyttää asemakaavan laatimista. Edellytyksenä on lisäksi, että yleiskaava ohjaa riittävästi rakentamista ja muuta maankäyttöä kyseisellä alueella.

{% include common/clause_start.html type="req" id="sp-yk/vaat-yk-kaytto-rakennusluvan-perusteena-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä nolla tai useampi [Tekstiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Tekstiarvo/) (yksi kullakin kielellä), joka täydentää kaavamääräystietoa. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

### Käyttötarkoituksen osuus kerrosalasta
{% include common/clause_start.html type="req" id="sp-yk/vaat-osuus-kerrosalasta" %}
Aluevarauksen käyttötarkoitusta kuvaavaan kaavamääräykseen liitetty ```lisatieto```-attribuutti, jonka laji on [Käyttötarkoituksen osuus kerrosalasta](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/kayttotarkoituksenOsuusKerrosalasta), voi saada täsmälleen yhden arvon:
* Yksi [Numeerinen arvo](https://tietomallit.suomi.fi/model/rytj-kaava/NumeerinenArvo/) tai yksi [Numeerinen arvoväli](https://tietomallit.suomi.fi/model/rytj-kaava/NumeerinenArvovali/) jotka kertovat sallitun, käyttötarkoitukseen kohdistettavan kerroalan määrän koko sallitusta kerrosalasta joko kerrosneliömetreinä (```k-m2```) tai prosentteina (```%```). Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava [Integer](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/dokumentaatio/#real)-rajapinta.
{% include common/clause_end.html %}

Mikäli sallittua rakentamisen määrää ei ole jaoteltu käyttötarkoituksittain, ei lisätietoja käytetä.

<!--
## Kulttuuriymparistöarvojen alue
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/kulttuuriymparistoarvojenAlue>

{% include common/clause_start.html type="req" id="sp-ak/vaat-kulttuuriymparistoarvojen-alue" %}
* ```arvo```-attribuutin arvona saa esiintyä nolla tai useampi [Tekstiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Tekstiarvo/) (yksi kullakin kielellä), joka täydentää kaavamääräystietoa. Muun tyyppiset arvot eivät ole sallittuja.
* ```lisatieto```-attribuutin arvoina saa esiintyä nolla tai useampi [Lisätieto](https://tietomallit.suomi.fi/model/rytj-kaava/Lisatieto/) joka ```laji``` on yksi seuraavista:   
   * [Kulttuurihistoriallinen merkittävyys](http://uri.suomi.fi/codelist/rytj/RY_LisatiedonLaji_AK/code/05), jonka arvoina on yksi tai useampi [Koodiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Koodiarvo/) jotka viittaavat johonkin [Kulttuurihistoriallinen merkittävyys](http://uri.suomi.fi/codelist/rakrek/kulthistmer) koodiston koodeista,
   * [Kulttuurihistoriallinen arvotyyppi](http://uri.suomi.fi/codelist/rytj/RY_LisatiedonLaji_AK/code/06), jonka arvoina on yksi tai useampi [Koodiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Koodiarvo/) jotka viittaavat johonkin [Kulttuurihistoriallinen arvotyyppi](http://uri.suomi.fi/codelist/rakrek/Kulthistatyyp) koodiston koodeista,
   * [Kulttuurihistoriallinen tyyppi](http://uri.suomi.fi/codelist/rytj/RY_LisatiedonLaji_AK/code/07), jonka arvoina on yksi tai useampi [Koodiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Koodiarvo/) jotka viittaavat johonkin [Kulttuurihistoriallinen tyyppi](http://uri.suomi.fi/codelist/rakrek/kulthistyyp) koodiston koodeista, tai
   * [Kulttuurihistoriallisen merkittävyyden kriteerit](http://uri.suomi.fi/codelist/rytj/RY_LisatiedonLaji_AK/code/08), jonka arvoina on yksi tai useampi[Koodiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Koodiarvo/) joka viittaa johonkin [Kulttuurihistoriallisen merkittävyyden kriteerit](http://uri.suomi.fi/codelist/rakrek/KultKritee) koodiston koodeista.
Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}
-->