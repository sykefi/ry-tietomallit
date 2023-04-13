---
layout: "default"
description: ""
id: "aluetunnukset"
status: "Ehdotus"
---
# Kaavamääräyslajit - Aluetunnukset
{:.no_toc}

**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/aluetunnukset>

Ryhmittelyotsikko, vain {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar" title="alakoodeja" %} käytetään.

{% include common/clause_start.html type="req" id="sp-ak/vaat-aluetunnukset-arvot" %}
```arvo```-attribuutin arvona saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %}.  Numeerisen arvon on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#integer" title="Integer" %}-rajapinta. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-korttelin-numero-kohdennus" %}
[Korttelin numero](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/korttelinNumero>) on kohdennettava  
 {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#kaavakohde" title="Kaavakohteeseen" %}, joka kuvaa [Aluevarausta](../../aluevaraukset/index.md). Samaa korttelin numeroa voidaan tarvittaessa käyttää useammalle Aluevaraukselle, jotka sijaitsevat maantieteellisesti vierekkäin. Tällöin näiden aluevarausten tulkitaan muodostavan samaa korttelia.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-tontin-numero-kohdennus" %}
[Tontin numero](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/tontinNumero>) on osoitettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#kaavakohde" title="Kaavakohteeseen" %}, johon liittyy kaavamääräyslaji-koodi [sitovanTonttijaonMukainenTontti](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/sitovanTonttijaonMukainenTontti) tai [ohjeellinenTontti](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/ohjeellinenTontti).
{% include common/clause_end.html %}