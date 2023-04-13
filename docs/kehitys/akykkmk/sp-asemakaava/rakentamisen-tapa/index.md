---
layout: "default"
description: ""
id: "rakentamisen-tapa"
status: "Ehdotus"
---

# Kaavamääräykset - suureet / Rakentamisen tapa
{:.no_toc}

## Rakentamisen tapa

### Kattokaltevuus
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/kattokaltevuus>

{% include common/clause_start.html type="req" id="sp-ak/vaat-kattokaltevuus-arvot" %}
```arvo```-attribuutin arvoja saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} joka kertoo rakennusten katon sallitun kaltevuuden asteina (```deg```) sen kaavakohteen alueella, johon kaavamääräys on liitetty. Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

### Rakennuksen harjan suunta
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennuksenHarjanSuunta>

{% include common/clause_start.html type="req" id="sp-ak/vaat-harjasuunta-arvot" %}
```arvo```-attribuutin arvona saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} jotka kertovat rakennusten katon harjan sallitun kompassisuunnan asteina (```deg```) sen kaavakohteen alueella, johon kaavamääräys on liitetty. Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

### Ääneneristävyys
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/aaneneristavyys>

{% include common/clause_start.html type="req" id="sp-ak/vaat-aaneneristavyys-arvot" %}
```arvo```-attribuutin mahdolliset arvot ovat seuraavat:
* Yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} joka kuvaa vähimmäisääneneristävyyden melua vastaan desibeleinä (```db```). Numeerisen arvon on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta.
{% include common/clause_end.html %}

Esimerkki:
<br>
* Kaavakohde, jolla määräyksinä [Melueste](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/melueste) sekä [Ääneneristävyys](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/aaneneristavyys) ```arvo```lla 20 (desibeliä).

### Vihertehokkuus
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/vihertehokkuus>

{% include common/clause_start.html type="req" id="sp-ak/vaat-vihertehokuus-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä nolla tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} joka kertoo {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavakohde" title="Kaavakohteen" %} alueen tonttien viherkertoimen vähimmäisarvon. Numeerisen arvon on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta. Muun tyyppiset arvot eivät ole sallittuja.

### Etäisyys tontin rajasta
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/etaisyysTontinRajasta>

{% include common/clause_start.html type="req" id="sp-ak/vaat-etaisyys-naapuritontin-rajasta-arvot" %}
```arvo```-attribuutin mahdolliset arvot ovat seuraavat:
* Yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} joka kertoo kaavakohteen vähimmäisetäisyyden naapuritontin rajasta sen {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavakohde" title="Kaavakohteen" %} alueella, johon kaavamääräys on liitetty. Numeerisen arvon on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta. Yksikkönä metri (```m```).
{% include common/clause_end.html %}