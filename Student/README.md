**Prerekvizity**

Azure subscripce s právy contributora

**Challenges 1 - Simple VirtualWAN**

*   Postavte VirtualWAN, který obsahuje dva HUBy, každý v jiném regionu.
*   Do každého hubu připojte 2 spoke VNETy
*   V každé spoke VNET vytvořte minimálně jeden subnet a do něj nasaďte jeden virtuální sever
*   Vyzkoušejte komunikaci mezi všemi VM (ping, ssh/rdp)

**Challenge 2 - VPN na on-prem**      

*   Propojte oba huby s On-Premises – každý zvlášť s jednou on-premises VPN GW (simulující on-premises v daném regionu)
*   Site2Site VPN spojení musí být na straně Azure redundantní
*   Pro distribuci rout použijte BGP
*   Potvrďte, že funguje VPN spojení s on-premises – zkuste si otevřít webovou stránku hostovanou na serveru v každé on-premises lokalitě z každé VM ve spoke VNETách

**Challenge 3 - Izolované VNETy**

*   Vytvořte další spoke VNETy tak, aby ke každému hubu byly připojeny přesně 4.
*   Rozdělte spoke VNETy u každého hubu dle role tak, že jedna bude sloužit pro DEV prosředí, dvě pro PROD a poslední bude obsahovat SHARED zdroje.
*   Síťově toto rozdělení znamená, že DEV může komunikovat se SHARED, ale ne s PROD. PROD může komunikovat se SHARED, ale ne s DEV. Toto platí i napříč huby, tj. PROD VNET z jednoho hubu může komunikovat s jinou PROD VNET z jiného hubu, atd.. Všechny spoke VNET nadále mohou komunikovat s on-premises.

**Challenge 4 - Secured Virtual HUB**

*   Přidejte do hubů Azure Firewal.
*   Zajistěte, aby veškerá komunikace do internetu procházela firewalem.
*   Na jednom z VM v PROD spoke VNET spusťte webový server a vypublikujte primitivní WEB stránku (statické „Hello World!“ stačí)
*   Zpřístupněte tuto stránku z internetu.

**Challenge 5 - Front Door**

*   Vytvořte jednoduchou webovou aplikaci na WeApp service (statické „Hello World!“ stačí)
*   Zakažte přístup na WebApp z internetu a zpřístupněte ji jen v rámci interní sítě.
*   Nasaďte Azure FrontDoor a vypublikujte stránku z WebAppky.
*   (optional) Vypublikujte na FrontDoor webovou stránku běžící na VM z Challenge 4 taktéž tak, aby komunikace mezi FrontDoot a VM nikde nešla otevřeným internetem.

