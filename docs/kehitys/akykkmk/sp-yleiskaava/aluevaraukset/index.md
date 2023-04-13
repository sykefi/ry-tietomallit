---
layout: "default"
description: ""
id: "aluevaraukset"
status: "Ehdotus"
---
# Yleiskaavan aluevaraukset

{% include common/clause_start.html type="req" id="sp-yk/vaat-aluemainen-aluevaraus" %}
Yleiskaavan aluevaraus on [Kaavakohde](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/)-luokan objekti, jonka ```geometria```-attribuutin kuvaama geometria on aluemainen.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-yk/vaat-aluevaraus-maar" %}
Yleiskaavan aluevaraus liittyy assosiaatiolla ```maarays``` yhteen tai useampaan sellaiseen [Kaavamaarays](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavamaarays/)-luokan objektiin, jonka ```laji```-attribuutin arvo on jokin [Kaavamääräyslaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji)-koodiston arvoista, joka sisältyy määrityshierarkioihin  ```Aluevaraus``` ja ```Yleiskaava```. Aluevarauksen pääkäyttötarkoitus osoitetaan lisätiedonlajilla [Pääkäyttötarkoitus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/paakayttotarkoitus).
{% include common/clause_end.html %}