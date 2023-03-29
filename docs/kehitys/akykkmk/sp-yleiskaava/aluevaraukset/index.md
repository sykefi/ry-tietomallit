---
layout: "default"
description: ""
id: "aluevaraukset"
status: "Ehdotus"
---
# Yleiskaavan aluevaraukset

{% include common/clause_start.html type="req" id="sp-yk/vaat-aluemainen-aluevaraus" %}
Yleiskaavan aluevaraus on {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavakohde" title="Kaavakohde" %}-luokan objekti, jonka ```geometria```-attribuutin kuvaama geometria on aluemainen.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-yk/vaat-aluevaraus-maar" %}
Yleiskaavan aluevaraus liittyy assosiaatiolla ```maarays``` yhteen tai useampaan sellaiseen [Kaavamaarays](dokumentaatio/#kaavamaarays)-luokan objektiin, jonka ```laji```-attribuutin arvo on jokin [Kaavamääräyslaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays)-koodiston arvoista, joka sisältyy määrityshierarkioihin  ```Aluevaraus``` ja ```Yleiskaava```. Aluevarauksen pääkäyttötarkoitus osoitetaan lisätiedonlajilla [Pääkäyttötarkoitus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/paakayttotarkoitus).
{% include common/clause_end.html %}