---
layout: "default"
description: ""
id: "johdanto"
status: "Ehdotus"
---
# Kaavatietomallin soveltamisprofiili yleiskaava-aineistoille
{:.no_toc}

Tämän dokumentin vaatimukset ja suositukset muodostavat Kaavatietomallin loogisen tietomallin soveltamisprofiilin yleiskaava-aineistoille. Soveltamisprofiili kuvaa ne rajoitukset ja lisävaatimukset, joita tulee noudattaa Kaavatietomallin {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/uml/doc/" title="UML-kielisen kuvauksen" %} ja sen {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/" title="sanallisen dokumentaation" %} soveltamisessa yleiskaavojen tietoaineistojen kuvaamiseen.

<!--
Tämän muodollisen dokumentin tietoja täydentää [Yleiskaavan kaavamääräysopas](https://sykefi.github.io/kaavamaaraysoppaat/yleiskaava/), joka sisältää käytännön esimerkkejä Kaavatietomallin soveltamisesta yleiskaavoituksen kaavoitusratkaisuihin.-->

{% include common/clause_start.html type="req" id="sp-yk/vaat-yleiskaava-aineisto-maar" %}
Kaavatietomallin mukainen yleiskaava-aineisto koostuu {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#kaava" title="Kaava" %}-luokan instansseista, joiden ```laji```-attribuutin arvo on jokin {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#kaavalaji" title="Kaavalajit" %}-koodiston koodin [Yleiskaava](http://uri.suomi.fi/codelist/rytj/RY_Kaavalaji/code/2) {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar" title="alakoodeista" %}, sekä näihin instansseihin Kaavatietomallin mukaisesti liittyvistä muiden luokkien instansseista.
{% include common/clause_end.html %}