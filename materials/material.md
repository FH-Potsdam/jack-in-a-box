---
title:  Jack in a Box Material
author: Fabian Morón Zirfas
geometry: margin=1.25cm
papersize: A4
fontsize: 13pt
geometry: top=3cm
geometry: left=2.25cm
geometry: right=2.25cm
geometry: bottom=3cm
linkcolor: TealBlue
---

# Info

Um die Boxen zu bauen haben wir 2 unterschiedliche Möglichkeiten. Entweder wir versuchen die Materialien einzeln und so günstig wie möglich zu kaufen (Arduino Pro Mini) oder wir sparen uns die Zeit und geben etwas mehr Geld aus (Adafruit Feather M0 oder Adafruit Feather HUZZAH mit ESP8266 WiFi).  

**TLDR;**  

Wenn jede/r von euch nur 2 Boxen baut spart ihr in der günstigen Variante ca 12€. Dafür haben wir um einiges mehr Aufwand die Boards zu besorgen und unvorhersebare Problem (Kompatibilität der Charger mit LiPo Batterien, FTDI Programmer etc). Mein Rat ist die 12€ eure mehr auszugeben und damit möglichen Problemen aus dem Weg zu gehen. Nicht bedacht sind bau von Switches, Firewalls etc.[^4]  

\newpage

## Pro Mini Board

### Pro Person

- 1 × [LiPo Charger](http://www.exp-tech.de/adafruit-mini-lipo-w-mini-b-usb-jack-usb-liion-lipoly-charger) 7,65€
- 1 × [FTDI Programmer](http://www.exp-tech.de/sparkfun-beefy-3-ftdi-basic-breakout)[^2] 15,95€
- 1 × [USB A auf MicroUSB Kabel](http://www.exp-tech.de/micro-usb-kabel-1m?___SID=U) 1,9€

### Pro Box

#### Zwingend:  

- 1 ×  [Arduino Pro Mini](https://ex-store.de/Arduino-Pro-Mini-328-3V3-8MHz-kompatibles-Board)  3,49€
- 1 × LiPoly Batterie  
    + **Nur einer wird Por Board benötigt**
    + [LiPo 2000 mAH](http://www.exp-tech.de/lipo-akku-2000mah)[^1] 8,5€ 
    + [LiPo 900 mAH](http://www.exp-tech.de/polymer-lithium-ion-battery-900mah-6618?___SID=U) 7,5€
- 1 × [JST Header](http://www.exp-tech.de/jst-s2b-ph-k-s-lf-sn-2-kont-stecker-seitlicher-eingang?___SID=U) (Wenn kein LiPoly Adapter verwendet wird) 0,5€

#### Nice to have:  

- 1 × [LiPoly Adapter](http://www.exp-tech.de/adafruit-switched-jst-ph-2-pin-smt-right-angle-breakout-board) (Ersetzt JST Header) 2,8€ 

\newpage

| Menge | Name                | Preis in € | Zwingend | Kommentar              |
| :--   | :--                 | :--        | :--      | :--                    |
| 1     | LiPo Charger        | 7,65       | ja       |                        |
| 1     | FTDI Programmer     | 15,95      | ja       | Gibt es günstiger      |
|       |                     |            |          | möglicherweise auch    |
|       |                     |            |          | günstiger              |
| 1     | USB A auf Micro USB | 1,9        |          |                        |
| n[^3] | Arduino Pro Micro   | 3,49       | ja       |                        |
| n     | LiPo Batt. 2000mAH  | 8,5        | ja       | mindestens 1000mAH     |
| n     | JST Header          | 0,5        | ja       | wenn kein LiPo Adpater |
|       |                     |            |          | genutzt wird           |
| n     | LiPoly Adapter      | 2,8        | nein     | siehe JST Header       |

Gesamtkosten für eine Box ohne weitere Bauelemente sind insgesamt max: 34,79€
Jede weitere Box kostet dann max: 17,19€

**Rechenbeispiel:**  

1 × Box = 34,79€  
2 × Box = 51,89€  
3 × Box = 68,99€  

\newpage

## Feather Board

### Pro Person  

- 1 × [USB A auf MicroUSB Kabel](http://www.exp-tech.de/micro-usb-kabel-1m?___SID=U) 1,9€  

### Pro Box  

- Feather Board
    + **Nur eine Variante wird benötigt**
    + [Adafruit Feather HUZZAH mit ESP8266 WiFi](http://www.exp-tech.de/adafruit-feather-huzzah-with-esp8266-wifi) 18,95€
    + [Adafruit Feather M0 Basic Proto - ATSAMD21 Cortex M0](http://www.exp-tech.de/adafruit-feather-m0-basic-proto-atsamd21-cortex-m0) 21,5€
- 1 × LiPoly Batterie  
    + Nur einer wird Por Board benötigt
    + [LiPo 2000 mAH](http://www.exp-tech.de/lipo-akku-2000mah) 8,5€ 
    + [LiPo 900 mAH](http://www.exp-tech.de/polymer-lithium-ion-battery-900mah-6618?___SID=U) 7,5€

| Menge | Name                | Preis in € | Zwingend | Kommentar          |
| :--   | :--                 | :--        | :--      | :--                |
| n     | Feather Board       | 21,5       | ja       | Das ESP Board      |
|       |                     |            |          | ist günstiger      |
| n     | LiPo Batt. 2000mAH  | 8,5        | ja       | mindestens 1000mAH |
| 1     | USB A auf Micro USB | 1,9        | ja       |                    |

Gesamtkosten für eine Box ohne weitere Bauelemente sind insgesamt max: 31,9€
Jede weitere Box kostet das gleiche.  

**Rechenbeipiel:**  

1 × Box = 31,9€  
2 × Box = 63,8€  
3 × Box = 95,7€  



[^1]: Milliamper (mA) Stunden (H). D.h bei 2000 mAH können wir zB 100mA 20 Stunden lang ziehen oder 1000mAH für 2 Stunden. Beispiel: Ein Neopixel verbraucht ca 60 mA in 100% Helligkeit. Wenn dieser Pixel 1 Stunde läuft haben wir 60 mAH verbracht. Bei einer 2000 mAH Batterie hätten wir also 33 Stunden Laufzeit ([Quelle](https://learn.adafruit.com/battery-power-for-led-pixels-and-strips/estimating-running-time)).
[^2]: 2 × vorhanden im Bestand der FHP  
[^3]: n = Menge an Boxen die gebaut werden
[^4]: Bezugsquellen sind verlinkt.  


