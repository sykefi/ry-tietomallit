---
layout: "default"
description: ""
id: "laatusaannot"
status: "Ehdotus"
---
# Laatusäännöt
Nämä laatusäännöt laajentavat Kaavatietomallin [yleisiä laatusääntöjä](../../looginenmalli/laatusaannot.html).

## Yleiset säännöt

{% include common/clause_start.html type="req" id="sp-yk/arvot" %}
Ellei tarkemmin ole määritetty, ```arvo```-attribuutin arvoina saa esiintyä nolla tai useampi [Tekstiarvo](https://tietomallit.suomi.fi/model/rytj-kaava/Tekstiarvo/) (yksi kullakin kielellä), joka täydentää kaavamääräystietoa. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

{% include common/clause_start.html type="rec" id="sp-yk/suos-asiakirja" %}
Mikäli kaavakohteeseen liittyen on laadittu jokin suunnitelma, selvitys, raportti tai muu asiakirja, on suositeltavaa linkittää se kaavamääräykseen ```liiteAsiakirja```-assosiaation avulla.
{% include common/clause_end.html %}

{% include common/clause_start.html type="rec" id="sp-yk/suos-liittyvakohde" %}
[Kaavakohde](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/) voidaan linkittää toisiin [Kaavakohteisiin](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/) assosiaation [Liittyvä kohde](https://tietomallit.suomi.fi/model/rytj-kaava/Kaavakohde/6e080c6a-bb00-4d7f-b095-215f7c902e19) arvojen avulla.
{% include common/clause_end.html %}