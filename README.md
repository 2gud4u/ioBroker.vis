# DashUI 0.3

## Installation auf der CCU

Es wird ein Zugang zur CCU via FTP oder SCP ben�tigt.

* Addon "WebAPI" installieren (den Ordner webapi auf diesem Zip-File https://github.com/hobbyquaker/WebAPI/archive/master.zip nach /www/addons/ kopieren)
* Den Ordner dashui ins Verzeichnis /www/addons/ kopieren
* leeren Ordner /usr/local/addons/dashui erstellen (hier werden Konfigurationen gespeichert)

## Dokumentation

### Views einrichten

* http://ccu/addons/dashui/?edit aufrufen
* W�hrend der Editor ge�ffnet ist finden keine automatischen Refreshs statt.
* Man muss manuell �ber die Buttons "auf CCU speichern" und "von CCU laden" Konfigurationen sichern und laden.

### Widgets

* hm_id ist die ID eines Datepunkts (STATE, LEVEL, TEMPERATURE, ...). Zum nachschauen dieser IDs bietet sich das HQ WebUI an.
* hm_wid ist die ID des WORKING Datenpunkts, sinnvoll bei Dimmern und Rolll�den um springende Slider w�hrend Aktivit�t der Aktoren zu verhindern.

#### basic - Value List

Der Parameter valuelist muss als ; (Semikolon) getrennte Liste angegeben werden

#### jqplot - MeterGauge Widget

Alle weiteren Parameter sind hier dokumentiert: <a href="http://www.jqplot.com/docs/files/plugins/jqplot-meterGaugeRenderer-js.html" target="_blank">jqPlot Docs meterGauge</a></li>

Die Parameter ticks, intervals, intervalColors k�nnen als ; (Semikolon) getrennte Liste angegeben werden

### Navigation

* Zur Navigation k�nnen einfache Links oder Link-Widgets auf #name-der-view genutzt werden, z.B.:

    <a href="#erdgeschoss">Link auf Erdgeschoss-View</a>

### Bedienung

* Einfach den Editor schlie�en oder http://ccu/addons/dashui/ aufrufen

### Rohdaten bearbeiten

Das Javascript Object in dem alle Views und Widgets gespeichert werden kann �ber http://homematic/addons/dashui/views.html bearbeitet werden.

## Todo / Bekannte Fehler

* Views duplizieren, umbenennen und l�schen implementieren
* Fehler beheben - manchmal erscheint kein Inspect-Helper (gestrichelte Linie um Widget) wenn neu eingef�gtes Widget angeklickt wird
* Fehler beheben bei Widget auf andere View kopieren (wird erst nach Reload sichtbar)
* Fehler beheben jqPlot Gauge Widget: Wird nur Fehlerfrei auf der sichtbaren View gerendert :(
* Spezielle Widget-Attribute (Infoschnipsel z.B. f�r die Dokumentation der Attribute)
* Config-File
* Mehr Widgets! ;-)
* Erweiterte Widget-Attribute: CSS-Klassen, Kommentar, ...
* Erweiterte View-Attribute: CSS-Klassen, jqui-Theme?
* Navigations-Effekte (Beim wechseln der View konfigurierbare Animationen)

## Changelog

### 0.3

Erstes �ffentliches Release




## Copyright, Lizenz, Bedingungen

DashUI

Copyright (c) 2013 hobbyquaker https://github.com/hobbyquaker
MIT Lizenz (MIT)

Hiermit wird unentgeltlich, jeder Person, die eine Kopie der Software und der zugeh�rigen Dokumentationen (die
"Software") erh�lt, die Erlaubnis erteilt, sie uneingeschr�nkt zu benutzen, inklusive und ohne Ausnahme, dem Recht,
sie zu verwenden, kopieren, �ndern, fusionieren, verlegen, verbreiten, unterlizenzieren und/oder zu verkaufen, und
Personen, die diese Software erhalten, diese Rechte zu geben, unter den folgenden Bedingungen:

Der obige Urheberrechtsvermerk und dieser Erlaubnisvermerk sind in allen Kopien oder Teilkopien der Software beizulegen.

DIE SOFTWARE WIRD OHNE JEDE AUSDR�CKLICHE ODER IMPLIZIERTE GARANTIE BEREITGESTELLT, EINSCHLIESSLICH DER GARANTIE ZUR
BENUTZUNG F�R DEN VORGESEHENEN ODER EINEM BESTIMMTEN ZWECK SOWIE JEGLICHER RECHTSVERLETZUNG, JEDOCH NICHT DARAUF
BESCHR�NKT. IN KEINEM FALL SIND DIE AUTOREN ODER COPYRIGHTINHABER F�R JEGLICHEN SCHADEN ODER SONSTIGE ANSPR�CHE
HAFTBAR ZU MACHEN, OB INFOLGE DER ERF�LLUNG EINES VERTRAGES, EINES DELIKTES ODER ANDERS IM ZUSAMMENHANG MIT DER
SOFTWARE ODER SONSTIGER VERWENDUNG DER SOFTWARE ENTSTANDEN.


HomeMatic und das HomeMatic Logo sind eingetragene Warenzeichen der eQ-3 AG