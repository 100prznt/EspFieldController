
# Water Analytic Riser

Erweitert den [ESP Field Controller](../) um zwei EZO Circuit Sockel, welche die entsprechenden Module von Atlas Scientifics aufnehmen können.

![Zusammenbau im Spelsberg Gehäuse](docu/war_assembly.png)

## Funktionen

Um eine Potentialverschiebung an den eingesetzen Messelektroden zu vermeden, ist sowohl die Versorgungsspannung als auch der I2C Bus für jedes EZO Circuit isoliert ausgeführt. Die herausgeführten Elektrodenanschlüsse sind somit gegeneinander und gegen den ESP Field Controller isoliert, sowohl auf der Messleitung also auch auf der zugehörigen Masse.

* Isolierte Versorgungsspannung je Sockel
* Isolierter I2C Bus je Sockel

## Feature Request

* 1-Wire Stecker für DS18B20
* Taster für Kalibrierung
* LED für Kalibrierung
