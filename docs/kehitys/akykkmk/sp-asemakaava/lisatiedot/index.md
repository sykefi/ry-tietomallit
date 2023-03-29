---
layout: "default"
description: ""
id: "lisatiedot"
status: "Ehdotus"
---

# Kaavamääräyksen lisätiedot
{:.no_toc}

{% include common/clause_start.html type="req" id="sp-ak/vaat-kaavamaarayksen-lisatieto" %}
Kaavamääräyksen lisätiedot ovat kaavamääräystä täsmentäviä tietoja, jotka ei voida käyttää yksinään. Kaavamääräyksen lisätieto liittyy aina Kaavamääräykseen, jolle on annettu '''laji''' kaavamääräyslaji-koodiston arvolla.
{% include common/clause_end.html %}

## Tyyppi
Kaavamääräyksen tarkempi tyypittely. Ryhmittelyotsikko, vain {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar" title="alakoodeja" %} käytetään.

### Pääkäyttötarkoitus
Kaavamääräyksen lisätiedolla [Pääkäyttötarkoitus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/paakayttotarkoitus) annotoidaan [Aluevarauksille](../aluevaraukset/index.md) annettuista {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#kaavamaarays" title="Kaavamääräyksistä" %} pääkäyttötarkoitus. Pääkäyttötarkoituksella tarkoitetaan sitä käyttötarkoitusta, johon suhteellisesti suurin osa alueen rakennusoikeudesta on tarkoitettu.

{% include common/clause_start.html type="req" id="sp-yk/paakayttotarkoitus" %}
[Aluevarauksiin](../aluevaraukset/index.md) liittyvistä, käyttötarkoituksen kuvaavista {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#kaavamaarays" title="Kaavamääräyksistä" %} yhdelle tai useammalle on merkittävä {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#lisatieto" title="Lisatiedoksi" %} [Pääkäyttötarkoitus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/paakayttotarkoitus). Pääkäyttötarkoituksia voi liittyä {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#kaavakohde" title="Kaavakohteelle" %} useampia, mikäli useampi käyttötarkoitus on tarkoitettu  osuudeltaan yhtäsuureksi.
{% include common/clause_end.html %}

### Osa-alue
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/osaAlue>
{% include common/clause_start.html type="req" id="sp-ak/vaat-aluemainen-osaalue" %}
Asemakaavan alueen osa on {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavakohde" title="Kaavakohde" %}-luokan objekti, jonka ```geometria```-attribuutin kuvaama geometria on aluemainen.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-osaalue-maar" %}
Asemakaavan osa-alue liittyy assosiaatiolla ```maarays``` yhteen tai useampaan sellaiseen [Kaavamaarays](dokumentaatio/#kaavamaarays)-luokan objektiin, jonka ```laji```-attribuutin arvo on jokin [Kaavamääräyslaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays)-koodiston arvoista, joka sisältyy määrityshierarkiaan ```Asemakaava```, ei sisälly määrityshierarkiaan ```Suure```, ja jonka lisätiedon arvoksi on annettu [Osa-alue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/osaAlue).
{% include common/clause_end.html %}

### Poisluettava käyttötarkoitus
Kaavamääräyksen ```lisatieto```-attribuutin arvoina saa esiintyä nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#lisatieto" title="Lisatieto" %} jonka laji on [Poisluettava käyttötarkoitus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/poisluettavaKayttotarkoitus), ja jonka ```arvo```-attribuutin arvoina on yksi tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#koodiarvo" title="KoodiArvo" %} jotka viittaavat [Kaavamääräys](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays)-koodiston koodeihin, jotka sisältyvät ```Aluevaraus```-määrityshierarkiaan. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

Poisluettavat käyttötarkoituslajit tulee valita siten, että ne kohdistuvat ```arvo```-attribuuttien avulla valittuun yleispiirteisempään joukkoon käyttötarkoituksia pois lukien niistä osan.

Esimerkkejä: 
* [Toimitilojen alue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/toimitilojenAlue) pois lukien [Tuotantorakennusten alue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/tuotantorakennustenAlue).

## Rakentamisen ohjaus

Ryhmittelyotsikko, vain {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar" title="alakoodeja" %} käytetään.

### Rakentamistapaohje huomioitava
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/rakentamistapaOhjeHuomioitava>

{% include common/clause_start.html type="rec" id="sp-ak/suos-sitovat-rakentamistapaohjeet-liittyva-asiakirja" %}
Rakentamistapaohje on suositeltavaa linkittää kaavamääräykseen ```liittyvaAsiakirja```-assosiaation avulla.
{% include common/clause_end.html %}

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