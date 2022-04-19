---
layout: "default"
title: "Käännös suomesta englannin kielelle"
description: "Kaavatietomallin luokkien ja ominaisuuksien englanninkieliset nimet"
id: "kaannos"
---
# Kaavatietomallin luokkien ja ominaisuuksien englanninkieliset nimet

Hankkeessa tuottaavan XML-skeeman elementtien, attribuuttien ja assosiaatioiden nimet päätettiin tuottaa englanninkielellä, jotta skeeman kuvaus olisi tuotettu vain yhdellä kielellä. Tämä helpottaa tiedon teknistä käsittelyä tietojärjestelmissä.

Alla on kuvattu KAATIO-hankkeessa tuotetuissa XML-skeemoissa käytetyt Kaavatietomallin luokkien ja niiden ominaisuuksien suomenkielisiä nimiä vastaavat englanninkieliset nimet. Huomaa, että attribuutit ```nimi``` ja ```kuvaus``` on käännetty nimiksi ```loc_name``` ja ```loc_description```,  jotta ne eivät aiheuttaisi konflikteja GML:n AbstractFeatureType:n ```name```- ja ```description```-elementtien kanssa. Nämä GML:n elementit eivät tue monikielistä sisältöä, joka on Kaavatietomallissa vaatimuksena. 


## MKP-ydin -paketti

| Luokka                     | Ominaisuus                      | Name                           |
|----------------------------|---------------------------------|--------------------------------|
| AbstraktiVersioituObjekti  | | AbstractVersionedObject |
| | paikallinenTunnus        | versionIdentifier |
| | nimiavaruus              | namespace
| | viittausTunnus           | gml:identifier |
| | identiteettiTunnus       | objectIdentifier |
| | tuottajakohtainenTunnus  | producerSpecificIdentifier |
| | viimeisinMuutos          | latestChange |
| | tallennusAika            | storageTime  |
| | korvaaObjektin           | replacesObject |
| | korvattuObjektilla       | replacedByObject |
| AbstraktiMaankayttoasia    | | AbstractLandUseMatter   |
| | nimi                     | loc_name |
| | kuvaus                   | loc_description |
| | aluerajaus               | boundary |
| | oikeusvaikutteisuus      | legalEffectiveness |
| | metatietokuvaus          | metadata |
| | voimassaoloAika          | validityTime |
| | asianLiite               | annex |
| | koskeeHallinnollistaAluetta | administrativeArea |
| | vastuullinenOrganisaatio | responsibleOrganisation |
| | hyodynnettyAineisto      | usedInputDataset |
| | liittyvaAsia             | relatedMatter |
| Asiakirja                  | | Document |
| | asiakirjanTunnus         | documentIdentifier |
| | nimi                     | loc_name |
| | laji                     | type |
| | lisatietolinkki          | additionalInformationLink |
| | metatietokuvaus          | metadata |
| | liittyvaAsiakirja        | relatedDocument |
| Lahtotietoaineisto         | | InputDataset |
| | aineistoTunnus           | datasetIdentifier |
| | nimi                     | loc_name |
| | laji                     | type |
| | aluerajaus               | boundary |
| | lisatietolinkki          | additionalInformationLink |
| | metatietokuvaus          | metadata |
| Abstraktitapahtuma         | | AbstractEvent |
| | nimi                     | loc_name |
| | kuvaus                   | loc_description |
| | tapahtumaAika            | eventTime |
| | sijainti                 | location |
| | lisatietolinkki          | additionalInformationLink |
| | peruttu                  | cancelled |
| | liittyvaAsia             | relatedMatter |
| | liittyvaAsiakirja        | relatedDocument |
| Kasittelytapahtuma         | | HandlingEvent |
| | laji                     | type |
| | kasittelija              | handler |
| Vuorovaikutustapahtuma     | | InteractionEvent |
| | laji                     | type

## Kaavatiedot-paketti

| Luokka                     | Ominaisuus                      | Name                           |
|----------------------------|---------------------------------|--------------------------------|
| Kaava | | SpatialPlan
| | laji | type
| | kaavaTunnus | planIdentifier
| | elinkaaritila | lifecycleStatus
| | kumoamistieto | cancellationInfo
| | maanalaisuus | groundRelativePosition
| | vireilletuloAika | initiationTime
| | hyvaksymisAika | approvalTime
| | digitaalinenAlkupera | digitalOrigin
| | yleismaarays | generalOrder
| | laatija | planner
| | kaavakohde | planObject
| | yleissuositus | generalRecommendation
| | osallistumisJaArviointisuunnitelma | participationAndEvaluationPlan
| AbstraktiKaavakohde | | AbstractPlanObject
| | nimi | loc_name
| | geometria | geometry
| | pystysuuntainenRajaus | verticalLimit
| | kaava | spatialPlan
| | liittyvaKohde | relatedObject
| AbstraktiTietoyksikko | | AbstractInformationUnit
| | nimi | loc_name
| | arvo | value
| | kaava | spatialPlan
| | kohdistus | target
| Kaavakohde | | PlanObject
| | laji | type
| | sijainninSitovuus | bindingnessOfLocation
| | liittyvanLahtotietokohteenTunnus | relatedInputDataObjectIdentifier
| | ymparistomuutoksenLaji | environmentalChangeType
| | maanalaisuus | groundRelativePosition
| | maarays | order
| | suositus | recommendation
| Kaavamaarays | | PlanOrder
| | laji | type
| | elinkaariTila | lifecycleStatus
| | teema | theme
| | lisatieto | supplementaryInfo
| | voimassaoloAika | validityTime
| | liittyvaAsiakirja | relatedDocument
| Kaavamaaraysryhma | | PlanOrderGroup
| | ryhmanumero | groupNumber
| | jasen | member
| Kaavasuositus | | PlanRecommendation
| | elinkaaritila | lifecycleStatus
| | teema | theme
| | voimassaoloAika | validityTime
| | liittyvaAsiakirja | relatedDocument
| Kaavayksikko | | PlanUnit
| | kiinteisto | property
| Muodostajakiinteisto | | FormingProperty
| | kiinteistoTunnus | propertyIdentifier
| | sisaltyyKokonaan | includedCompletely
| | sisaltyvaPintaAla | includedArea
| Lisatieto | | SupplementaryInformation
| KaavanKumoamistieto | | CancellationInformation
| | kumottavanKaavanTunnus | cancelledPlanIdentifier
| | kumoaaKaavanKokonaan | cancelsEntirePlan
| | kumottavaKaavanAlue | areaToCancel
| | kumottavanMaarayksenTunnus | cancelledPlanOrderIdentifier
| | kumottavanSuosituksenTunnus | cancelledPlanRecommendationIdentifier
| KaavanLaatija | | Planner
| | nimi | personName
| | nimike | professionTitle
| | rooli | role
| OsallistumisJaArviointisuunnitelma | | ParticipationAndEvaluationPlan
| | asiakirja | document 
| Kaavaselostus | | SpatialPlanCommentary
| | asiakirja | document
| AbstraktiArvo | | AbstractValue |
| TekstiArvo | | TextValue
| | arvo | value
| | syntaksi | syntax
| TunnusArvo | | IdentifierValue
| | arvo | value
| | rekisterinTunnus | registryIdentifier
| | rekisterinNimi | registryName | 
| Aikavaliarvo | | TimePeriodValue
| | arvo | value
| Ajanhetkiarvo | | TimeInstantValue
| | arvo | value
| GeometriaArvo | | GeometryValue
| | arvo | value
| Koodiarvo | | CodeValue
| | arvo | value
| | koodistonTunnus | codelistIdentifier
| | otsikko | label
| NumeerinenArvo | | NumericValue
| | arvo | value
| | mittayksikko | unitOfMeasure
| NumeerinenArvovali | | NumericRange
| | minimiarvo | minimumValue
| | maksimiarvo | maximumValue
| | mittayksikko | unitOfMeasure
| Korkeuspiste | | ElevationPoint
| | referenssipiste | referencePoint
| Korkeusvali | | ElevationRange
| | referenssipiste | referencePoint
