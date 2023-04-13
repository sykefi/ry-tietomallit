---
layout: "default"
description: ""
id: "johdanto"
status: "Ehdotus"
---
# Kaavatietomallin soveltamisprofiili yleiskaava-aineistoille
{:.no_toc}

Tämän dokumentin vaatimukset ja suositukset muodostavat Kaavatietomallin loogisen tietomallin soveltamisprofiilin yleiskaava-aineistoille. Soveltamisprofiili kuvaa ne rajoitukset ja lisävaatimukset, joita tulee noudattaa [Kaavatietomallin](https://tietomallit.suomi.fi/model/rytj-kaava/) ja sen [sanallisen dokumentaation](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/dokumentaatio/) soveltamisessa yleiskaavojen tietoaineistojen kuvaamiseen.

<!--
Tämän muodollisen dokumentin tietoja täydentää [Yleiskaavan kaavamääräysopas](https://sykefi.github.io/kaavamaaraysoppaat/yleiskaava/), joka sisältää käytännön esimerkkejä Kaavatietomallin soveltamisesta yleiskaavoituksen kaavoitusratkaisuihin.-->

{% include common/clause_start.html type="req" id="sp-yk/vaat-yleiskaava-aineisto-maar" %}
Kaavatietomallin mukainen yleiskaava-aineisto koostuu [Kaava](https://tietomallit.suomi.fi/model/rytj-kaava/Kaava/)-luokan instansseista, joiden ```laji```-attribuutin arvo on jokin [Kaavalajit](https://koodistot.suomi.fi/codescheme;registryCode=rytj;schemeCode=RY_Kaavalaji)-koodiston koodin [Yleiskaava](http://uri.suomi.fi/codelist/rytj/RY_Kaavalaji/code/2) [Alakoodeista](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar), sekä näihin instansseihin Kaavatietomallin mukaisesti liittyvistä muiden luokkien instansseista.
{% include common/clause_end.html %}