# ReadMe


## Getting started
Latex kann, gerade wenn man noch nie damit zu tun hatte, erstmals komplex wirken. Gerade für Abschlussarbeiten, kann es einem aber einiges an ärger ersparen. 
Ziel dieses Projekts ist es, Anfängern den Einstieg zu erleichtern, eine minimale Grundstruktur und hilfreiche Informationsquellen gesammelt zur Verfügung zu stellen. 

Latex Tutorial gibt es wie Sand am Meer. Manche hilfreich andere eher weniger. Deswegen werden wir hier nicht noch eine schreiben. Allerdings haben wir versucht einige, zumindest unserer Meinung nach, hilfreiche Quellen zusammenzutragen. 

--Tutorial für Einsteiger (TU Graz)

Der Latex Guide der TU Graz gibt einen guten Überblick, was Latex überhaupt ist, welche Software überhaupt benötigt wird und ein kurzes Tutorial, mit dem schrittweise ein erstes Dokument mit LaTeX erstellt werden kann.
Aufrufbar unter:
https://latex.tugraz.at/latex/tutorial

-- The Not So Short Introduction to LATEX 2ε

Ein sehr umfangreicher Einführung in Latex. Hier wird ausführlich auf die Grundlagen eingegangen, aber auch auf fortschrittliche Themen wird eingegangen. Das Dokument gibt es auf Englisch und auf Deutsch, wobei die Englische Fassung aktueller ist. 
Aufrufbar unter: 
https://tobi.oetiker.ch/lshort/lshort.pdf (Englisch)
https://mirror.dogado.de/tex-archive/info/lshort/german/l2kurz.pdf (Deutsch)

-- Overleaf Tutorial

Das Tutorial von Overleaf, einem kollaborativer Cloud-basierter LaTeX-Editor, ist ebenfalls ziemlich umfangreich. Hier wird vor allem mit kurzen Beispielen gearbeitet. 
Aufrufbar unter:
https://de.overleaf.com/learn/latex/Tutorials

-- Wiki Hilfe
Hier sind sämtliche mathematischen Zeichen und Symbole aufgelistet
Aufrufbar unter: 
https://de.wikipedia.org/wiki/Hilfe:TeX

-- Literaturverwaltung 
Wir haben uns für BibLaTex entschieden, da es das Ändern vom Aussehen der Zitate oder des Literaturverzeichnisses wesentlich vereinfacht, eine bessere Dokumantation hat und deutlich mehr Zitierbefehle bietet. 
Grundsätzlich reicht aber auch ein einfacher Text-Editor, dies wird allerdings schnell unübersichtlich daher sollte auf eine zusätzliche Software zurückgegriffen werden. 
Hierfür können kostenpflichtige Software (z.B Mendeley, Citavi) oder Freeware (z.B JabRef) verwendet werden. 

-- sonstige Tipps:

*wie fast immer gilt, Google ist dein Freund. Zu 99% der auftretenden Probleme gibt es bereits Lösungen online. Meist werden diese in Latex Foren wie LaTeX Stack Exchange (https://tex.stackexchange.com/) diskutiert. 

*Für (fast) alle Pakete gibt es eine Dokumenation. Oft lässt sich ein Problem lösen, in dem du die kurz überfliegt. 

*Es gibt auch einige gute YouTube Videos zum Einstieg in Latex.


## How to use this template
Grundsätzlich empfehlen wir die Verwendung von Overleaf. Die TU Wien stellt allen Mitarbeitern_innen und gültig zurückgemeldeten Studierenden eine Overleaf Professional Lizenz zur Verfügung. 
Mehr Infos hier: 
https://de.overleaf.com/edu/tuw#overview

Es ist aber auch möglich die Vorlage mit den üblichen Text Editoren  (siehe Liste unten) zu verwenden. 
!!!!! TO BE TESTED !!!! ;) 
Tested: 

###Grundstruktur

├── chapters
├── img		
├── config.tex
├── README.txt
└── Thesis.tex

- chapters
Hier werden alle einzelen Kapitel abgelegt. Diese können dann per \include{chapters/...} in Thesis.txt importiert werden. 

- img
Hier werden sämtliche Bilder abgelegt. Diese werden dann mittels \includegraphics{img/...} im entsprechenden Dokumente importiert. 

-- config.tex
Das Dokument in dem alle Pakete geladen werden und andere Anpassungen vorgenommen werden können. Dies wird zur besseren Übersichtlichkeit in einer separaten Datei erledigt. Erfüllt die Funktion des Headers

-- README.txt
Die aktuelle Beschreibung 

-- Thesis.tex
Das eigentliche Hauptdokument. Hier werden die einzelne Kapitel importiert, die Verzeichnisse angelegt und die Titelseite konfiguriert. (siehe später)

### Titelseite
Die Titelseite wird automatisch generiert. Dies geschieht nach der Word-Vorlage des Dekanats für Maschinenwesen und Betriebswissenschaften (https://www.tuwien.at/mwbw/dekanat/studienabschluss). 
Hierfür müssen nur die nötigen Daten in Thesis.txt eingegeben werden. 
Der größte Teil sollte selbsterklärend sein, für einige Parameter wird im folgenden eine kurze Erklärung zusammengeschrieben:

type -> wird der Typ der Arbeit angegeben
aktuell werden die Befehle bac,dipl,diss (Bachelorarbeit, Diplomarbeit, Dissertation) unterstützt.

instLogo -> hiermit wird das Institutslogo ausgewählt. es wird die Institutsnummer mit vorangestelltem E (E+Institutsnummer) benötigt z.B. E325 

Die unterstützten Nummern können aus der folgenden Liste entnommen werden. 

E302 - Energietechnik und Thermodynamik
E307 - Konstruktionswissenschaften und Produktentwicklung
E308 - Werkstoffwissenschaft und Werkstofftechnologie
E311 - Fertigungstechnik und Photonische Technologien
E315 - Fahrzeugantriebe und Automobiltechnik
E317 - Leichtbau und Struktur-Biomechanik
E322 - Strömungsmechanik und Wärmeübertragung
E325 - Mechanik und Mechatronik
E330 - Managementwissenschaften

To Do: !!! Alle implementieren !!!! ;)

### Sonstiges 
-- pagestyles wird für die Kapitel in der Thesis.txt gelöst, für die ersten Inhalte (Eidesstattliche, Abstract) im jeweiligen Dokument, da diese nie eine Seitenzahl haben 

-- Postition der Verzeichnisse (Bilder, Tabellen usw.) ist Standardmäßig am Ende vorgesehen, wenn dies am Anfang benötigt wird muss dies selbest verschoben werden. (in Thesis.txt)

 

## License
This Project is based on the https://github.com/joerg/abschlussarbeit-tuwien-physik template.

