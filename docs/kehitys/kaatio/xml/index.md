---
layout: "default"
description: ""
id: "skeema"
---
# XML-skeematiedostot

KAATIO-projektissa käytettävät kaavatiedon XML-skeemat kuvaavat [Kaavatietomallin version 1.1 loogisen tietomallin](/kaavatiedot/v1.1/) mukaisen fyysisen tietomallin [GML](https://www.ogc.org/standards/gml)-sovellusskeemana, jossa elementtien, attribuuttien ja assosiaatioiden nimet on [käännetty](../kaannos.html) englanninkielelle.

## Spatial Plan

* Versio 1.1: [spatialplan-1.1.xsd](spatialplan-1.1.xsd) 
* Versio 1.2: [spatialplan-1.2.xsd](spatialplan-1.2.xsd)

### Muutoshistoria

 * 1.2.1:
   * Removed PlanObject.type element, does not have any defined codelist in the model, so cannot be used in practice.
   * now uses absolute URL for importing localization and lud-core schemas
          
* 1.2.0:
   * Updated lud-core to version 1.2
   * Removed the optional elements PlanObjectType.order and PlanObjectType.recommendation to break the problematic bidirectional associations between PlanObjects and PlanOrder/PlanRecommendations. Bidirectional linking of PlanObjects and PlanOrders / PlanRecommendations would be a problem in practice: It would only be possible to link PlanOrderGroups in one direction (by the PlanOrderGroup.target attribute), so PlanObjects would only contain links to the directly linked PlanOrders. Instead design the APIs to enable fetching PlanOrders, PlanOrderGroups and PlanRecommendations by their "target" attibute value (first fetch PlanObjects, then fetch orders & recommandations on demand using the received PlanObject IDs) or altenatively return orders, groups and recommandations preemptively in the same LandUseFeatureCollection as the PlanObjects they are linked to.           
   * Removed the optional element SpatialPlan.planObject with the same justification as removing the PlanObjectType.order and PlanObjectType.recommendation: the bidirectional links between SpatialPlan and its PlanObjects are not necessary, the PlanObjects always have the mandatory link to their SpatialPlan which is enough for fetching the PlanObjects included in a particial SpatialPlan. This also allows for linking any future concrete realizations of AbstractPlanObject to a SpatialPlan.        
* 1.1.1 / 2.8.2022
   * Fixed the schemaLocation path of http://tietomallit.ymparisto.fi/ry-yhteiset/kielituki/xml/1.0 from localization.xsd -> localization-1.0.xsd
   * Fixed the schemaLocation path of http://tietomallit.ymparisto.fi/mkp-ydin/xml/1.1 from land-use-decision-core.xsd land-use-decision-core-1.1.xsd


## Land Use Decision Core

* Versio 1.1: [land-use-decision-core-1.1.xsd](land-use-decision-core-1.1.xsd) 
* Versio 1.2: [land-use-decision-core-1.2.xsd](land-use-decision-core-1.2.xsd)

### Muutoshistoria

* 1.2.1:
   * fixed substitutionGroup of LandUseFeatureCollection from gml:AbstractGML to gml:AbstractFeature (as required by GML 3.2 Standard)
   * now uses absolute URL for importing localization schema
* 1.2.0:
   * Added new LandUseFeatureCollection container type and element.
* 1.1.1:
   * Fixed the schemaLocation path of http://tietomallit.ymparisto.fi/ry-yhteiset/kielituki/xml/1.0 from localization.xsd -> localization-1.0.xsd
   * Added LandUseFeatureCollection as a generic container

## Localization

* Versio 1.0: [localization-1.0.xsd](localization-1.0.xsd) 