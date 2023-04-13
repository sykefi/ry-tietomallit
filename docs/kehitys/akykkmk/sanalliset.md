---
layout: "default"
description: ""
id: "sanalliset"
status: "Ehdotus"
---
# Sanalliset kaavamääräykset
{:.no_toc}

Tekstimuotoisina annettujen, sanallisten kaavamääräysten koneellinen tulkittavuus on monimutkaisempaa kuin kuvattaessa sama ohjausvaikutus koodistojen arvojen tai numeeristen arvojen avulla. Tekstimuotoiset arvot ovat kuitenkin usein tarpeen, koska kaikkia mahdollisia yksityiskohtaisia kaavamääräyksiä ei ole mielekästä tai edes mahdollista koodittaa. Ihmisen tulee todennäköisesti aina tarkistaa tekstimuotoisten kaavamääräysten tulkinta, mikä heikentää kaavatiedon koneellista tulkintaa. Tämän vuoksi tekstimuotoisia kaavamääräysten ja niiden lisätietojen arvoja tulee käyttää kuvaamaan vain näitä täydentävää tai täsmentävää sisältöä.

{% include common/clause_start.html type="req" id="laatu/vaat-vain-tarpeelliset-tekstiarvot" %}
Mikäli [Kaavamaarays](dokumentaatio/#kaavamaarays)- tai [Lisatieto](dokumentaatio/#lisatieto)-luokkien ```arvo```-attribuuteille on annettu nollasta poikkeava määrä [TekstiArvo](dokumentaatio/#tekstiarvo)-tyyppisiä arvoja, tulee niitä käyttää lähtökohtaisesti täydentämään tai täsmentämään kaavamääräyksen tai lisätiedon muiden attribuuttien avulla kuvattua merkitystä.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="laatu/vaat-sanallisten-maaraysten-luokittelu" %}
Sanallisilla kaavamääräyksillä tarkoitetaan kaavatietomallissa kaavamääräystä, jolle on annettu Kaavamääräyksen ```lajiksi``` [Sanallinen määräys](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/sanallinenMaarays) ja ```arvo```-attribuutille {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#tekstiarvo" title="TekstiArvo" %} Sanalliset kaavamääräykset on annotoitava [Sanallisen määräyksen laji](<http://uri.suomi.fi/codelist/rytj/RY_Sanallisen_Kaavamaarayksen_Laji/>) -koodein.
{% include common/clause_end.html %}

{% include common/tip.html content="Sanallisten kaavamääräysten luokittelun avulla mahdollistetaan sisällöltään usein hyvin vaihtelevien sanallisten kaavamäärästen älykäs etsittävyys ja luokiteltavuus. Tyypillisesti seikat, joita ei voida pelkin koodiarvoin kuvata, liittyvät esimerkiksi kaavakohteen toteutustapaan tai jonkin ilmiön erityiseen huomiomiseen." %}

{% include common/clause_start.html type="req" id="laatu/vaat-otsikointi-nimi" %}
[Kaavamaarays](dokumentaatio/#kaavamaarays)-, [Kaavasuositus](dokumentaatio/#kaavasuositus)- ja [Kaavakohde](dokumentaatio/#kaavakohde)-luokkien instanssien mahdolliseen ei-oikeusvaikutteiseen otsikointiin tulee käyttää niiden ```nimi```-attribuutteja.
{% include common/clause_end.html %}