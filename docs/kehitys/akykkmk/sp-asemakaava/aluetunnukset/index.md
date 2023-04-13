---
layout: "default"
description: ""
id: "aluetunnukset"
status: "Ehdotus"
---
# Kaavamääräyslajit - Aluetunnukset
{:.no_toc}

**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/aluetunnukset>

Ryhmittelyotsikko, vain [Alakoodeja](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar) käytetään.

{% include common/clause_start.html type="req" id="sp-ak/vaat-aluetunnukset-arvot" %}
```arvo```-attribuutin arvona saa esiintyä yksi [Numeerinen arvo](https://tietomallit.suomi.fi/model/rytj-kaava/NumeerinenArvo/).  Numeerisen arvon on toteutettava [Integer](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/dokumentaatio/#integer)-rajapinta. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-korttelin-numero-kohdennus" %}
[Korttelin numero](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/korttelinNumero>) on kohdennettava  
 [Kaavakohteeseen](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/), joka kuvaa [Aluevarausta](../../aluevaraukset/index.md). Samaa korttelin numeroa voidaan tarvittaessa käyttää useammalle Aluevaraukselle, jotka sijaitsevat maantieteellisesti vierekkäin. Tällöin näiden aluevarausten tulkitaan muodostavan samaa korttelia.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-tontin-numero-kohdennus" %}
[Tontin numero](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/tontinNumero>) on osoitettava [Kaavakohteeseen](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/), johon liittyy kaavamääräyslaji-koodi [sitovanTonttijaonMukainenTontti](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/sitovanTonttijaonMukainenTontti) tai [ohjeellinenTontti](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/ohjeellinenTontti).
{% include common/clause_end.html %}