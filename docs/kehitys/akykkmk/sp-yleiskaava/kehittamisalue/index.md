---
layout: "default"
description: ""
id: "kehittamisalue"
status: "Ehdotus"
---
# Kehittämisalue
{:.no_toc}

**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/kehittamisAlue>

{:toc}

{% include common/clause_start.html type="req" id="sp-yk/vaat-kehittamisalue-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä joko
* yksi [Numeerinen arvo](https://tietomallit.suomi.fi/model/rytj-kaava/NumeerinenArvo/) joka kuvaa sen kaavan hyväksymisestä alkavan ajanjakson pituuden, jona kehittämisalue-status on voimassa. Numeerisen arvon  on toteutettava [Integer](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/dokumentaatio/#integer)-rajapinta. Yksikkönä vuosi (```v```), tai kuukausi (```kk```) tai
* yksi [Ajanhetkiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Ajanhetkiarvo/) joka kuvaa päivämäärän, johon saakka kehittämisalue-status on voimassa.

Lisäksi ```arvo```-attribuutin arvoina saa esiintyä yksi tai useampi [Tekstiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Tekstiarvo/) (yksi kullakin kielellä), joka täydentää kaavamääräystietoa.

Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}