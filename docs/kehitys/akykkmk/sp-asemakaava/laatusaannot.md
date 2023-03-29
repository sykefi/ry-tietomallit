---
layout: "default"
description: ""
id: "laatusaannot"
status: "Ehdotus"
---
# Laatusäännöt

Nämä laatusäännöt laajentavat Kaavatietomallin [yleisiä laatusääntöjä](https://tietomallit.ymparisto.fi/kaavatiedot/v1.1/looginenmalli/laatusaannot.html).

## Lisätietojen käyttö aluemaisilla kaavakohteilla
{% include common/clause_start.html type="req" id="sp-ak/vaat-aluemainenkohde-lisatiedot" %}
Geometrialtaan aluemaiseen {% include common/moduleLink.html moduleId="kaavatiedot" path="dokumentaatio/#kaavakohde" title="Kaavakohde" %}-luokan objektiin tulee liittyä assosiaation ```määräys``` kautta vähintään yksi attribuutti ```lisätieto```, jonka arvona ```laji``` on [Kaavamääräyksen lisätiedonlaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto)-koodiston koodeista joko [Osa-alue](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/osaAlue) tai [Pääkäyttötarkoitus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/paakayttotarkoitus).
{% include common/clause_end.html %}