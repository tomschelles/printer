# Intune Printer Installatie Tool

Deze repository bevat een webapplicatie en bijbehorende scripts om
printerinstallaties via Microsoft Intune te vereenvoudigen en te
standaardiseren.

## Structuur

    .
    ├── app/
    │   ├── index.html
    │   ├── web.config
    │   └── 1.0.0.1_Install-Printer.intunewin (voorbeeldbestand)
    ├── drivers/
    │   ├── Canon/
    │   ├── Kyocera/
    │   └── Ricoh/
    ├── Install-Printer.ps1
    ├── Remove-Printer.ps1
    └── README.md

## Onderdelen

### /app

Bevat de webinterface.

-   index.html\
    Hier configureer je de applicatie voor je eigen omgeving. Pas hier
    de printerinstellingen, paden en variabelen aan.

-   web.config\
    Configuratiebestand voor hosting (bijv. IIS).

-   .intunewin bestand\
    Voorbeeldpakket voor gebruik in Microsoft Intune.\
    Let op: moet aangepast worden per omgeving.

### /drivers

Bevat de printerdrivers, gestructureerd per fabrikant.

### Scripts

-   Install-Printer.ps1\
-   Remove-Printer.ps1

## Gebruik

1.  Pas app/index.html aan
2.  Plaats drivers in /drivers
3.  Pas scripts aan indien nodig
4.  Maak een nieuwe intunewin
5.  Upload naar Intune

## Status

In ontwikkeling.

## Bron
Install script https://github.com/MSEndpointMgr/Intune/blob/master/Windows%2010/Install-Printer.ps1

Remove script https://github.com/MSEndpointMgr/Intune/blob/master/Windows%2010/Remove-Printer.ps1
