# Kaufberatung

Hier haben wir unsere Empfehlungen für Freifunk-Hardware zusammengestellt.
Alle diese Geräte sind mit unserer Firmware kompatibel und können in unserem Netz betrieben werden.

Ebenso verfügen sie über mindestens Wi-Fi 5 und unabhängig von der WLAN-Generation über **Dualband-WLAN** auf 2.4 und 5 GHz.

!!! note "Andere Empfehlungen"
    Viele Freifunk-Communitys haben eigene Empfehlungen für Hardware.
    Insbesondere Empfehlen manche Communitys noch Geräte, welche schlechter und teurer als die hier empfohlenen Geräte sind.
    Es gibt keinen Grund, diese Geräte zu kaufen, da sie nicht mehr zeitgemäß sind.

Wir haben die Geräte nach Anwndungsfall in drei Kategorien
unterteilt:

 - **Empfohlen** Diese Geräte, haben wir selbst getestet und sind in der Praxis bewährt. Sie unterstützen aktuelle WLAN-Standards und sind neu im Handel erhältlich.

 - **Günstig** Diese Geräte sind oft günstig erhältlich. Sie unterstützen nur ältere WLAN-Standards und sind daher etwas langsamer und unterstützen weniger gleichzeitig verbundene Nutzer.

 - **Experimentell** Diese Geräte sind bisher nicht in unserem stabilen Firmware-Release enthalten. Sie sind allerdings entweder attraktiv bepreist oder bieten besondere Features.


Diese Klassen sind untereinander nach Installationsart gruppiert

 - **Webinterface** Diese Geräte können über ein Webinterface geflasht werden. Das ist besonders einfach und für Einsteiger geeignet.

 - **TFTP** Diese Geräte müssen über (T)FTP geflasht werden. Das ist etwas komplizierter, anleitungen sind aber verlinkt.

 - **SSH** Diese Geräte müssen über SSH geflasht werden. Das ist etwas komplizierter, anleitungen sind aber verlinkt.

<!--
 - **Serielles Kabel** Diese Geräte müssen über ein serielles Kabel geflasht werden. Das ist die komplizierteste Methode und benötigt spezielle Hardware.
-->

## Empfohlen

=== "Webinterface"

    | Gerät (Anleitung) | Stromversorgung | Montagemöglichkeiten | Ethernetports | Wi-Fi Standard | Preis | 
    |-------|-----------------|----------------------|---------------|----------------|-------|
    | [ZyXEL NWA50AX](https://git.openwrt.org/?p=openwrt/openwrt.git;a=commit;h=a0b7fef0ffe4cd9cca39a652a37e4f3ce8f0a681) | Netzteil / [PoE](https://de.wikipedia.org/wiki/Power_over_Ethernet) | Deckenmontage | 1 | Wi-Fi 6 802.11ax | [70 €](https://geizhals.de/ zyxel-nwa50ax-nwa50ax-eu0102f-a2634708.html) |
    | [Zyxel NWA55AXE](https://git.openwrt.org/?p=openwrt/openwrt.git;a=commit;h=a0b7fef0ffe4cd9cca39a652a37e4f3ce8f0a681) | [PoE](https://de.wikipedia.org/wiki/Power_over_Ethernet) | Outdoor Mast | 1 | Wi-Fi 6 802.11ax | [95 €](https://geizhals.de/zyxel-nwa55axe-nwa55axe-eu0102f-a2634709.html) |
    | [D-Link DAP-X1860](https://openwrt.org/inbox/toh/d-link/dap-x1860) | Integriert | Steckdose | 1 | Wi-Fi 6 802.11ax | [29 €](https://geizhals.de/d-link-dap-x1860-e-a2418687.html) |

=== "TFTP"

    | Gerät | Stromversorgung | Montagemöglichkeiten | Ethernetports | Wi-Fi Standard | Preis | 
    |-------|-----------------|----------------------|---------------|----------------|-------|
    | [AVM Fritz!Box 4040](https://fritz-tools.readthedocs.io/de/latest/flashing/general.html) | Netzteil | Aussparung für Schraubenköpfe | 1+4 | Wi-Fi 5 802.11ac (Wave2) | [93 €](https://geizhals.de/avm-fritz-box-4040-20002763-a1501050.html) |


## Günstig

!!! note "Spende"
    Aufgrund einer großzügigen Spende haben wir einige dieser Geräte auf Lager,
    die wir gerne auf Anfrage abgeben. Eine kurze Nachricht im Chat oder per E-Mail mit deinem Standort reicht.


=== "Webinterface"


    | Gerät | Stromversorgung | Montagemöglichkeiten | Ethernetports | Wi-Fi Standard | Preis |
    |-------|------|-----|-----|-------|-------|
    | [Genexis EX400](https://github.com/freifunk-darmstadt/projects/wiki/90-%E2%80%90-Hardware-%E2%80%90-Genexis-EX400) | Netzteil | Aussparung für Schraubenköpfe | 1+1 | Wi-Fi 5 802.11ac (Wave2) | Im Chat erfragen |


## Experimentell

=== "Webinterface"

    | Gerät (Anleitung) | Stromversorgung | Montagemöglichkeiten | Ethernetports | Wi-Fi Standard | Preis | 
    |-------------------|-----------------|----------------------|---------------|----------------|-------|
    | [Zyxel NWA50AX Pro](https://github.com/openwrt/openwrt/commit/f0445746f6fd96fc7c5394b238153bd2ff22bc5b) | Netzteil / [PoE](https://de.wikipedia.org/wiki/Power_over_Ethernet) | Deckenmontage | 2.5 GBit/s | Wi-Fi 6 802.11ax | [90 €](https://geizhals.de/zyxel-nwa50ax-pro-nwa50axpro-eu0102f-a2974098.html) |
    | [ASUS RT-AX52](https://openwrt.org/toh/asus/rt-ax52#installation) | Netzteil | Keine | 1+3 | Wi-Fi 6 802.11ax | [40 €](https://geizhals.de/asus-rt-ax52-90ig08t0-mo3h00-a3031824.html) |

=== "SSH"

    | Gerät (Anleitung) | Stromversorgung | Montagemöglichkeiten | Ethernetports | Wi-Fi Standard | Preis | 
    |-------------------|-----------------|----------------------|---------------|----------------|-------|
    | [ASUS TUF AX4200](https://github.com/blocktrron/openwrt-asus-filogic-factory/releases/tag/filogic-v1) | Netzteil | Keine | 2.5 Gbit/s WAN + 4 x Gbit/s LAN | Wi-Fi 6 802.11ax | [105 €](https://geizhals.de/asus-tuf-ax4200-rt-ax4200-a2634707.html) |
