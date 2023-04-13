---
layout: "default"
description: ""
id: "korkeusasema"
status: "Ehdotus"
---
# Kaavamääräykset - korkeusasema
{:.no_toc}

**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/korkeusasema>

1. 
{:toc}

### Korkeusasema

## Maanpinnan korkeusasema
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/maanpinnanKorkeusasema>

{% include common/clause_start.html type="req" id="sp-ak/vaat-maanpinnan-korkeusasema" %}
Kaava-aineistossa voidaan ilmaista maanpinnan nimelliskorkeus merenpinnasta tietyissä pisteissä kaavamääräyksenä kaavamääräyslaji-koodin [Maanpinnan korkeusasema](#maanpinnan-korkeusasema) ja sen arvon avulla.
{% include common/clause_end.html %} 

{% include common/clause_start.html type="req" id="sp-ak/vaat-maanpinnan-korkeusasema-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi [Korkeuspiste](https://tietomallit.suomi.fi/model/rytj-kaava/Korkeuspiste/) tai yksi [Korkeusväli](https://tietomallit.suomi.fi/model/rytj-kaava/Korkeusvali/) jotka kertovat maanpinnan korkeuden merenpinnasta sovitun pystysuuntaisen koordinaatiston arvona kaavakohteen sijainnissa. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Vesikaton ylimmän kohdan korkeusasema
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/vesikatonYlimmanKohdanKorkeusasema>

{% include common/clause_start.html type="req" id="sp-ak/vaat-vesikaton-korkeusasema-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi [Korkeuspiste](https://tietomallit.suomi.fi/model/rytj-kaava/Korkeuspiste/) tai yksi [Korkeusväli](https://tietomallit.suomi.fi/model/rytj-kaava/Korkeusvali/) jotka kertovat kaavakohteen alueelle sijoitettavien rakennusten vesikaton ylimmän kohdan korkeuden merenpinnasta sovitun pystysuuntaisen koordinaatiston arvona. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Julkisivupinnan ja vesikaton leikkauskohdan korkeusasema
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/julkisivupinnanJaVesikatonLeikkauskohdanKorkeusasema>

{% include common/clause_start.html type="req" id="sp-ak/vaat-julkisivupinnan-ja-vesikaton-leikkauksen-korkeusasema-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi [Korkeuspiste](https://tietomallit.suomi.fi/model/rytj-kaava/Korkeuspiste/) tai yksi [Korkeusväli](https://tietomallit.suomi.fi/model/rytj-kaava/Korkeusvali/) jotka kertovat kaavakohteen alueelle sijoitettavien rakennusten julkisivupinnan ja vesikaton leikkauskohdan korkeuden merenpinnasta sovitun pystysuuntaisen koordinaatiston arvona. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Julkisivun enimmäiskorkeus
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/julkisivunEnimmaiskorkeus>

{% include common/clause_start.html type="req" id="sp-ak/vaat-julkisivun-enimmaiskorkeus-arvot" %}
```arvo```-attribuutin arvona saa esiintyä yksi [Numeerinen arvoväli](https://tietomallit.suomi.fi/model/rytj-kaava/NumeerinenArvovali/) joka kertoo kaavakohteen alueelle sijoitettavien rakennusten julkisivujen minimikorkeuden, maksimikorkeuden tai molemmat. Numeerisen arvon on toteutettava [Integer](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/dokumentaatio/#real)-rajapinta. Yksikkönä metri (```m```). Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Rakennusten, rakenteiden ja laitteiden ylin korkeusasema
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/rakennustenRakenteidenJaLaitteidenYlinKorkeusasema>

{% include common/clause_start.html type="req" id="sp-ak/vaat-rakennusten-rakent-lait-korkeusasema-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi [Korkeuspiste](https://tietomallit.suomi.fi/model/rytj-kaava/Korkeuspiste/) tai yksi [Korkeusväli](https://tietomallit.suomi.fi/model/rytj-kaava/Korkeusvali/) jotka kertovat kaavakohteen alueelle sijoitettavien rakennusten, rakenteiden ja laitteiden ylimmän korkeuden merenpinnasta sovitun pystysuuntaisen koordinaatiston arvona. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Maanalaisen kohteen korkeusasema
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/maanalaisenKohteenKorkeusasema>

{% include common/clause_start.html type="req" id="sp-ak/vaat-maanalaisen-kohteen-korkeusasema-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi [Korkeuspiste](https://tietomallit.suomi.fi/model/rytj-kaava/Korkeuspiste/) tai yksi [Korkeusväli](https://tietomallit.suomi.fi/model/rytj-kaava/Korkeusvali/) jotka kertovat maanalaisen kaavakohteen perustason korkeuden merenpinnasta sovitun pystysuuntaisen koordinaatiston arvona. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Alin painovoimainen viemäröintitaso
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/alinPainovoimainenViemarointitaso>

{% include common/clause_start.html type="req" id="sp-ak/vaat-alin-painovoimainen-viemarointitaso-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi [Korkeuspiste](https://tietomallit.suomi.fi/model/rytj-kaava/Korkeuspiste/) joka kertoo alimman painovoimaisen viemäröintitason korkeuden sovitun pystysuuntaisen koordinaatiston arvona. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}