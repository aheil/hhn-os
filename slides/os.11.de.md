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
## Free-Space Management 
Prof. Dr.-Ing. Andreas Heil

![h:32 CC 4.0](../img/cc.svg)![h:32 CC 4.0](../img/by.svg) Licensed under a Creative Commons Attribution 4.0 International license. Icons by The Noun Project.

v1.0.0

---

# Lernziele und Kompetenzen

---

# Wiederholung

* Bisher galt die Annahme, das alle Adressräume gleich sind
* Somit muss man »eigentlich nur« die nächste freie Lücke finden und »auffüllen«
* Segmentierung führt nun jedoch zur Fragmentierung (engl. external fragmentation)
* Innerhalb eines Adressraus spricht man ebenfalls von Fragmentierung (engl. internal fragmentation)

Beispiel: Heap

![center w:600](../img/os.11.heap.de.png)

---

# Free List

* Datenstruktur zur Verwaltung freier Speicherbereiche ist die sog. Free List
* Basiert auf einer verketteten Liste (engl. linked list)

![center w:800](../img/os.11.freelist.de.png)

---

# Free List Beispiel (1) 

* Anfragen für größer 10 Bytes schlagen fehl (liefert NULL)
* Exakt 10 Bytes kann durch einen der beiden Blöcke bedient werden 
* Aber was passiert, wenn nur 1 Byte angefordert wird?

![center w:700](../img/os.11.freelist_example.de.png)

---

# Free list Beispiel (2)

* Anfragen für größer 10 Bytes schlagen fehl (liefert NULL)
* Exakt 10 Bytes kann durch einen der beiden Blöcke bedient werden 
* Aber passiert, wenn nur 1 Byte angefordert wird?
* Einer der freien Blöcke wird verkleinert…

![center w:700](../img/os.11.freelist_example_2.de.png)

---

# Free list Beispiel (3)

* Zurück zur Ausgangssituation mit drei Blöcken…
* Was passiert wenn der mittlere Block freigegeben wird? 
* Es entstehen drei Blöcke… keine Gute Idee…

![center w:850](../img/os.11.freelist_example_3.de.png)

---

# Free list Beispiel (4)

* Daher fasst die zuständige Bibliothek den freien Speicher vor dem Allokieren so gut wie möglich zusammen

![center w:550](../img/os.11.freelist_example_4.de.png)

---

# Referenzen 

---

# Bildnachweise

