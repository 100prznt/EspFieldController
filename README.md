# EspFieldController
Modular aufgebauter Hardware-Controller für den Betrieb mit ESPHome.




## Onboard Funktionen
### Netzteil
* 230 VAC Netzklemme
* Versorgung von ESP und Peripherie
* 24 VDC und 5 VDC
* 3,3 VDC über linearen Spannungsregler
* Automatische Umschaltung zwischen Versorgung per Netzteil und USB

### ESP
* Arduino Nano ESP32


### Erweiterungsport
* 2 unabhängige Ports
* I2C (SCL, SDA)
* 4 GPIOs
* 24V
* 5V
* 3V3
* TE Micro-Match

#### Standardpins
| ~D | GPIO | I2C | SPI         |
|----|------|-----|-------------|
| 21 | 11   | SDA |             |
| 22 | 12   | SCL |             |
| 11 | 38   |     | COPI (MOSI) |
| 12 | 47   |     | CIPO (MISO) |
| 13 | 48   |     | SCK         |


### Relais
* 2 unabhängige Kanäle
* 230 VAC 10 A (einpolig)
* 230 VAC Eingang über Netzklemme, L, N, PE (welche auch das Onboard Netzteil versorgt)
* Ausgangsklemmen inkl. N und PE
#### Safty Circuit
* Optional per eigenen Controller (alternativ per Jumper oder 0R gebrückt)
* Softwarefunktionen
  * Überwachung des ESP per Watchdog
  * Externe Freigabe per Enable Eingang
  * Verriegelung der Kanäle (inkl. Definition von Umschaltzeiten)
* Mögliche Controller
  * ATtiny25 (SOIC)
  * MSPM0C1104 (Cortex-M0+; SOT-23-THN)
