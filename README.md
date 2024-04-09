# EspFieldController
Modular aufgebauter Hardware-Controller für den Betrieb mit ESPHome.




## Onbaord Funktionen
### Netzteil
* 230 VAC Netzklemme
* Versorgung von ESP und Peripherie
* 24 VDC und 5 VDC
* 3,3 VDC über linearen Spannungsregler
* Automatische Umschaltung zwischen Versorgung per Netzteil und USB

### ESP
* Wemos Lolin S2 mini mit ESP32-S2
* optional bestückbar mit Wemos D1 mini?


### Erweiterungsport
* 2 unabhängige Ports
* I2C (SCL, SDA)
* 4 GPIOs
* 24V
* 5V
* 3V3
* TE Micro-Match

#### I2C Standardpins
| GPIO | ESP32 | ESP8266 |
|------|-------|---------|
| 4    |       | SDA     |
| 5    |       | SCL     |
| 21   | SDA   |         |
| 22   | SCL   |         |


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
