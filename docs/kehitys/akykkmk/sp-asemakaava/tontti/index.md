---
layout: "default"
description: ""
id: "tonttijako"
status: "Ehdotus"
---
# Kaavamääräykset - tontti

## Tontti
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/tontti>
Ryhmittelyotsikko, vain [Alakoodeja](https://tietomallit.ymparisto.fi/kaavatiedot/dev/looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar) käytetään.

{% include common/clause_start.html type="req" id="sp-ak/vaat-tontti-liittyvakohde" %}
Kaavakohteeseen, johon liittyy kaavamääräyslaji-koodi [Sitovan tonttijaon mukainen tontti](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/sitovanTonttijaonMukainenTontti>)(http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/sitovanTonttijaonMukainenTontti) tai [Ohjeellinen tontti](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/ohjeellinenTontti>), tulee '''Liittyvä kohde''' -assosiaation avulla linkittää se (Aluevaraus)[/../../aluevaraukset/index.md], jonka sisälle tontti spatiaalisesti sijoittuu.
{% include common/clause_end.html %}

### Sitovan tonttijaon mukainen tontti
{% include common/clause_start.html type="req" id="sp-ak/vaat-sitova-tonttijako" %}
Sitovan tonttijaon mukainen tontti kuvataan siten, että Kaavakohteeseen liittyy kaavamääräyslaji-koodiston koodi [Sitovan tonttijaon mukainen tontti](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/sitovanTonttijaonMukainenTontti>).
{% include common/clause_end.html %}

### Ohjeellinen tontti
{% include common/clause_start.html type="req" id="sp-ak/vaat-ohjeellinen-tontti" %}
Ohjeellinen tontti kuvataan siten, että Kaavakohteeseen liittyy kaavamääräyslaji-koodiston koodi [Ohjeellinen tontti](<http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayslaji/code/ohjeellinenTontti>).
{% include common/clause_end.html %}