# Advanced networking - VirtualWAN

## Intro
Tento hack vás seznámí s konceptem Azure VirtualWAN. Začnete s jednoduchou konfigurací dvou hubů a poté ji bude rozšiřovat o připojení k on-premises, upravovat routing kvůli segmentaci a nakonec ji zabezpečíte pomocí Azure Firewallu. Jako poslední přidanou Challenge si poté vyzkoušíte publikaci webové aplikace na Azure FrontDooru. 

## Co se naučíte
Následující hack challenges poktrývají tyto oblasti:
- Základní konektivita ve VirtualWAN
- Připojení poboček (on-premises) včetně použití BGP
- Pokročilý routing
- Zabezpečení pomocí Azure Firewallu
- Bezpečná publikace aplikací pomocí Azure FrontDoor


## Challenges

- Challenge 1: **[Simple Virtual WAN](./Student/01_simple_vwan.md)**
    - Nasaďte jednoduchý VWAN se dvěma huby

- Challenge 2: **[Branch connectivity](./Student/02_branch_connectivity.md)**
    - Připojte HUBy k on-premises

- Challenge 3: **[Isolated VNets](./Student/03_isolated_vnets.md)**
    - Použijte custom routing pro segmentaci

- Challenge 4: **[Secured Virtual HUB](./Student/04_secured_hub.md)**
    - Nasaďte Azure Firewall a zabezpečete komunikaci

- Challenge 5: **[Secured publishing](./Student/05_secured_publishing.md)**
    - Nasaďte Azure FrontDoor a bezpečně publikujte webové stránky


