---
layout: "default"
description: ""
id: "suunnittelutarvealue"
status: "Ehdotus"
---
# Suunnittelutarvealue
{:.no_toc}

**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/suunnittelutarveAlue>

{:toc}

{% include common/clause_start.html type="req" id="sp-yk/vaat-suunnittelutarvealue-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä joko
* yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} joka kuvaa sen kaavan hyväksymisestä alkavan ajanjakson pituuden, jona suunnittelutarvealue-status on voimassa. Numeerisen arvon  on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#integer" title="Integer" %}-rajapinta. Yksikkönä vuosi (```v```), tai kuukausi (```kk```) tai
* yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#ajanhetkiarvo" title="Ajanhetkiarvo" %} joka kuvaa päivämäärän, johon saakka suunnittelutarvealue-status on voimassa.

Lisäksi ```arvo```-attribuutin arvoina saa esiintyä yksi tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#tekstiarvo" title="TekstiArvo" %} (yksi kullakin kielellä), joka täydentää kaavamääräystietoa.

Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}