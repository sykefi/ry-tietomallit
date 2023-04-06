---
layout: "default"
description: ""
id: "rakentamisen-maara-sijoittaminen"
status: "Ehdotus"
---
# Kaavamääräyslajit - rakentamisen määrä ja sijoittaminen
{:.no_toc}

## Rakentamisen määrä
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/rakentamisenMaara>

Ryhmittelyotsikko, vain {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/elinkaarisaannot.html#elinkaari-vaat-alakoodi-maar" title="alakoodeja" %} käytetään.

1. 
{:toc}

### Sallittu kerrosala
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/sallittuKerrosala>

{% include common/clause_start.html type="req" id="sp-ak/vaat-sallittu-kerrosala-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} joka kertoo sallitun rakentamiseen kokonaismäärän kerrosneliömetreinä (```k-m2```) sen kaavakohteen aluella, johon kaavamääräys on liitetty. Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-sallittu-kerrosala-kaavakohde" %}
Asemakaavassa kaavamääräyslaji [Sallittu kerrosala](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/sallittuKerrosala) voidaan osoittaa vain {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#kaavakohde" title="Kaavakohteelle"%}, johon liittyy [KaavamääraysLaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays)-koodi [Rakennusala](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/rakennusala), tai joka kuvaa [Aluevarausta](../../aluevaraukset/index.md).
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-sallittu-kerrosala-lisatiedot" %}
```lisatieto```-attribuutin arvoina saa esiintyä nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#lisatieto" title="Lisatieto" %} jonka laji on [Käyttötarkoituksen osuus kerrosalasta](http://uri.suomi.fi/codelist/rytj/RY_Lisatiedonlaji_AK/code/01), jolla on täsmälleen kaksi arvoa:
*  Yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} jotka kertovat sallitun tiettyyn käyttötarkoitukseen kohdistettavan kerroalan määrän koko sallitusta kerrosalasta joko kerrosneliömetreinä (```k-m2```) tai prosentteina (```%```). Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta.
* Yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#koodiarvo" title="KoodiArvo" %}, joka viittaa [KaavamääraysLaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays)-koodiston aluevaraus-määrityshierarkiaan sisältyvään koodiin.
{% include common/clause_end.html %}

Mikäli sallittua rakentamisen määrää ei ole jaoteltu käyttötarkoituksittain, ei lisätietoja käytetä.

### Sallittu rakennustilavuus
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/sallittuRakennustilavuus>

{% include common/clause_start.html type="req" id="sp-ak/vaat-sallittu-rakennustilavuus-arvot" %}
```arvo```-attribuutin arvoina saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} jotka kertovat sallitun rakentamisen kokonaismäärän kuutiometreinä (```m3```) sen kaavakohteen aluella, johon kaavamääräys on liitetty. Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-sallittu-rakennustilavuus-kaavakohde" %}
Asemakaavassa kaavamääräyslaji [Sallittu rakennustilavuus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/sallittuRakennustilavuus) voidaan osoittaa vain {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#kaavakohde" title="Kaavakohteelle"%}, johon liittyy [KaavamääraysLaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays)-koodi [Rakennusala](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/rakennusala), tai joka kuvaa [Aluevarausta](../../aluevaraukset/index.md).
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-sallittu-rakennustilavuus-lisatiedot" %}
```lisatieto```-attribuutin arvoina saa esiintyä nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#lisatieto" title="Lisatieto" %} jonka laji on [Käyttötarkoituksen osuus kerrosalasta](http://uri.suomi.fi/codelist/rytj/RY_Lisatiedonlaji_AK/code/01), jolla on täsmälleen kaksi arvoa:
*  Yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} jotka kertovat sallitun tiettyyn käyttötarkoitukseen kohdistettavan rakennustilavuuden määrän koko sallitusta rakennustilavuudesta joko kuutiometreinä (```k-m3```) tai prosentteina (```%```). Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta.
* Yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#koodiarvo" title="KoodiArvo" %}, joka viittaa [KaavamääraysLaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays)-koodiston aluevaraus-määrityshierarkiaan sisältyvään koodiin.
{% include common/clause_end.html %}

Mikäli sallittua rakentamisen määrää ei ole jaoteltu käyttötarkoituksittain, ei lisätietoja käytetä.

### Tehokkuusluku
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/tehokkuusluku>

{% include common/clause_start.html type="req" id="sp-ak/vaat-tehokkuusluku-arvot" %}
```arvo```-attribuutin arvona saa esiintyä joko yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} jotka kertovat rakennustehokkuden, eli alueen rakennusten yhteenlasketun kerrosalan suhteessa alueen pinta-alaan, sen kaavakohteen aluella, johon kaavamääräys on liitetty. Ilmaistaan tehokkuuslukuna ```e```, yksikkönä ```k-m2/m2```. Muun tyyppiset arvot eivät ole sallittuja. Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta.
{% include common/clause_end.html %}

### Maanpäällinen kerrosluku
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/maanpaallinenKerrosluku>

{% include common/clause_start.html type="req" id="sp-ak/vaat-maanpaallinen-kerrosluku-arvot" %}
```arvo```-attribuutin arvona saa esiintyä joko yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} jotka kertovat rakennusten maanpäällisten kerrosten sallitun lukumäärän sen kaavakohteen aluella, johon kaavamääräys on liitetty. Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#integer" title="Integer" %}-rajapinta. Yksikköjä ei käytetä. Muun tyyppiset arvot eivät ole sallittuja. 
{% include common/clause_end.html %}

### Maanalainen kerrosluku
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/maanalainenKerrosluku>

{% include common/clause_start.html type="req" id="sp-ak/vaat-maanalainen-kerrosluku-arvot" %}
```arvo```-attribuutin arvona saa esiintyä joko yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} jotka kertovat rakennusten maanalaisten kerrosten sallitun lukumäärän sen kaavakohteen aluella, johon kaavamääräys on liitetty. Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#integer" title="Integer" %}-rajapinta. Yksikköjä ei käytetä. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

### Kellarin sallittu kerrosalaosuus
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/kellarinSallittuOsuusKerrosalasta>

{% include common/clause_start.html type="req" id="sp-ak/vaat-kellarin-sallittu-kerrosalaosuus-arvot" %}
```arvo```-attribuutin arvona saa esiintyä joko yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} jotka kertovat kuinka suuren osan kunkin rakennuksen suurimman kerroksen alasta saa kellarikerroksessa käyttää kerrosalaan luettavaksi tilaksi sen kaavakohteen aluella, johon kaavamääräys on liitetty. Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta. Ilmaistaan prosentteina (```%```). Muun tyyppiset arvot eivät ole sallittuja. 
{% include common/clause_end.html %}

{% include common/tip.html content="Murtolukuna ilmaistun osuuden voi ilmaista likimääräisesti myös arvovälinä, esim. ```1/3``` olisi ```33-34%```" %}

### Ullakon sallittu kerrosalaosuus
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/ullakonSallittuOsuusKerrosalasta>

{% include common/clause_start.html type="req" id="sp-ak/vaat-ullakon-sallittu-kerrosalaosuus-arvot" %}
```arvo```-attribuutin arvona saa esiintyä joko yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} jotka kertovat kuinka suuren osan kunkin rakennuksen suurimman kerroksen alasta saa ullakkokerroksessa käyttää kerrosalaan luettavaksi tilaksi sen kaavakohteen aluella, johon kaavamääräys on liitetty. Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta. Ilmaistaan prosentteina (```%```). Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

{% include common/tip.html content="Murtolukuna ilmaistun osuuden voi ilmaista likimääräisesti myös arvovälinä, esim. ```1/3``` olisi ```33-34%```" %}

### Rakennuspaikkojen määrä
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/rakennuspaikkojenMaara>

{% include common/clause_start.html type="req" id="sp-ak/vaat-rakennuspaikkojen-maara-arvot" %}
```arvo```-attribuutin arvona saa esiintyä yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} joka kertoo sallitun rakennuspaikkojen enimmäismäärän sen kaavakohteen aluella, johon kaavamääräys on liitetty. Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#integer" title="Integer" %}-rajapinta. Yksikköä ei käytetä. Muun tyyppiset arvot eivät ole sallittuja.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-rakennuspaikkojen-maara-lisatiedot" %}
```lisatieto```-attribuutin arvoina saa esiintyä nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#lisatieto" title="Lisatieto" %} jonka laji on [Käyttötarkoituskohdistus](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/kayttotarkoituskohdistus), jolla on täsmälleen yksi ```arvo``` lajia {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#koodiarvo" title="KoodiArvo" %} joka viittaa johonkin [Rakennusluokitus 2018](http://uri.suomi.fi/codelist/jhs/rakennus_1_20180712)-koodiston koodiin. Muun tyyppiset arvot eivät ole sallittuja.

Mikäli vähintään yksi lisätieto on annettu, koskee rakennuspaikkojen lukumäärä vain lisätietojen avulla rajattuja rakennustyyppejä.
{% include common/clause_end.html %}

{% include common/note.html content="Käytetään tavallisesti vain ranta-asemakaavoissa" %}

### Lisärakennusoikeuden määrä
**Koodi**: <http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays/code/lisarakennusoikeudenMaara>

{% include common/clause_start.html type="req" id="sp-ak/vaat-lisarakennusoikeus-arvot" %}
```arvo```-attribuutin mahdolliset arvot ovat seuraavat:
* Yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} joka kertoo sallitun lisärakentamisen kokonaismäärän joko kerrosneliömetreinä (```k-m2```) tai kuutiometreinä (```m3```) sen kaavakohteen aluella, johon kaavamääräys on liitetty. Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta.
* Nolla tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#tekstiarvo" title="TekstiArvo" %} (yksi kullakin kielellä), joka täydentää kaavamääräystietoa.
{% include common/clause_end.html %}

{% include common/clause_start.html type="req" id="sp-ak/vaat-lisarakennusoikeus-lisatiedot" %}
```lisatieto```-attribuutin arvoina saa esiintyä yksi tai useampi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#lisatieto" title="Lisatieto" %} jonka laji on [Käyttötarkoituksen osuus kerrosalasta](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarayksen_Lisatieto/code/kayttotarkoituksenOsuusKerrosalasta), jolla on täsmälleen kaksi arvoa:
*  Yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvo" title="NumeerinenArvo" %} tai yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#numeerinenarvovali" title="NumeerinenArvovali" %} jotka kertovat sallitun tiettyyn käyttötarkoitukseen kohdistettavan kerroalan määrän koko sallitusta kerrosalasta joko kerrosneliömetreinä (```k-m2```), kuutioina (```m3```) tai prosentteina (```%```). Numeerisen arvon tai arvovälin minimi- ja maksimiarvojen on toteutettava {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#real" title="Real" %}-rajapinta.
* Yksi {% include common/moduleLink.html moduleId="kaavatiedot" path="looginenmalli/dokumentaatio/#koodiarvo" title="KoodiArvo" %}, joka viittaa [KaavamääraysLaji](http://uri.suomi.fi/codelist/rytj/RY_Kaavamaarays)-koodiston aluevaraus-määrityshierarkiaan sisältyvään koodiin.
{% include common/clause_end.html %}
