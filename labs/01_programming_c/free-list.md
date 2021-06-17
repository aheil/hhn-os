# Übungsaufgabe: Stack Implementierung

In dieser Aufgabe implementieren Sie die Datenstruktur Free List in der Sprach C, wie sie in der Vorlesung vorgestellt wurde.  

## Voraussetzungen

Nutzen Sie wenn möglich [gcc](https://gcc.gnu.org/).

Sie können *gcc* unter Linux und/oder macOS direkt nutzen. Unter Linux installieren Sie *gcc* über Ihren Paket-Manager, unter macOX über [Homebrew](https://brew.sh/).

Nutzen Sie Windows 10 können Sie entweder eine Linux in einer virtuellen Maschine (z.B. in [VirtualBox](https://www.virtualbox.org/)) nutzen, oder direkt das [Windows Subsystem for Linux (WSL 2.0)](https://docs.microsoft.com/en-us/windows/wsl/install-win10) nutzen.

In der Wahl des Linux Systems sind sie frei, alle Beispiele in der Vorlesung werden unter Ubuntu (letzter stabiler Release) vorgestellt. 

## Aufgabenstellung 

1. Implementieren Sie eine einfache Datenstruktur, die Ihren Hauptspeicher repräsentiert.

2. Implementieren Sie eine Datenstruktur Free List, die jeweils die Position und die Größe freier Datenblöcke Repräsentiert. 

3. Aus Ihrer Main Datei wird ein Zufallsgenerator gestartet, der willkürlich Speicherbereiche anfordert und wieder freigibt. Bei jeder Änderung ist die Linked List zu aktualisieren, so dass darin alle freien Speicherbereiche enthalten sind. 

3. Jedes Mal wenn ein Speicherbereich "reserviert" wird, schreiben Sie entsprechende Daten in Ihre Datenstruktur. Wird Speicher frei gegeben, werden die Daten gelöscht. 

4. Ihr Programm muss mind. 100 Iterrationen durchlaufen. 

5. Implementieren Sie entsprechende Ausgaben auf der Konsole, so das der jeweilige Status der Free-List erkennbar ist. 

## Abgabe

Die Bewertung Ihrer Abgabe findet automatisch statt. Stellen Sie hierzu folgende Punkte sicher:

* Ihre Implementierung befindet sich in einer Datei mit dem Namen **stack.c**. 
* Sie nutzen eine Header-Datei in der der obige Header hinterlegt ist. 
* Ihre Implementierung darf maximal den System-Header `stdio.h` referenzieren. 
* Zur Abgabe erstellen Sie eine ZIP-Datei, die ausschließlich Ihre C-Datei enthält und stellen diese in der entsprechenden ILIAS-Abgabe bereit.

## Bewertung

Die Bewertung Ihrer Aufgabe findet anhand einer Reihe von  Tests statt. 

Ihr Implementierung wird einer Reihe von Tests unterzogen, die Ihre Implementierung auf Korrektheit überprüfen. 

Abgaben, die nicht vollständig sind oder die Abgabekriterien nicht erfüllen werden nicht bewertet. 

Abgaben, die nicht fristgerecht eingereicht werden, werden nicht bewertet. 

Nutzen Sie zur Abgabe ausschließlich die In ILIAS gegebene Möglichkeit. Abgaben, die per E-Mail oder anderen Wegen eingereicht werden, werden nicht bewertet. 

Abgaben, die aufgrund eines Fehlers nicht durch die Tests laufen werden entsprechend mit weniger Punkten bewertet. 
