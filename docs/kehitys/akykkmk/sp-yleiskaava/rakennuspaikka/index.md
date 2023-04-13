---
layout: "default"
description: ""
id: "rakennuspaikka"
status: "Ehdotus"
---
# Kaavamääräykset - Rakennuspaikka

## Rakennuspaikka
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennuspaikka>
{% include common/clause_start.html type="req" id="sp-yk/vaat-rakennuspaikka-lisatiedot" %}
```lisatieto```-attribuutin arvoina saa esiintyä nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#lisatieto" title="Lisatieto" %} jonka laji on [Käyttötarkoituskohdistus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/kayttotarkoituskohdistus), jolla on täsmälleen yksi ```arvo``` lajia {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#koodiarvo" title="KoodiArvo" %} joka viittaa johonkin [Rakennusluokitus 2018](http://uri.suomi.fi/codelist/jhs/rakennus_1_20180712)-koodiston koodiin. Mikäli vähintään yksi lisätieto on annettu, saa rakennuspaikkaan rakentaa vain lisätietojen avulla rajattuja rakennustyyppejä. Muun tyyppiset arvot eivät ole sallittuja.  
<!-- MRL 44 §, 72 § ja 77 § huomiointi -->
{% include common/clause_end.html %}

Esimerkkejä:<br>
* ```Asunnon rakennuspaikka``` voidaan määritellä käyttötarkoituskohdistus-lisätiedon Rakennusluokituksen 2018:n mukaisella arvolla [Asuinrakennukset](http://uri.suomi.fi/codelist/jhs/rakennus_1_20180712/code/01).

* ```Loma-asunnon rakennuspaikka``` voidaan määritellä käyttötarkoituskohdistus-lisätiedon Rakennusluokituksen 2018:n mukaisella arvolla [Vapaa-ajan asuinrakennukset](http://uri.suomi.fi/codelist/jhs/rakennus_1_20180712/code/02).

* ```Saunan rakennuspaikka``` voidaan määritellä käyttötarkoituskohdistus-lisätiedon Rakennusluokituksen 2018:n mukaisella arvolla [Saunarakennukset](http://uri.suomi.fi/codelist/jhs/rakennus_1_20180712/code/1910).

* ```Maatalouden talouskeskuksen rakennuspaikka``` voidaan määritellä kahden käyttötarkoituskohdistus-lisätiedon yhdistelmällä, arvoina Rakennusluokituksen 2018:n mukaiset [Asuinrakennukset](http://uri.suomi.fi/codelist/jhs/rakennus_1_20180712/code/01) ja [Maatalousrakennukset ja eläinsuojat](http://uri.suomi.fi/codelist/jhs/rakennus_1_20180712/code/14) yhdistelmällä.

{% include common/clause_start.html type="req" id="sp-yk/vaat-rakennuspaikka-tuulivoimayleiskaava" %}
[Maankäyttö- ja rakennuslain 77 a §](https://www.finlex.fi/fi/laki/ajantasa/1999/19990132#L10aP77a) mukaisissa yleiskaavoissa tuulivoimalan rakennuspaikka tulee kuvata kaavamääräyslajilla [Rakennuspaikka](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennuspaikka), joka sijaitsee spatiaalisesti sellaisen Kaavakohteen sisällä, johon liittyy kaavamääräyslaji [Tuulivoimala-alue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/tuulivoimalaAlue).
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-yk/vaat-tuulivoimalan-suureet" %}
[Maankäyttö- ja rakennuslain 77 a §](https://www.finlex.fi/fi/laki/ajantasa/1999/19990132#L10aP77a) mukaisissa yleiskaavoissa käytettäessä kaavamääräyslajikoodeja [Tuulivoimaloiden määrä](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/tuulivoimaloidenMaara) ja/tai [Tuulivoimalan enimmäiskorkeus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/tuulivoimalanEnimmaiskorkeus) tulee liittyä sellaiseen Kaavakohteeseen, johon liittyy myös kaavamääräyslaji [Tuulivoimala-alue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/tuulivoimalaAlue).
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-yk/vaat-44-72-lisatieto" %}
[Maankäyttö- ja rakennuslain 44 §](https://www.finlex.fi/fi/laki/ajantasa/1999/19990132#L5P44) ja [72 §](https://www.finlex.fi/fi/laki/ajantasa/1999/19990132#L10P72) mukaisissa yleiskaavoissa tulee [Rakennuspaikkaan](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennuspaikka) liittyä kaavamääräyksen lisätiedonlaji-koodiston koodi [Rakennusluvan peruste](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/rakennusluvanPeruste) ja tämän arvona [Yleiskaavan oikeusvaikutukset](https://koodistot.suomi.fi/codescheme;registryCode=rytj;schemeCode=oikeusvaik_YK) -koodiston arvo, joka vastaa rakennusluvan perusteena toimivaa pykälää, mikäli kohde määräyksineen toimii rakennusluvan perusteena.
{% include common/clause_end.html %}