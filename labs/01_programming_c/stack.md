# Übungsaufgabe: Stack Implementierung

In dieser Aufgabe implementieren Sie die Datenstruktur Stack in der Sprach C, wie sie in der Vorlesung vorgestellt wurde.  

## Voraussetzungen

Nutzen Sie hierfür [gcc](https://gcc.gnu.org/).

Sie können *gcc* unter Linux und/oder macOS direkt verwenden. Unter Linux installieren Sie *gcc* über Ihren Paket-Manager, unter macOX über [Homebrew](https://brew.sh/).

Nutzen Sie Windows 10 können Sie entweder eine Linux in einer virtuellen Maschine (z.B. in [VirtualBox](https://www.virtualbox.org/)) nutzen, oder direkt das [Windows Subsystem for Linux (WSL 2.0)](https://docs.microsoft.com/en-us/windows/wsl/install-win10) nutzen. Alternativ ist es möglich *Windows Subsystem for Linux* über den Windows App Store zu installieren.

In der Wahl der Linux Distribution sind sie frei, alle Beispiele in der Vorlesung werden jedoch unter Ubuntu (letzter stabiler Release) bewertet und eventuell vorgestellt. 

## Aufgabenstellung 

1. Implementieren Sie einen Stack auf Basis folgender Header-Datei (`stack.h`): 

```c
void push(int val);
int pop();
int peek();
```

2. Ihr Stack verfügt über eine maximale Größe von 100 Elementen. 

2. Ihr Code sollte zu einem gewissen Maße robust sein, stellen Sie daher sicher dass folgende Bedingungen eingehalten werden: 

    a. Beim überschreiten der maximal zulässigen Anzahl von Einträgen durch den Aufruf von `push()` liefert Ihr Code folgende Fehlermeldung: 

    > ERROR: Size 100 of stack exeeded when adding value X

    Wobei X der Wert der Variable ist, welcher versucht wurde auf den Stack zu legen.

    b. Beim Versuch einen Wert mittels `pop()` vom Stack zu nehmen, ohne dass ein Wert auf dem Stack liegt erfolgt folgende Fehlermeldung: 

    > ERROR: Stack is empty, NULL return instead

    In diesem Fall liefert die Funktion `pop()` keinen Integer-Wert, sonden den Wert `NULL` zurück. 

    c. Beim Versuch einen Wert mittels `peek()`vom Stack zu lesen wenn der Stack keine Einträge enthält erfolgt folgender Hinweis: 

    > ERROR: Stack is empty, NULL return instead
     
    In diesem Fall liefert die Funktion `peek()`keinen Integer-Wert, sondern den Wert `NULL`zurück.

    d. Alle drei Fehlermeldungen werden auf [stderr](https://www.gnu.org/software/libc/manual/html_node/Standard-Streams.html) ausgegeben.  

    **Hinweis: Achten Sie darauf, dass bei der Ausgabe der Fehlermeldung diese immer mit einem ZTeilenumbruch (`\n`) endet.**


## Abgabe

Die Bewertung Ihrer Abgabe findet automatisch statt. Stellen Sie hierzu folgende Punkte sicher:

* Ihre Implementierung befindet sich in einer Datei mit dem Namen **stack.c**. 
* Sie nutzen eine Header-Datei in der der obige Header hinterlegt ist. 
* Zur Abgabe erhalten Sie einen Zugang zum hochschulinternen [GitLab](https://git.it.hs-heilbronn.de/).
* Ihre Lösung checken Sie in Ihrem Repository ein.
* Die eigentliche Abgabe erfolgt über das hochschuleigene [Commit-System](https://commit.it.hs-heilbronn.de/). Der Zugriff ist ausschließlich im Hochschulnetz oder über VPN möglich. 

## Bewertung

Die Bewertung Ihrer Aufgabe findet anhand einer Reihe von automatisierten Tests statt. 

Hierzu ist es erforderlich, dass die obigen Schritte exakt eingehalten werden. 

Ihr Implementierung wird einer Reihe von automatisierten Tests unterzogen, die Ihre Implementierung auf Korrektheit überprüfen. 

Abgaben, die nicht vollständig sind oder die Abgabekriterien nicht erfüllen werden nicht bewertet. 

Abgaben, die nicht fristgerecht eingereicht werden, werden nicht bewertet. 

Nutzen Sie zur Abgabe ausschließlich das beschriebene Verfahren. Abgaben, die per E-Mail oder anderen Wegen eingereicht werden, werden nicht bewertet. 

Abgaben, die aufgrund eines Fehlers nicht durch die Tests laufen, werden entsprechend mit weniger Punkten bewertet.