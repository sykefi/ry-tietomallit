---
layout: "default"
description: ""
id: "suureet"
status: "Ehdotus"
---

# Kaavamääräykset - suureet
{:.no_toc}

Suure-tyyppisillä kaavamääräyksillä tarkoitetaan tässä [Kaavamääräys](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/)-koodiston koodeja, jotka sisältyvät määrityshierarkiaan ```Suure```.

{% include common/clause_start.html type="req" id="sp-ak/vaat-arvot" %}
Tyypiltään suuremaisille kaavamääräyksille on ```arvo```-attribuutin arvona annettava **täsmälleen yksi** {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %}, paitsi jos määräys kuuluu alaluokkaan [Nimistö](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/nimisto), jolloin arvon tulee olla tyyppiä {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#tekstiarvo" title="TekstiArvo" %} (yksi kullakin kielellä).
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-suureet-lisatiedot" %}
```lisatieto```-attribuutilla ei saa olla arvoja.
{% include common/clause_end.html %}