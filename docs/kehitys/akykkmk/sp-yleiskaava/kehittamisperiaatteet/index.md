---
layout: "default"
description: ""
id: "kehittamisperiaatteet"
status: "Ehdotus"
---
# Kaavamääräyslajit - kehittämisperiaatteet
{:.no_toc}

**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/alueJotaKoskeeKehittamisperiaate>

1. 
{:toc}

## Yhdyskuntarakenteen laajenemissuunta
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/yhdyskuntarakenteenLaajenemissuunta>

{% include common/clause_start.html type="req" id="sp-yk/vaat-yhdyskuntarakenteen-laajenemissuunta-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä nolla tai useampi [Koodiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Koodiarvo/) [Kaavamääräyslaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji)-koodiston arvoa, jotka sisältyy määrityshierarkioihin ```Aluevaraus``` ja ```Yleiskaava``` ja joiden avulla voidaan kuvata laajenevan yhdyskuntarakenteen käyttötarkoitukset. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-yk/vaat-yhdyskuntarakenteen-laajenemissuunta-geometria" %}
[Kaavakohteen](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/), johon liittyy Yhdyskuntarakenteen laajenemissuunta -lajin kaavamääräys, ```geometria```-attribuutin arvon tulee olla pistemäinen, ja sen tulee sijaita paikassa, josta yhdyskuntarakenne laajenee ```arvo```-attribuutin osoittamaan suuntaan.  
{% include common/clause_end.html %}

<!--
## Kävely-ympäristön kehittämistarve
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_KaavamaarayslajiLaji_YK/code/0412>

{% include common/clause_start.html type="req" id="sp-yk/vaat-kavely-ympariston-kehittamistarve-maar" %}
Ilmaisee, että kaavakohde kuvaa kävely-ympäristön kehittämistarpeen.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-yk/vaat-kavely-ympariston-kehittamistarve-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä nolla tai useampi [Tekstiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Tekstiarvo/) (yksi kullakin kielellä), joka täydentää kaavamääräystietoa. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}
-->
<!--
## Meluntorjuntatarve
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_KaavamaarayslajiLaji_YK/code/0414>

{% include common/clause_start.html type="req" id="sp-yk/vaat-meluntorjuntatarve-maar" %}
Ilmaisee, että kaavakohde kuvaa alueen, jolla esiintyy siinä määrin melua, että siitä voi aiheutua merkittävää haittaa. Meluntorjunta tulee huomioida alueen käyttöä ja rakentamista suunniteltaessa.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-yk/vaat-meluntorjuntatarve-arvot" %}
```arvo```-attribuutin arvona saa esiintyä nolla tai useampi [Tekstiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Tekstiarvo/) (yksi kullakin kielellä), jolla kuvataan melun tyyppiä ja haitallisuutta. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}-->