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
* Nolla tai useampi [Koodiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Koodiarvo/) jotka kuvaa rakennusalalle rakennettavaksi tarkoitetun rakennuksen lajin viittaamalla koodistoon [Rakennusluokitus 2018](http://uri.suomi.fi/codelist/jhs/rakennus_1_20180712).
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-rakennusala-liittyvakohde" %}
Kaavakohteeseen, johon liittyy kaavamääräyslaji-koodi [Rakennusala](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusala), tulee  -assosiaation avulla linkittää se (Aluevaraus)[/../../aluevaraukset/index.md], jonka sisälle rakennusala spatiaalisesti sijoittuu.
{% include common/clause_end.html %}

### Rakennusalan sivu, jota koskee tarkempi määräys
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusalanSivuJotaKoskeeTarkempiMaarays>
{% include common/clause_start.html type="req" id="sp-ak/vaat-rakennusalan-sivu" %}
[Kaavakohteen](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/), johon liittyy [Kaavamääräyslaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/)-koodiston mukainen koodi [Rakennuksen sivu, jota koskee tarkempi määräys](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusalanSivuJotaKoskeeTarkempiMaarays), tulee geometrialtaan olla päällekkäinen toisen [Kaavakohteen](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/) geometrian kanssa, johon liittyy [Kaavamääräys](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavamaarays/) [Rakennusala](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusala).
{% include common/clause_end.html %}

### Rakennuksen sivu, jossa suora uloskäynti porrashuoneista
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusalanSivuJossaSuoraUloskayntiPorrashuoneista>

{% include common/clause_start.html type="req" id="sp-ak/vaat-suora-uloskaynti-porrashuoneista-arvot" %}
[Kaavakohteen](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/), johon liittyy [Kaavamääräyslaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/)-koodiston mukainen koodi [Rakennuksen sivu, jossa suora uloskäynti porrashuoneista](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusalanSivuJossaSuoraUloskayntiPorrashuoneista), tulee geometrialtaan olla päällekkäinen toisen [Kaavakohteen](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/) geometrian kanssa, johon liittyy [Kaavamääräys](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavamaarays/) [Rakennusala](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusala)
{% include common/clause_end.html %}

### Ikkunaton seinä
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/ikkunatonSeina>

{% include common/clause_start.html type="req" id="sp-ak/vaat-ei-ikkunoita-geometria" %}
[Kaavakohteen](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/), johon liittyy [Kaavamääräys](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavamaarays/) [Ikkunaton seinä](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/ikkunatonSeina), tulee geometrialtaan olla päällekkäinen toisen [Kaavakohteen](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/) geometrian kanssa, johon liittyy [Kaavamääräys](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavamaarays/) [Rakennusala](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennusala)
{% include common/clause_end.html %}