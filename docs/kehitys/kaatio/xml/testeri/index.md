---
layout: "swagger-ui"
description: ""
id: "testeri"
openapi-url: "https://kaatio.spatineo-devops.com/openapi.json"
---
# Kaava-XML:n simuloitu tallennuspalvelu

Tässä kuvattu rajapinta simuloi KAATIO-projektissa määritellyn XML-muotoisen kaavatiedon tallennusrajapintaa. Rajapinta on laadittu KAATIO-hankkeen aikaista ohjelmistojen testausta varten, eikä se ole tarkoitettu operatiiviseen käyttöön. Rajapinta ottaa vastaan XML-muotoisen kaavan paketoituna ```LandUseFeatureCollection```-juurielementin sisään, kuten kuvattu [Esimerkit-sivulla](../esimerkit/). Lähetettäviä tiedostoja ei tallenneta mihinkään.

Palvelun on toteuttanut Spatineo Oy, ja se on käytettävissä KAATIO-hankkeen ajan. [Toteutus](https://github.com/spatineo/kaatio-planvalidator) on julkaistu avoimena lähdekoodina (GPL v3.0). OpenAPI-rajapinta löytyy osoitteesta [https://kaatio.spatineo-devops.com/openapi.json](https://kaatio.spatineo-devops.com/openapi.json) ja Swagger-UI-dokumentaatio upotettuna alta tai osoitteesta [https://kaatio.spatineo-devops.com/docs](https://kaatio.spatineo-devops.com/docs).
