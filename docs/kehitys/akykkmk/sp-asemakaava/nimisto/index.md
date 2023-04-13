---
layout: "default"
description: ""
id: "nimisto"
status: "Ehdotus"
---
# Kaavamääräyslajit - nimistö
{:.no_toc}

**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/nimisto>

Ryhmittelyotsikko, vain {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar" title="alakoodeja" %} käytetään.

{% include common/clause_start.html type="req" id="sp-ak/vaat-nimisto-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#tekstiarvo" title="TekstiArvo" %} (yksi kullakin kielellä), jolla annetaan kaavakohteen nimi, kohteelle liitetyn kaavamääräyksen perusteella joko [Torin tai aukion nimi](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/torinTaiKatuaukionNimi), [Puiston tai muun yleisen alueen nimi](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/puistonTaiMuunYleisenAlueenNimi), [Kadun tai tien nimi](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/kadunTaiTienNimi) tai [Kaupungin- tai kunnanosan nimi](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/kaupunginTaiKunnanosanNimi). Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}