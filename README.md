# EspFieldController
Modular hardware controller for integration into ESPHome.

## Onbaord Funktionen
### Netzteil
* 230 VAC Netzklemme
* Versorgung von ESP und Peripherie
* 24 VDC und 5 VDC
* 3,3 VDC über linearen Spannungsregler
### Relais
Spezifikation
* 2 unabhängige Kanäle
* 230 VAC 10 A
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
