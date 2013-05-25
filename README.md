# DashUI

## Dokumentation

siehe https://hobbyquaker.github.io/DashUI


## Todo

* Mehr Widgets! ;-)
* Config-File, Editor und Engine sauber trennen
* Erweiterte Template-Attribute: Doku, Kompatibilit�t, ...


## Changelog

### 0.7
* Container implementiert, Views k�nnen nun in Widgets und jQuery UI Dialogen dargestellet werden
* Fehler behoben - Buttons waren nicht mehr editierbar
* Dialog-Widgets mit zus�tzlichen Attributen ausgestattet
* container und view id pr�fix, link disable im edit-mode
* neues Widget-Set: "fancyswitch"
* Widget-Definitionen und Bindings in eigene Files ausgelagert
* toggle Binding und neue Widgets
* diverse Fehler behoben, Pfade gek�rzt (100-Zeichen-Limit...)

### 0.6

* Sind keine lokalen Views vorhanden wird nun automatisch versucht die Views von der CCU zu laden
* W�hrend des Ladevorgangs wird div#loader eingeblendet
* Widget-Select wird nun aktualisiert wenn Widgets gel�scht werden
* Diverse Fehler beim duplizieren von Views behoben
* Beim �ndern von Widget-Attributen werden Widgets nun neu gerendert, es ist kein Reload mehr notwendig
* View-Select ist jetzt alphabetisch sortiert
* Instanzen und Variablen f�r externe Kommandos werden nicht mehr automatisch angelegt und k�nnen entfernt werden
* Widget "mfd-icon Shutter/Dimmer + jqui Dialog" neue Attribute autoclose und modal
* Widget "basic - Red Number" Zahl sitzt nun sauber in der Mitte
* Widget "jqui Button Link" und "jqui Button Link _blank" fehlendes Attribut erg�nzt


### 0.5

* externe Steuerung �ber automatisch angelegte Systemvariablen, bisherige Befehle: alert, changeView, reload, popup
* Widget jqui Radio ValueList hinzugef�gt
* Widget jqui Select ValueList hinzugef�gt
* diverse Fehler behoben
* Widget jqui Input Datetime ausgearbeitet


### 0.4

* Views k�nnen nun unterschiedliche jQuery UI Themes zugewiesen werden, 3 Themes sind bisher mitgeliefert
* Ab sofort kann als Attribut hm_id neben der id auch eine Adresse in der Form BidCos-RF.EEQ0012345:1.LEVEL bzw ein Variablen- oder Programmname angegeben werden
* �ber http://ccu/addons/dashui/reset.html kann der Cache komplett geleert werden
* diverse Fehler beim Selektieren von Widgets und Wechseln der View behoben
* Views k�nnen nun gel�scht und umbenannt werden
* Views werden nun erst beim erstmaligen Aufruf gerendert (merzt auch jqPlot Probleme aus)
* Views und Widget k�nnen nun CSS-Klassen zugewiesen werden
* Widget jqui-input und jqui-input-set-button mit weiteren Attributen ausgestattet
* Widget mfd-icon Shutter angepasst
* Widget basic - rednumber: Zeigt Ganzzahlwerte an, verschwindet bei Wert 0 (iOS-Like...)
* mfd-icons werden nun vollst�ndig mitgeliefert

### 0.3

* Erstes �ffentliches Release


## In DashUI verwendete Software

alle verwendeten Softwarekomponenten stehen (unter anderem) unter einer MIT-Lizenz zur Verf�gung.

* jQuery http://jquery.com/
* CanJS http://canjs.com/
* lostorage.js https://github.com/js-coder/loStorage.js
* jqHomematic https://github.com/hobbyquaker/jqHomematic
* jQuery UI http://jqueryui.com/
* jQuery UI Multiselect Widget https://github.com/ehynds/jquery-ui-multiselect-widget
* jQuery UI Timepicker http://trentrichardson.com/examples/timepicker/
* jqPlot http://www.jqplot.com/

CC-Lizensierte Icons aus dem KNX-User-Forum http://knx-user-forum.de mfd.gfx@gmail.com User: mfd

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