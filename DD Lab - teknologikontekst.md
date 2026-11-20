# DD Lab — teknologikontekst til kreativt projektarbejde

Denne fil kan bruges alene eller sammen med *DD Lab - tilgang.md*, som beskriver lab’ets tilgang til teknologi og prototyping og giver anvisninger til AI’ens støtte undervejs. Tilgangsfilen er et frivilligt supplement og skal kun anvendes, når den studerende vælger at inddrage den.

## Anvendelse i samtalen

Dette dokument er en kontekstressource til en AI-assistent, som hjælper studerende med kreativt projektarbejde. Det beskriver den dokumenterede del af DD Labs teknologiudbud inden for physical computing samt lokale hardwarevarianter og relevante vejledninger.

Brug oplysningerne, når de er relevante for den studerendes projektidé, spørgsmål og præferencer:

- Forbind projektets ønskede oplevelser, interaktioner og funktioner med relevante boards, sensorer, outputenheder, motorer og softwaretilgange fra referencen.
- Forklar, hvorfor en foreslået teknologi passer til projektet, og hvilke praktiske forhold eller begrænsninger der er relevante. Hjælp efter behov med idéudvikling, teknologivalg, prototyper, opsætning og kode.
- Skeln mellem dokumenterede lokale oplysninger, udtrykkelige anbefalinger fra laboratoriets kilder og dine egne forslag til anvendelse eller kombinationer. Kreative anvendelsesforslag er ikke i sig selv dokumenterede laboratorieeksempler.
- Brug de relevante links til laboratoriets og producenternes vejledninger, når yderligere detaljer er nødvendige, og du har mulighed for at åbne dem. Hvis du ikke kan åbne dem, må du ikke fremstille deres aktuelle indhold som kontrolleret.
- Behandl referencen som et dateret overblik, ikke som en aktuel lagerliste. En opført teknologi er dokumenteret af laboratoriet; aktuelt antal, tilgængelighed og stand er ikke fastslået. Oversigten er ikke udtømmende, og fravær fra dokumentet betyder ikke fravær fra laboratoriet.
- Gør opmærksom på manglende oplysninger og kildeuklarheder, når de påvirker et konkret forslag. Tag højde for den præcise hardwarevariant ved vejledning om firmware, tilslutning og strømforsyning.

Denne kontekstfil fastlægger ikke i sig selv en arbejdsform. Når den studerende vælger at bruge tilgangsfilen, følges dens anvisninger til samarbejdet og arbejdet med kode og prototyper.

## Referencegrundlag og afgrænsning

- Forfatter til kildematerialet: dd lab, ddlab@au.dk.
- Referencens angivne kildedato: 29. oktober 2026.
- Oplysninger og links kan være ændret siden den angivne kildedato.
- Dækning: den offentlige CircuitPython- og STEMMA QT-samling samt det tilknyttede ESP-boardmateriale; ikke hele laboratoriets teknologiudbud.

---

# DD Lab — kontekst om physical computing

Øjebliksbillede af referencematerialet · Kilder gennemgået 29. oktober 2026

## Formål

At give studerende faktuel, lokal kontekst til brug med deres sædvanlige AI-assistent: udstyr dokumenteret af DD Lab, relevante detaljer om laboratoriets opsætning samt links til lokale ressourcer og producenternes vejledninger. Assistenten kan bruge oplysningerne sammen med den studerendes egne mål og præferencer.

Lokale anbefalinger medtages kun, når de står udtrykkeligt i kildematerialet, og henføres til den pågældende kilde.

Afgrænsning: den offentlige samling om CircuitPython og STEMMA QT samt det tilknyttede materiale om ESP-boards. Dette er ikke en komplet fortegnelse over physical computing-udstyr. At en komponent er medtaget, betyder, at laboratoriet har dokumenteret den; dens aktuelle tilgængelighed, antal og stand er ikke fastslået her.

## Centrale ressourcer

| Ressource                                                                                            | Indhold                                                                       |
| ---------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| [DD Labs vejledninger](https://ddlabau.github.io/)                                                   | Udvalgt oversigt over vejledninger til teknologi og udstyr.                   |
| [CircuitPython og STEMMA QT](https://ddlabau.github.io/CircuitPython-and-STEMMA-QT/)                 | Boards, komponenter, netværk og motorer.                                      |
| [Boards](https://ddlabau.github.io/CircuitPython-and-STEMMA-QT/boards/)                              | Boardmodeller, lokale varianter og links til firmware.                        |
| [STEMMA QT-komponenter](https://ddlabau.github.io/CircuitPython-and-STEMMA-QT/stemmaqt/)             | Komponentbeskrivelser med officielle vejledninger og eksempler.               |
| [Andre komponenter](https://ddlabau.github.io/CircuitPython-and-STEMMA-QT/other/)                    | Yderligere sensorer, outputenheder og komponenter med separat ledningsføring. |
| [Netværk og avancerede teknologier](https://ddlabau.github.io/CircuitPython-and-STEMMA-QT/advanced/) | Eksempler med WipperSnapper, Adafruit IO og Shelly.                           |
| [Motorvejledning](https://ddlabau.github.io/CircuitPython-and-STEMMA-QT/komplet_motor_guide/)        | Bevægelsestyper, drivere og oplysninger om tilslutning.                       |
| [Faciliteter og udstyr](https://ddlabau.github.io/faciliteter-og-udstyr/)                            | Bredere udstyrsoversigt og lokale adgangsbetingelser.                         |

Linkene er en del af konteksten og giver adgang til detaljer ud over denne oversigt. Datoen for kildegennemgangen betyder ikke, at alle de linkede sider blev opdateret den dag.

## Boards dokumenteret i CircuitPython-oversigten

| Lokalt ID | Board | Lokale detaljer | Producentens læringsressource |
| --- | --- | --- | --- |
| b1 | QT Py S3 | Kompakt ESP32-S3-board med STEMMA QT. | [QT Py ESP32-S3](https://learn.adafruit.com/adafruit-qt-py-esp32-s3) |
| b2 | Feather S3 | Batteritilslutning; laboratoriet angiver varianter både med og uden PSRAM. Mærkningen på undersiden identificerer varianten ved valg af firmware. | [ESP32-S3 Feather](https://learn.adafruit.com/adafruit-esp32-s3-feather) |
| b3 | Feather RP2040 Adalogger | MicroSD-kortplads, batteritilslutning og STEMMA QT; ingen indbygget Wi-Fi eller Bluetooth. | [RP2040 Adalogger](https://learn.adafruit.com/adafruit-feather-rp2040-adalogger) |


## Katalog over STEMMA QT-komponenter

Kilde: [det lokale STEMMA QT-katalog](https://ddlabau.github.io/CircuitPython-and-STEMMA-QT/stemmaqt/). ID'erne nedenfor følger indholdets opslag frem for de inkonsekvente betegnelser i navigationen.

| ID | Komponent |
| --- | --- |
| i1 | Temperatur og luftfugtighed |
| i2 | Temperatur og lufttryk/højde |
| i3 | Luftkvalitetssensor: eCO2/VOC |
| i4 | Lys og nærhed/afstand |
| i5 | Accelerometer |
| i6 | Drejeencoder |
| i7 | Gamepad |
| i8 | Realtidsur |
| i9 (navigation) | Strøm- og spændingssensor til lavspænding |
| i10 | Wii Nunchuck og adapter |
| i11 | IR-sensor til tilstedeværelse/bevægelse |
| i12 | Refleksionsbaseret optisk afbrydersensor |
| i13 | Læser til vejecelle/strain gauge |
| i14 | Mini-GPS |
| i15 | APDS9960-sensor til nærhed, lys, RGB og gestus |
| i16 | SCD41-sensor til CO2, temperatur og luftfugtighed |
| i+ | ANO-drejeencoder; kapacitiv berøringssensor |
| o1 | LED-matrix på 13×9 |
| o2 | Haptik-/vibrationscontroller |
| o3 | 1,5-tommers OLED med gråtoner |
| o4 | Syvsegmentdisplay med fire tegn |
| o5 | NFC-komponent til tekst/links |
| o6 | LCD med I2C-adaptermodul (backpack) |
| o7 | MOSFET-driver |

Kataloget linker til vejledninger for de enkelte komponenter og for mange komponenters vedkommende også til eksempelsider. Produktsider identificerer hardwaren; vejledninger beskriver opsætning og brug. At et produkt er tilgængeligt hos en ekstern leverandør, dokumenterer ikke laboratoriets lagerbeholdning.

## Andre komponenter

Kilde: [det lokale katalog over andre komponenter](https://ddlabau.github.io/CircuitPython-and-STEMMA-QT/other/).

| ID | Komponent |
| --- | --- |
| m1 | Fingeraftrykssensor |
| m2 | GPS |
| m3 | Sensor til jordfugtighed og temperatur |
| m4 | Trykknap med taktil feedback |
| m5 | Farvedisplay |
| m6 | Infrarød sender/modtager |
| m7 | MOSFET-motordriver |
| m8 | Servo |
| m9 | I2S DAC med minijackudgang |
| m10 | I2S DAC/forstærker til små højttalere |
| m12 | NeoPixel-strimmel |
| m13 | Niakset orienteringssensor |
| m+ | Infrarød modtager til fjernbetjening |

Lokale detaljer: Vejledningen til farvedisplayet bruger en Feather-opsætning. Laboratoriet beskriver sin niaksede sensor som varianten uden STEMMA QT-stik. Lydopslagene skelner mellem en minijackudgang og en forstærket udgang til små højttalere.

## Motorer og bevægelse

Kilde: [den lokale motorvejledning](https://ddlabau.github.io/CircuitPython-and-STEMMA-QT/komplet_motor_guide/).

| ID | Komponent |
| --- | --- |
| n0 | Lille solenoide |
| n1 | Positionsservo |
| n2 | Servo med kontinuerlig rotation |
| n3 | DC-motor |
| n4 | DC-motor med gear |
| n5 | Stor solenoide |
| n6 | Stepmotor |
| o2 | Vibrationsmotor/-controller |
| Intet ID angivet | Afsnit om lineær aktuator |

Vejledningen beskriver bevægelsesegenskaber, drivere og ekstern strømforsyning. Den identificerer stepmotorerne som NEMA17-enheder genbrugt fra ældre printere og linker til en [Adafruit-vejledning til TMC2209](https://learn.adafruit.com/adafruit-tmc2209-stepper-motor-driver-breakout-board/circuitpython-and-python). En motors præcise elektriske krav afhænger af den konkrete hardware og driver.

## Software- og netværkstilgange i materialet

| Tilgang | Hvad det lokale materiale dækker |
| --- | --- |
| CircuitPython | Links til boardfirmware samt komponentspecifikke vejledninger og eksempler. |
| WipperSnapper | En Wi-Fi-løsning uden programmering via Adafruit IO, udtrykkeligt beskrevet som begrænset i omfang. |
| Adafruit IO med CircuitPython | Udveksling af data og kommandoer mellem boards og computere. |
| Shelly-stik | Selvstændig webgrænseflade og eksempler på styring og aflæsning af status via netværket. |


## Udvalgte direkte links til Adafruit

Dette er konkrete ressourcer, som DD Labs materiale eller de tilknyttede producentvejledninger linker til. At de er medtaget, indebærer ikke en ubekræftet påstand om brugerens niveau eller en foretrukken undervisningsrækkefølge.

| Komponent | Produktidentifikation | Læringsressource |
| --- | --- | --- |
| APDS9960 | [Produkt 3595](https://www.adafruit.com/product/3595) | [Python og CircuitPython](https://learn.adafruit.com/adafruit-apds9960-breakout/circuitpython) |
| DRV2605L-haptikcontroller | [Produkt 2305](https://www.adafruit.com/product/2305) | [Python og CircuitPython](https://learn.adafruit.com/adafruit-drv2605-haptic-controller-breakout/python-circuitpython) |
| MPR121-berøringssensor | [Produkt 1982](https://www.adafruit.com/product/1982) | [Python og CircuitPython](https://learn.adafruit.com/adafruit-mpr121-12-key-capacitive-touch-sensor-breakout-tutorial/python-circuitpython) |
| WipperSnapper | Software-/firmwareløsning | [Kom hurtigt i gang](https://learn.adafruit.com/quickstart-adafruit-io-wippersnapper?view=all) |
| WipperSnapper på QT Py S3 | Den præcise boardvariant er afgørende | [Opsætning af boardet](https://learn.adafruit.com/adafruit-qt-py-esp32-s3/wippersnapper-setup) |

Yderligere produkt- og vejledningslinks findes i de lokale komponentkataloger. Ikke alle eksterne links i katalogerne er kontrolleret særskilt.
