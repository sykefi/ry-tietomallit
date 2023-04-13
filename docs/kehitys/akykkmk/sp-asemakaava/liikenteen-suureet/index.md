---
layout: "default"
description: ""
id: "liikenteen-suureet"
status: "Ehdotus"
---

# Kaavamääräykset - suureet / Liikenteen suureet

## Liikenteen suureet
### Pysäköinnin määrä
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/pysakoinninMaara>

Ryhmittelyotsikko, vain [Alakoodeja](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar) käytetään.

Niin moottoajoneuvoille kuin polkupyörille varattujen pysäköintipaikkojen määrä voidaan ilmaista usealla tavalla.

Ilmaistaessa pysäköintipaikkojen kokonaismäärää, käytetään joko Kaavamääräys-koodia [Pyöräpaikkojen määrä](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/pyorapaikkojenMaara) tai [Autopaikkojen määrä](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/autopaikkojenMaara).

Ilmaistaessa pysäköintipaikkojen lukumäärää per asunto, käytetään joko Kaavamääräys-koodia [Pyöräpaikkojen määrä asuntoa kohden](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/pyorapaikkojenMaaraAsuntoaKohden) tai [Autopaikkojen määrä asuntoa kohden](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/autopaikkojenMaaraAsuntoaKohden).

Ilmaistaessa pysäköintipaikkojen lukumäärää per kerrosneliömetri, käytetään Kaavamääräys-koodia [Pyöräpaikkojen määrä kerrosneliömetriä kohden](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/pyorapaikkojenMaaraKerrosneliometriaKohden). tai [Autopaikkojen määrä kerrosneliömetriä kohden](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/autopaikkojenMaaraKerrosneliometriaKohden). Lisätiedon [Käyttötarkoituskohdistus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatiedonlaji/code/kayttotarkoituskohdistus) ja sen ```arvo```-attribuutin avulla täsmennetään, minkä käyttötarkoituksen mukaiseen kerrosalaan pysäköinnin määrää verrataan.

{% include common/tip.html content="Mikäli halutaan antaa pysyköintipaikojen lukumäärät erikseen eri käyttötarkoituksille, voidaan kaavakohteella käyttää useampaa kaavamääräyksen ja sen lisätiedon yhdistelmää yllä kuvatulla tavalla kutakin käyttötarkoitusta kohden." %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-pysakointipaikkojen-maara-arvot" %}
```arvo```-attribuutin arvona saa esiintyä yksi [Numeerinen arvoväli](https://tietomallit.suomi.fi/model/rytj-kaava/NumeerinenArvovali/) joka kertoo vaaditun pysäköintipaikkojen minimimäärän, maksimimäärän tai molemmat sen [Kaavakohteen](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/) aluella, johon kaavamääräys on liitetty. Numeerisen arvovälin minimi- ja maksimiarvojen on toteutettava [Integer](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/dokumentaatio/#real)-rajapinta. Yksikköä ei kirjata. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}