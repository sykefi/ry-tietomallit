---
layout: "default"
description: ""
id: "korkeusasema"
status: "Ehdotus"
---
# Kaavamääräykset - korkeusasema
{:.no_toc}

**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/korkeusasema>

1. 
{:toc}

### Korkeusasema

## Maanpinnan korkeusasema
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/maanpinnanKorkeusasema>

{% include common/clause_start.html type="req" id="sp-ak/vaat-maanpinnan-korkeusasema" %}
Kaava-aineistossa voidaan ilmaista maanpinnan nimelliskorkeus merenpinnasta tietyissä pisteissä kaavamääräyksenä kaavamääräyslaji-koodin [Maanpinnan korkeusasema](#maanpinnan-korkeusasema) ja sen arvon avulla.
{% include common/clause_end.html %} 

{% include common/clause_start.html type="req" id="sp-ak/vaat-maanpinnan-korkeusasema-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#korkeuspiste" title="Korkeuspiste" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#korkeusvali" title="Korkeusvali" %} jotka kertovat maanpinnan korkeuden merenpinnasta sovitun pystysuuntaisen koordinaatiston arvona kaavakohteen sijainnissa. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Rakennuksen vesikaton ylimmän kohdan korkeusasema
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/vesikatonYlimmanKohdanKorkeusasema>

{% include common/clause_start.html type="req" id="sp-ak/vaat-vesikaton-korkeusasema-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#korkeuspiste" title="Korkeuspiste" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#korkeusvali" title="Korkeusvali" %} jotka kertovat kaavakohteen alueelle sijoitettavien rakennusten vesikaton ylimmän kohdan korkeuden merenpinnasta sovitun pystysuuntaisen koordinaatiston arvona. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Rakennuksen julkisivupinnan ja vesikaton leikkauskohdan korkeusasema
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/julkisivupinnanJaVesikatonLeikkauskohdanKorkeusasema>

{% include common/clause_start.html type="req" id="sp-ak/vaat-julkisivupinnan-ja-vesikaton-leikkauksen-korkeusasema-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#korkeuspiste" title="Korkeuspiste" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#korkeusvali" title="Korkeusvali" %} jotka kertovat kaavakohteen alueelle sijoitettavien rakennusten julkisivupinnan ja vesikaton leikkauskohdan korkeuden merenpinnasta sovitun pystysuuntaisen koordinaatiston arvona. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Rakennuksen julkisivun enimmäiskorkeus
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/julkisivunEnimmaiskorkeus>

{% include common/clause_start.html type="req" id="sp-ak/vaat-julkisivun-enimmaiskorkeus-arvot" %}
```arvo```-attribuutin arvona saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} joka kertoo kaavakohteen alueelle sijoitettavien rakennusten julkisivujen minimikorkeuden, maksimikorkeuden tai molemmat. Numeerisen arvon on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta. Yksikkönä metri (```m```). Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Rakennusten, rakenteiden ja laitteiden ylin korkeusasema
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/rakennustenRakenteidenJaLaitteidenYlinKorkeusasema>

{% include common/clause_start.html type="req" id="sp-ak/vaat-rakennusten-rakent-lait-korkeusasema-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#korkeuspiste" title="Korkeuspiste" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#korkeusvali" title="Korkeusvali" %} jotka kertovat kaavakohteen alueelle sijoitettavien rakennusten, rakenteiden ja laitteiden ylimmän korkeuden merenpinnasta sovitun pystysuuntaisen koordinaatiston arvona. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Maanalaisen kohteen korkeusasema
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/maanalaisenKohteenKorkeusasema>

{% include common/clause_start.html type="req" id="sp-ak/vaat-maanalaisen-kohteen-korkeusasema-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#korkeuspiste" title="Korkeuspiste" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#korkeusvali" title="Korkeusvali" %} jotka kertovat maanalaisen kaavakohteen perustason korkeuden merenpinnasta sovitun pystysuuntaisen koordinaatiston arvona. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

## Alin painovoimainen viemäröintitaso
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/alinPainovoimainenViemarointitaso>

{% include common/clause_start.html type="req" id="sp-ak/vaat-alin-painovoimainen-viemarointitaso-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#korkeuspiste" title="Korkeuspiste" %} joka kertoo alimman painovoimaisen viemäröintitason korkeuden sovitun pystysuuntaisen koordinaatiston arvona. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}