# Challenge 4: 

[< Previous Challenge](./04_secured_hub.md) - **[Home](../README.md)** 

## Intro

V tého challenge si vyzkoušíte zabezpečit komunikaci ve virtualWAN / hubech pomocí Azure Firewall


## Popis 
*   Vytvořte jednoduchou webovou aplikaci na WeApp service (statické „Hello World!“ stačí)
*   Zakažte přístup na WebApp z internetu a zpřístupněte ji jen v rámci interní sítě.
*   Nasaďte Azure FrontDoor a vypublikujte stránku z WebAppky.
*   (volitelné) Vypublikujte na FrontDoor webovou stránku běžící na VM z Challenge 4 taktéž tak, aby komunikace mezi FrontDoot a VM nikde nešla otevřeným internetem.

Ukázka topologie:

![topology](../images/vwan04.png)

## Success Criteria

- Přistupte z internetu na stánku hostovanou na WebApp. Dohledejte přístup v logu FrontDooru.
- (volitelné) Přistupte z intenetu na stánku hostovanou na VM. Dohledejte přístup v logu FrontDooru.

## Zdroje pro studium

- [What is Azure Front Door?](https://learn.microsoft.com/en-us/azure/frontdoor/front-door-overview)

- [Use private endpoints for Azure App Service apps](https://learn.microsoft.com/en-us/azure/app-service/overview-private-endpoint)
- [Quickstart: Create an Azure Front Door using Azure portal](https://learn.microsoft.com/en-us/azure/frontdoor/create-front-door-portal?tabs=quick)
- [Connect Azure Front Door Premium to an App Service (Web App) origin with Private Link](https://learn.microsoft.com/en-us/azure/frontdoor/standard-premium/how-to-enable-private-link-web-app)

