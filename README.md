# Rakennetun ympäristön tietomallit
Ryhti-hankkeen piiriin kuuluvien rakennetun ympäristön tietomallien yhteinen dokumentaatiosivusto. Sivustoa hallinnoi [Suomen ympäristökeskus](https://www.syke.fi/), ja tietomallien muutoshallintaprosessista vastaa [ympäristöministeriö](https://ym.fi/).

Dokumentaatio on koottu pääosin tämän repon [wikiin](../../wiki), ks. muun muassa sivut
* [Sivuston rakenne](../../wiki/Sivuston-rakenne)
* [Tietomallien kehittäminen ja ylläpito](../../wiki/Tietomallien-kehitt%C3%A4minen-ja-yll%C3%A4pito)
* [Modulien konfigurointi](../../wiki/Modulien-konfigurointi)
* [Sisältömakrot](../../wiki/Sis%C3%A4lt%C3%B6makrot)

## Linkitetyt repot

RY-tietomallit sivusto on rakennettu siten, että sen sisältö koostuu pääosin toisista git-repoista  noudettavista lähdekooditiedostoista. Linkitys ry-tietomallit-reposta toisiin git-repoihin on toteutettu [git submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules)-mekanismilla. Näin voidaan esittää samalla sivustolla useamman kuin yhden tietomallin version kuvaus linkittämällä ko. tietomallirepon eri release-tagien mukaisiin committeihin, ks. lisää wiki-sivu [Tietomallien kehittäminen ja ylläpito](../../wiki/Tietomallien-kehitt%C3%A4minen-ja-yll%C3%A4pito).

Sivulle voidaan linkittää mitä tahansa julkisia git-repoja, ja GitHub Pages -osaa noutaa ko. linkkien asetetun commitin mukaiset sisällöt automaattisesti sivuston buildauksen yhteydessä. **Huom**: Mikäli moduli ei ole julkaistu GitHub:issa, sen sivumetatieto-laatikon muutostietojen esittäminen ei onnistu, sillä sen tiedot haetaan JavaScriptillä käyttäen [GitHub REST API](https://docs.github.com/en/rest)a.

| Nimi                       | versio | hakemistopolku          | linkitetty git-repo          | tagi / haara / commit  | huom     |
-----------------------------|--------|-------------------------|------------------------------|------------------------|----------|
| RY-yhteiset komponentit    | dev    | [docs/ry-yhteiset/](../../tree/main/docs/ry-yhteiset/)dev | [github.com/sykefi/ry-yhteiset](https://github.com/sykefi/ry-yhteiset) | develop | |
| Kaavatiedot                | 1.0.1  | [docs/kaavatiedot/](../../tree/main/docs/kaavatiedot/)v1.0 | [github.com/ilkkarinne/kaavatietomalli](https://github.com/ilkkarinne/kaavatietomalli) | v1.0.1 | TODO: siirto ilkkarinne -> sykefi |
| Asemakaavan soveltamisprofiili | 1.0 | [docs/kaavatiedot/soveltamisprofiili/asemakaava/](../../tree/main/docs/kaavatiedot/soveltamisprofiili/asemakaava/)v1.0 | [github.com/sykefi/sp-asemakaava](https://github.com/sykefi/sp-asemakaava) |  |  |
| Kaavatiedot                | dev    | [docs/kaavatiedot/](../../tree/main/docs/kaavatiedot/)dev | [github.com/ilkkarinne/kaavatietomalli](https://github.com/ilkkarinne/kaavatietomalli) | develop | TODO: siirto ilkkarinne -> sykefi |
| Tonttijakosuunnitelma      | 1.0    | [docs/tonttijakosuunnitelma/](../../tree/main/docs/tonttijakosuunnitelma/)v1.0 | [github.com/ilkkarinne/Tonttijakosuunnitelman-tietomalli](https://github.com/ilkkarinne/Tonttijakosuunnitelman-tietomalli) |  | TODO: siirto ilkkarinne -> sykefi |
| Tonttijakosuunnitelma      | dev    | [docs/tonttijakosuunnitelma/](../../tree/main/docs/tonttijakosuunnitelma/)dev | [github.com/ilkkarinne/Tonttijakosuunnitelman-tietomalli](https://github.com/ilkkarinne/Tonttijakosuunnitelman-tietomalli) |  | TODO: siirto ilkkarinne -> sykefi |
| Rakennuskohteet    | dev    | [docs/rakennuskohteet/](../../tree/main/docs/rakennuskohteet/)dev | [github.com/sykefi/rakennuskohteet](https://github.com/sykefi/rakennuskohteet) | develop |  |
| Rakentamista koskevat lupapäätökset    | dev    | [docs/rakentamisenluvat/](../../tree/main/docs/rakentamisenluvat/)dev | [github.com/ilkkarinne/rakentamisenluvat](https://github.com/ilkkarinne/rakentamisenluvat) | develop | TODO: siirto ilkkarinne -> sykefi |
| Yhteiset Sisältömakrot | | [docs/_includes/](../../tree/main/docs/_includes/)common | [github.com/sykefi/rytm-jekyll-includes](https://github.com/sykefi/rytm-jekyll-includes) | main | 

Kulloinkin linkatut git submodulet ja niiden tilan saa tulostettua (linux-tyyppisessä komentoriviympäristössä) seuraavalla loitsulla:
```sh
$ git submodule foreach --quiet 'printf "\n$sm_path: linked to " && git remote get-url origin && printf "at " && git describe --tags --first-parent --dirty --always'

docs/_includes/common: linked to https://github.com/ilkkarinne/rytm-jekyll-includes.git
at 28f784a-dirty

docs/kaavatiedot/dev: linked to https://github.com/ilkkarinne/kaavatietomalli-1.git
at v1.0-43-g5c44c08-dirty

docs/kaavatiedot/soveltamisprofiili/asemakaava/v1.0: linked to https://github.com/ilkkarinne/sp-asemakaava.git
at 5bce9c1

docs/kaavatiedot/v1.0: linked to https://github.com/ilkkarinne/kaavatietomalli-1.git
at 1.0.1

docs/rakennuskohteet/dev: linked to https://github.com/ilkkarinne/rakennuskohteet.git
at b68f2f9

docs/rakentamisenluvat/dev: linked to https://github.com/ilkkarinne/rakentamisenluvat.git
at 95f8e49

docs/ry-yhteiset/dev: linked to https://github.com/ilkkarinne/ry-yhteiset.git
at 04c89ea

docs/tonttijakosuunnitelma/dev: linked to https://github.com/ilkkarinne/Tonttijakosuunnitelman-tietomalli.git
at v1.0-256-g405e7f2

docs/tonttijakosuunnitelma/v1.0: linked to https://github.com/ilkkarinne/Tonttijakosuunnitelman-tietomalli.git
at 1.0.0
```

## Suunnitellut tietomallit

Seuraavassa listassa on lueteltu [rakennetun ympäristön yhteentoimivuustyössä](https://ym.fi/yhteentoimivuus) tunnistettuja tietomalleja, jotka on tarkoitus tuoda sivustolle omina moduleinaan tulevaisuudessa:

* Useita sovellusalueita koskevat tietomallit
   * RYTJ-soveltamisprofiili (yhdistelmä RYTJ:ssä toteutettavista loogisista ry-tietomalleista)
   * Rakennetun ympäristön yläontologia
* Alueiden käytön suunnittelu
   * Yleisten alueiden suunnitelmat
   * Kaavatietomallin soveltamisprofiili maakuntakaavoille
   * Merialuesuunnitelma
   * Kaupunkiseutusuunnitelma
* Rakentaminen
   * Maankäytön rajoitukset
   * Rakennusjärjestys
* Kulttuuriympäristö
   * Rakennettu kulttuuriympäristö
   * Rakennusperinnön ja arkeologisen kulttuuriperinnön suojelu

## Paikallinen kehitysympäristö

Sivuston kehittämisessä on huomattavasti hyötyä paikallisesta kehitysympäristöstä, jossa tietoihin tehtävät muutokset saa näkyviin esikatseluna ilman tietojen viemistä GitHub Pages - mekanismilla julkaistulle [Rakennetun ympäristön tietomallit](https://tietomallit.ymparisto.fi)-sivustolle.

Mikäli valmistelet uutta versiota kehitettävästä tietomallista tai uutta sivustolle tuotavaa tietomallia, noudata [sisältörepojen kehittämis- ja ylläpito-ohjetta](https://github.com/sykefi/ry-tietomallit/wiki/Tietomallien-kehitt%C3%A4minen-ja-yll%C3%A4pito) tämän repon wikissä.

GitHub Pages -sivugenerointia voi simuloida varsin uskottavasti paikallisella työasemalla ajaen [Docker GitHub Pages](https://github.com/Starefossen/docker-github-pages) -Docker-konttia:

1. [Asenna Docker Engine](https://docs.docker.com/engine/install/), ja [komentorivi-git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git), mikäli ei jo asennettu.
1. Tee juurihakemisto koneelle kloonatuille git-repoille ja siirry sinne
1. Tee [oma fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) git-reposta [sykefi/ry-tietomallit](https://github.com/sykefi/ry-tietomallit)
1. [Kloonaa](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) forkkisi paikalliselle työasemalle:
   ```sh
   $ git clone https://github.com/<oma-gh-tunnus>/ry-tietomallit.git
   ```
1. Siirry hakemistoon ```ry-tietomallit/docs```
1. Käynnistä docker-github-pages -kontti porttiin 4000:
   ```sh
   $ docker run -it --rm -v "$PWD":/usr/src/app -p "4000:4000" starefossen/github-pages
   ```
1. Sivusto tulee buildauksen jälkeen näkyviin osoitteeseen http://localhost:4000/ 
   Mikäli tulee virheilmoitus "docker: Cannot connect to the Docker daemon...", varmista, että asentamasi Docker Engine on käynnissä taustalla.
1. Muokkaa sivuston tietoja tarpeellisilta osin, varmista, että kaikki näyttää hyvältä osoitteesta http://localhost:4000/
1. On hyvä käytäntö olla tekemättä muutos-committeja suoraan linkitettyjen submodulien sisältöihin, ja tyypillisesti tietomallien kehittäjillä ei ole siihen oikeuksiakaan. Voit toki kokeilla muutoksia paikallisesti, kopioida ne  sitten muutoksiksi linkitettyihin repoihin, commitoida ja pushata, palauttaa muutokset ry-tietomallit -repon linkitetyissä hakemistoissa ```git restore```-komennolla, ja tehdä pull ry-tietomallit -repon paikallisen klooniin ko. modulin hakemistossa.
