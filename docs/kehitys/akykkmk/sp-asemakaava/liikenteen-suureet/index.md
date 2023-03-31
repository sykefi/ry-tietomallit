---
layout: "default"
description: ""
id: "liikenteen-suureet"
status: "Ehdotus"
---

# Kaavamääräykset - suureet / Liikenteen suureet

## Liikenteen suureet
### Pysäköinnin määrä
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/pysakoinninMaara>

Ryhmittelyotsikko, vain {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar" title="alakoodeja" %} käytetään.

Niin moottoajoneuvoille kuin polkupyörille varattujen pysäköintipaikkojen määrä voidaan ilmaista usealla tavalla.

Ilmaistaessa pysäköintipaikkojen kokonaismäärää, käytetään joko Kaavamääräys-koodia [Polkupyöräpysäköinnin määrä](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/polkupyoraPysakoinninMaara) tai [Autopaikkojen määrä](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/autopaikkojenMaara).

Ilmaistaessa pysäköintipaikkojen lukumäärää per asunto, käytetään joko Kaavamääräys-koodia [Polkupyöräpysäköinnin määrä per asunto](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/polkupyoraPysakoinninMaaraPerAsunto) tai [Autopaikkojen määrä per asunto](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/autopaikkojenMaaraPerAsunto).

Ilmaistaessa pysäköintipaikkojen lukumäärää per kerrosneliömetri, käytetään Kaavamääräys-koodia [Polkupyöräpysäköinnin määrä per kerrosneliömetri](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/polkupyoraPysakoinninMaaraPerKerrosneliometri). tai [Autopaikkojen määrä per kerrosneliömetri](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/polkupyoraPysakoinninMaaraPerKerrosneliometri). Lisätiedon [Käyttötarkoituskohdistus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/kayttotarkoituskohdistus) ja sen ```arvo```-attribuutin avulla täsmennetään, minkä käyttötarkoituksen mukaiseen kerrosalaan pysäköinnin määrää verrataan.

{% include common/tip.html content="Mikäli halutaan antaa pysyköintipaikojen lukumäärät erikseen eri käyttötarkoituksille, voidaan kaavakohteella käyttää useampaa kaavamääräyksen ja sen lisätiedon yhdistelmää yllä kuvatulla tavalla kutakin käyttötarkoitusta kohden." %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-pysakointipaikkojen-maara-arvot" %}
```arvo```-attribuutin arvona saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} joka kertoo vaaditun pysäköintipaikkojen minimimäärän, maksimimäärän tai molemmat sen {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavakohde" title="Kaavakohteen" %} aluella, johon kaavamääräys on liitetty. Numeerisen arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta. Yksikköä ei kirjata. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}