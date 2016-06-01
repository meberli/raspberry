#Projektdokumentation 
>(PDO, gelegentlich auch Projektabschlussbericht) ist gem. DIN69901 die Zusammenstellung ausgewählter, wesentlicher Daten über Konfiguration, Organisation, Mitteleinsatz, Lösungswege, Ablauf und erreichte Ziele des Projektes.

##Typischer Aufbau
* Projektvorfeld (IST-Analyse)
* Aufgabenstellung (SOLL-Konzept)
* Anforderungen
* Projektziele (SOLL-IST-VERGLEICH)
* Zeitplanung / Meilenstein (Projektmanagement)
* Wirtschaftlichkeit
* Projektverlauf
* Ausblick / Folgeaktivitäten
* Fazit
* Begriffserklärungen

### Anlagen / Anhang: (eigentlich Bestandteil der Projektakte)
* Pflichtenheft
* Angebot
* Preiskalkulation/Nutzwertanalyse
* Kundeneinweisung
* Abnahme- und Testprotokoll
* Rechnung
* ev. Codeauszug

Beispiel
```python
import RPi.GPIO as GPIO
GPIO.setmode(GPIO.BCM)
GPIO.setup(23, GPIO.IN, pull_up_down = GPIO.PUD_DOWN)
GPIO.setup(24, GPIO.IN, pull_up_down = GPIO.PUD_UP)
while True:
if(GPIO.input(23) ==1):
print(“Button 1 pressed”)
if(GPIO.input(24) == 0):
print(“Button 2 pressed”)
GPIO.cleanup()
```
