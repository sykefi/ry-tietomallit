---
layout: "default"
description: ""
id: "aluevaraukset"
status: "Ehdotus"
---
# Kaavamääräyslajit - aluevaraukset

## Aluevaraus

{% include common/clause_start.html type="req" id="sp-ak/vaat-aluemainen-aluevaraus" %}
Asemakaavan aluevaraus on [Kaavakohde](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/)-luokan objekti, jonka ```geometria```-attribuutin kuvaama geometria on aluemainen.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-kayttotarkoitusalue-maar" %}
Asemakaavan aluevaraus liittyy assosiaatiolla ```maarays``` yhteen tai useampaan sellaiseen [Kaavamaarays](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavamaarays/)-luokan objektiin, jonka ```laji```-attribuutin arvo on jokin [Kaavamääräyslaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji)-koodiston arvoista, joka sisältyy määrityshierarkioihin  ```Aluevaraus``` ja ```Asemakaava```.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-ei-leikkaavat-kayttotarkoitusalueet" %}
Asemakaavan aluevaraukset eivät saa leikata toisiaan. Toisin sanoen alueet eivät saa sijaita spatiaalisesti päällekkäin.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-asemakaavan-kayttotarkoituspeite" %}
Asemakaavan, jonka ```elinkaaritila```-attribuutin arvo on kaavaehdotus tai myöhempi (Kaavaehdotus, Tarkistettu kaavaehdotus, Hyväksytty kaava, Oikaisukehotuksen alainen, Valituksen alainen, Osittain voimassa, Voimassa, Kumottu tai Kumoutunut), sisältämien aluevarausten tulee peittää sen ```aluerajaus```-attribuutin ilmaisema kaavan alue siten, että jokainen alueen sisäinen sijaintipiste sisältyy täsmälleen yhteen aluevaraukseen.
{% include common/clause_end.html %}