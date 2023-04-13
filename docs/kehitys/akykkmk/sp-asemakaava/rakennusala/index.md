---
layout: "default"
description: ""
id: "rakennusala"
status: "Ehdotus"
---
# Kaavamääräykset - Rakennusala

## Rakennusala
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusala>

{% include common/clause_start.html type="req" id="sp-ak/vaat-rakennusala-arvot" %}
```arvo```-attribuutin mahdolliset arvot ovat seuraavat:
* Nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#koodiarvo" title="KoodiArvo" %} jotka kuvaa rakennusalalle rakennettavaksi tarkoitetun rakennuksen lajin viittaamalla koodistoon [Rakennusluokitus 2018](http://uri.suomi.fi/codelist/jhs/rakennus_1_20180712).
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-rakennusala-liittyvakohde" %}
Kaavakohteeseen, johon liittyy kaavamääräyslaji-koodi [Rakennusala](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusala), tulee {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#liittyvakohde" title="Liittyvakohde" %}-assosiaation avulla linkittää se (Aluevaraus)[/../../aluevaraukset/index.md], jonka sisälle rakennusala spatiaalisesti sijoittuu.
{% include common/clause_end.html %}

### Rakennusalan sivu, jota koskee tarkempi määräys
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusalanSivuJotaKoskeeTarkempiMaarays>
{% include common/clause_start.html type="req" id="sp-ak/vaat-rakennusalan-sivu" %}
{% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavakohde" title="Kaavakohteen" %}, johon liittyy {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavamaarays" title="Kaavamääräyslaji" %} [Rakennuksen sivu, jota koskee tarkempi määräys](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusalanSivuJotaKoskeeTarkempiMaarays), tulee geometrialtaan olla päällekkäinen toisen {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavakohde" title="Kaavakohteen" %} geometrian kanssa, johon liittyy {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavamaarays" title="Kaavamääräys" %} [Rakennusala](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusala).
{% include common/clause_end.html %}

### Rakennuksen sivu, jossa suora uloskäynti porrashuoneista
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusalanSivuJossaSuoraUloskayntiPorrashuoneista>

{% include common/clause_start.html type="req" id="sp-ak/vaat-suora-uloskaynti-porrashuoneista-arvot" %}
{% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavakohde" title="Kaavakohteen" %}, johon liittyy {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavamaarays" title="Kaavamääräyslaji" %} [Rakennuksen sivu, jossa suora uloskäynti porrashuoneista](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusalanSivuJossaSuoraUloskayntiPorrashuoneista), tulee geometrialtaan olla päällekkäinen toisen {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavakohde" title="Kaavakohteen" %} geometrian kanssa, johon liittyy {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavamaarays" title="Kaavamääräys" %} [Rakennusala](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusala)
{% include common/clause_end.html %}

### Ikkunaton seinä
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/ikkunatonSeina>

{% include common/clause_start.html type="req" id="sp-ak/vaat-ei-ikkunoita-geometria" %}
{% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavakohde" title="Kaavakohteen" %}, johon liittyy {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavamaarays" title="Kaavamääräys" %} [Ikkunaton seinä](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/ikkunatonSeina), tulee geometrialtaan olla päällekkäinen toisen {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavakohde" title="Kaavakohteen" %} geometrian kanssa, johon liittyy {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavamaarays" title="Kaavamääräys" %} [Rakennusala](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusala)
{% include common/clause_end.html %}