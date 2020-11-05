---

marp: true
theme: defalut
paginate: true
footer: 

---
<style>
img[alt~="center"] {
  display: block;
  margin: 0 auto;
}
</style>
# Fortgeschrittene Speicherverwaltung
## Paging 
Prof. Dr.-Ing. Andreas Heil

![h:32 CC 4.0](../img/cc.svg)![h:32 CC 4.0](../img/by.svg) Licensed under a Creative Commons Attribution 4.0 International license. Icons by The Noun Project.

v1.0.0

---

# Lernziele und Kompetenzen

---

# Motivation

* Bisher gelernt: Segmentierung führt früher oder später dazu, dass der Speicher fragmentiert…
* Glücklicherweise nutzen Betriebssysteme noch einen zweiten Mechanismus der Speicherverwaltung: Paging
* Dabei wird der Speicher in fixe Einheiten aufgeteilt 
  * Jede solche fixe Einheit heißt Page (dt. Speicherseite)
  * Der physikalische Speicher ist demnach eine Aneinanderreihung von gleichgroßen Slots 
  * Jeder solcher Slot heißt Page Frame (dt. Seitenrahmen)
  * Jeder Frame kann eine Page enthalten 

---

# Beispiel 

Hier ein einfaches Beispiel:
  * 64-Byte virtueller Adressraum
  * 4 Pages a 16-Byte Pages
  * Betriebssystem muss »nur« vier freie Page Frames finden
  * Dafür gibt es eine Free List mit freien Page Frames
  * Datenstruktur mit den Einträgen wo eine Page im physikalischen Speicher liegt, heißt Page Table (dt. Seitentabelle)
  * Es gibt eine Page Table pro Prozess


---

# Zuordnung von Frames 

![center](../img/os.12.paging.de.png)

---

# Referenzen 

---

# Bildnachweise

