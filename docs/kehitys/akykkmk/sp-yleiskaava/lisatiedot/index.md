---
layout: "default"
description: ""
id: "lisatiedot"
status: "Ehdotus"
---

# Kaavamääräyksen lisätiedot
{:.no_toc}

## Tyyppi
Kaavamääräyksen tarkempi tyypittely. Ryhmittelyotsikko, vain {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar" title="alakoodeja" %} käytetään.

### Pääkäyttötarkoitus
Kaavamääräyksen lisätiedolla [Pääkäyttötarkoitus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/paakayttotarkoitus) annotoidaan [Aluevarauksille](../aluevaraukset/index.md) annettuista {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#kaavamaarays" title="Kaavamääräyksistä" %} pääkäyttötarkoitus. Pääkäyttötarkoituksella tarkoitetaan sitä käyttötarkoitusta, johon suhteellisesti suurin osa alueen käytöstä on tarkoitettu. 

{% include common/clause_start.html type="req" id="sp-yk/paakayttotarkoitus" %}
[Aluevarausten](../aluevaraukset/index.md) {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#kaavamaarays" title="Kaavamääräyksistä" %} yhdelle tai useammalle on merkittävä {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#lisatieto" title="Lisatiedoksi" %} [Pääkäyttötarkoitus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/paakayttotarkoitus), riippuen siitä, onko {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#kaavakohde" title="Kaavakohteelle" %} osoitettu osuudeltaan yhtäsuureksi tarkoitettuja käyttötarkoituksia.
{% include common/clause_end.html %}

### Poisluettava käyttötarkoitus
Kaavamääräyksen ```lisatieto```-attribuutin arvoina saa esiintyä nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#lisatieto" title="Lisatieto" %} jonka laji on [Poisluettava käyttötarkoitus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/poisluettavaKayttotarkoitus), ja jonka ```arvo```-attribuutin arvoina on yksi tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#koodiarvo" title="KoodiArvo" %} jotka viittaavat [Kaavamääräyslaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays)-koodiston koodeihin, jotka sisältyvät ```Käyttötarkoitus```-määrityshierarkiaan. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

Poisluettavat käyttötarkoituslajit tulee valita siten, että ne kohdistuvat ```arvo```-attribuuttien avulla valittuun yleispiirteisempään joukkoon käyttötarkoituksia pois lukien niistä osan.

Esimerkkejä: 
* [Toimitilojen alue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/toimitilojenAlue) pois lukien [Tuotantorakennusten alue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/tuotantorakennustenAlue).

### Reservialue
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/reserviAlue>

{% include common/clause_start.html type="req" id="sp-yk/vaat-reservialue" %}
Alustavaa tai ehdollista maankäyttöä kuvaavaa [Reservialue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/reserviAlue)-lisätietoa käytetään kaavamääräyksille, joilla kuvataan alueen käyttötarkoitusta, eli ns. [Aluevarauksille](../aluevaraukset/index.md).
{% include common/clause_end.html %}

{% include common/tip.html content="Reservialue-koodin avulla voidaan ohjata myös kaavan esitystapaa (ns. r-päätteisten aluevarausten nimiöiden kuvaamiseen)." %}

### Vaihtoehtoinen
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/vaihtoehtoinen>

Esimerkkejä
* ```Vaihtoehtoinen tielinjaus``` voidaan kuvata tien toiminnallista luokkaa kuvaavan kaavamääräyksen, esim. [Valtatie](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/valtatie) ja lisätiedon [vaihtoehtoinen](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/vaihtoehtoinen>) yhdistelmällä.

{% include common/tip.html content="```Ohjeelliset tielinjaukset``` ja vastaavat ohjeelliset kaavamääräykset muodostetaan Kaavakohteen ```sijainninSitovuus``` -attribuutin arvon ```Ohjeellinen``` avulla." %}

{% include common/clause_start.html type="rec" id="sp-yk/suos-vaihtoehtoinen-liittyva-kohde" %}
{% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#kaavakohde" title="Kaavakohteen" %}, johon liittyy lisätieto vaihtoehtoinen, assosiaation ```liittyvaKohde``` tulee viitata näiden vaihtoehtoista maankäyttöä kuvaaviin Kaavakohteisiin. Assosiaation ```rooli```-attribuutin arvon tulee ilmaista, että liittyvä kohde on vaihtoehtoinen." %}
{% include common/clause_end.html %}

## Merkittävyys
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/merkittavyys>

Ryhmittelyotsikko, vain {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar" title="alakoodeja" %} käytetään.

Merkittävyys-lisätiedon alakoodien avulla voidaan täsmentää kaavamääräyksen kuvaaman maankäytön tai sen perusteena olevien arvojen merkittävyyttä, maantieteellisin laajuuksin kuvattuna.

Esimerkkejä:<br>
* ``` Maakunnallisesti arvokas maisema-alue``` voidaan muodostaa liittämällä kaavakohteeseen määräys [Maisemallisesti arvokas alue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/maisemallisestiArvokasAlue) sekä lisätieto [Maakunnallinen](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/maakunnallinen).

* ```Alueverkon pyöräilyreitti``` voidaan muodostaa liittämällä kaavakohteeseen määräys [Pyöräilyreitti](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/pyorailyReitti) sekä lisätieto [Alueellinen](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/alueellinen). Vastaavasti ```Seutuverkon pyöräilyreitti``` voidaan muodostaa vaihtamalla lisätieto koodiin [Seudullinen](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/seudullinen).

## Tarve
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/tarve>

Yleiskaavoissa käytetään paljon jotakin tunnistettua tarvetta kuvaavia kaavamääräyksiä. Tällaiset muodostetaan [Kaavamääräyslaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays)-koodien ja [Tarve](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/tarve)-luokan lisätietokoodien yhdistelminä.

Esimerkkejä:<br>
* ```Johdon, putken tai linjan yhteystarve``` voidaan muodostaa liittämällä kaavakohteeseen määräys [Johto, putki tai linja](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/JohtoPutkiTaiLinja) sekä lisätieto [Yhteystarve](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/yhteystarve). 

* ```Viheryhteystarve``` voidaan muodostaa liittämällä kaavakohteeseen määräys [Ekologinen yhteys](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/ekologinenYhteys) sekä lisätieto [Yhteystarve](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/yhteystarve). Samoin esim. ```virkistysyhteystarve``` voidaan kuvata koodien [Ulkoilu- tai virkistysreitti](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/ulkoiluTaiVirkistysReitti) ja [Yhteystarve](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/yhteystarve) yhdistelmänä.

* Erityyppiset ```tieliikenteen yhteystarpeet``` saadaan kuvattua väylän toiminnallista luokkaa parhaiten kuvaavan määräyskoodin (esim. [Valtatie](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/valtaTie)) ja lisätiedon [Yhteystarve](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/yhteystarve) yhdistelmänä.

## Ympäristömuutoksen laji
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/ymparistomuutoksenLaji>

Ryhmittelyotsikko, vain {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar" title="alakoodeja" %} käytetään.

Ympäristömuutoksen laji -ryhmän lisätietokoodein voidaan täsmentää, miten kaavamääräyksen kuvaama maankäyttö eroaa suhteessa kaavan laadinnan ajanhetkellä olemassa olevaan, kaavakohteen alueella sijaitsevaan maankäyttöön.

Esimerkkejä:

* Määräys [Valtatie](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/valtaTie) + lisätieto [Uusi](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/uusi>) = ```Uusi valtatie```.

* Määräys [Asuinpientaloalue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/asuinpientaloAlue) + lisätieto [Pienin toimenpitein kehitettävä](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/pieninToimenpiteinKehitettava>) = ```Pienin toimenpitein kehitettävä asuinpientaloalue```.

## Maankäyttörajoitus

### Rakentamisrajoitus
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/rakentamisrajoitus>

{% include common/clause_start.html type="req" id="sp-yk/vaat-rakentamisrajoitus-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#tekstiarvo" title="TekstiArvo" %} (yksi kullakin kielellä), joka täydentää kaavamääräystietoa.  Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

### Määräaikainen rakentamisrajoitus
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/maaraaikainenRakentamisrajoitus>

{% include common/clause_start.html type="req" id="sp-yk/vaat-maara-aikainen-rakentamisrajoitus-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä joko
* yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} joka kuvaa sen kaavan hyväksymisestä alkavan ajanjakson pituuden, jona aikana käyttö on kielletty. Numeerisen arvon  on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#integer" title="Integer" %}-rajapinta. Yksikkönä vuosi (```v```), tai kuukausi (```kk```) tai
* yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#ajanhetkiarvo" title="Ajanhetkiarvo" %} joka kuvaa päivämäärän, johon saakka käyttö on kielletty.
Muun tyyppiset arvot eivät ole sallittuja.

Lisäksi ```arvo```-attribuutin arvoina saa esiintyä yksi tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#tekstiarvo" title="TekstiArvo" %} (yksi kullakin kielellä), joka täydentää kaavamääräystietoa.

Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

### Toimenpiderajoitus
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/toimenpiderajoitus>

{% include common/clause_start.html type="req" id="sp-yk/vaat-toimenpiderajoitus-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#tekstiarvo" title="TekstiArvo" %} (yksi kullakin kielellä), joka täydentää kaavamääräystietoa.  Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

### Rakennuksen purkamisrajoitus
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/rakennuksenPurkamisrajoitus>

{% include common/clause_start.html type="req" id="sp-yk/vaat-purkamisrajoitus-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#tekstiarvo" title="TekstiArvo" %} (yksi kullakin kielellä), joka täydentää kaavamääräystietoa. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Rakentamisen ohjaus
### Rakennusluvan peruste
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/rakennusluvanPeruste>

Rakennuslupa rakennuksen rakentamiseen voidaan MRL:n [137 §:n](https://www.finlex.fi/fi/laki/ajantasa/1999/19990132#L19P137) 1 momentissa säädetyn estämättä myöntää, jos oikeusvaikutteisessa yleiskaavassa on erityisesti määrätty kaavan tai sen osan käyttämisestä rakennusluvan myöntämisen perusteena. Määräys ei voi koskea aluetta, jolla maankäytön ohjaustarve edellyttää asemakaavan laatimista. Edellytyksenä on lisäksi, että yleiskaava ohjaa riittävästi rakentamista ja muuta maankäyttöä kyseisellä alueella.

{% include common/clause_start.html type="req" id="sp-yk/vaat-yk-kaytto-rakennusluvan-perusteena-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#tekstiarvo" title="TekstiArvo" %} (yksi kullakin kielellä), joka täydentää kaavamääräystietoa. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

### Käyttötarkoituksen osuus kerrosalasta
{% include common/clause_start.html type="req" id="sp-yk/vaat-osuus-kerrosalasta" %}
Aluevarauksen käyttötarkoitusta kuvaavaan kaavamääräykseen liitetty ```lisatieto```-attribuutti, jonka laji on [Käyttötarkoituksen osuus kerrosalasta](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/kayttotarkoituksenOsuusKerrosalasta), voi saada täsmälleen yhden arvon:
* Yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} jotka kertovat sallitun, käyttötarkoitukseen kohdistettavan kerroalan määrän koko sallitusta kerrosalasta joko kerrosneliömetreinä (```k-m2```) tai prosentteina (```%```). Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta.
{% include common/clause_end.html %}

Mikäli sallittua rakentamisen määrää ei ole jaoteltu käyttötarkoituksittain, ei lisätietoja käytetä.

{% include common/question.html content="Eikö olisi vain selkeämpää päättää, että käytetään esim. prosentteja? Eikä käytetä joko-tai -tyyppisiä vaihtoehtoja?" %}

<!--
## Kulttuuriymparistöarvojen alue
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/kulttuuriymparistoarvojenAlue>

{% include common/clause_start.html type="req" id="sp-ak/vaat-kulttuuriymparistoarvojen-alue" %}
* ```arvo```-attribuutin arvona saa esiintyä nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#tekstiarvo" title="TekstiArvo" %} (yksi kullakin kielellä), joka täydentää kaavamääräystietoa. Muun tyyppiset arvot eivät ole sallittuja.
* ```lisatieto```-attribuutin arvoina saa esiintyä nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#lisatieto" title="Lisatieto" %} joka ```laji``` on yksi seuraavista:   
   * [Kulttuurihistoriallinen merkittävyys](http://uri.suomi.fi/codelist/rytj/RY_LisatiedonLaji_AK/code/05), jonka arvoina on yksi tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#koodiarvo" title="KoodiArvo" %} jotka viittaavat johonkin [Kulttuurihistoriallinen merkittävyys](http://uri.suomi.fi/codelist/rakrek/kulthistmer) koodiston koodeista,
   * [Kulttuurihistoriallinen arvotyyppi](http://uri.suomi.fi/codelist/rytj/RY_LisatiedonLaji_AK/code/06), jonka arvoina on yksi tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#koodiarvo" title="KoodiArvo" %} jotka viittaavat johonkin [Kulttuurihistoriallinen arvotyyppi](http://uri.suomi.fi/codelist/rakrek/Kulthistatyyp) koodiston koodeista,
   * [Kulttuurihistoriallinen tyyppi](http://uri.suomi.fi/codelist/rytj/RY_LisatiedonLaji_AK/code/07), jonka arvoina on yksi tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#koodiarvo" title="KoodiArvo" %} jotka viittaavat johonkin [Kulttuurihistoriallinen tyyppi](http://uri.suomi.fi/codelist/rakrek/kulthistyyp) koodiston koodeista, tai
   * [Kulttuurihistoriallisen merkittävyyden kriteerit](http://uri.suomi.fi/codelist/rytj/RY_LisatiedonLaji_AK/code/08), jonka arvoina on yksi tai useampi{% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#koodiarvo" title="KoodiArvo" %} joka viittaa johonkin [Kulttuurihistoriallisen merkittävyyden kriteerit](http://uri.suomi.fi/codelist/rakrek/KultKritee) koodiston koodeista.
Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}
-->