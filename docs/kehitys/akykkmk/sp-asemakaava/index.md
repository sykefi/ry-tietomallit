---
layout: "default"
description: ""
id: "johdanto"
status: "Ehdotus"
---
# Kaavatietomallin soveltamisprofiili asemakaava-aineistoille
{:.no_toc}

Tämän dokumentin vaatimukset ja suositukset muodostavat Kaavatietomallin loogisen tietomallin soveltamisprofiilin asemakaava-aineistoille. Soveltamisprofiili kuvaa ne rajoitukset ja lisävaatimukset, joita tulee noudattaa [Kaavatietomallin](https://tietomallit.suomi.fi/model/rytj-kaava/) ja sen [sanallisen dokumentaation](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/dokumentaatio/) soveltamisessa asemakaavojen tietoaineistojen kuvaamiseen.

Tämän muodollisen dokumentin tietoja täydentää [Asemakaavan kaavamääräysopas](https://sykefi.github.io/kaavamaaraysoppaat/asemakaava/), joka sisältää käytännön esimerkkejä Kaavatietomallin soveltamisesta asemakaavoituksen kaavoitusratkaisuihin.

{% include common/clause_start.html type="req" id="sp-ak/vaat-asemakaava-aineisto-maar" %}
Kaavatietomallin mukainen asemakaava-aineisto koostuu [Kaava](https://tietomallit.suomi.fi/model/rytj-kaava/Kaava/)-luokan instansseista, joiden ```laji```-attribuutin arvo on jokin Kaavalajit-koodiston koodin [Asemakaava](http://uri.suomi.fi/codelist/rytj/RY_Kaavalaji/code/3) [Alakoodeista](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar), sekä näihin instansseihin Kaavatietomallin mukaisesti liittyvistä muiden luokkien instansseista.
{% include common/clause_end.html %}