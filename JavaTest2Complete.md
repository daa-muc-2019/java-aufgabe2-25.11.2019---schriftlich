
-Seite 1

**Name:**

## Java

### 1 (3 Punkte)
* Bringen Sie die folgenden Begriffe in eine sinnvolle Reihenfolge (Entstehung bis Ausführung eines Java Programms)

	* Quelltext
	* Java virtual machine (JVM)
	* realer Prozessor
	* Bytecode
	* Java Compiler

Antwort:
```
1. Quelltext



2.



3.



4.



5. realer Prozessor
```
## 2 (6 Punkte)
* Erläutern Sie die Begriffe `Syntax`, `Semantik`, `Pragmatik` anhand eines Beispiels. (java oder it oder natürliche Sprache)

Antwort:
```
 - Syntax:





  - Semantik:





 - Pragmatik:





 ```


# Klassen und Objekte / UML
## 1 (12 Punkte)
* Gegeben seien zwei Klassen: `Soldat` und `Personalakte`
* Soldaten haben einen `Namen` (String) und eine `Personalakte`
	*  Ein Soldat besitzt 2 Konstruktoren: `Soldat()`, `Soldat(String initName, Personalakte initPersonalakte)`
* Eine Personalakte besteht aus einem `Inhalt` (String) und einer `Personal Nummer` (ganze Zahl)
	* Eine Personalakte besitzt einen Konstruktor: `Personalakte(int initPersNu)`
* Methoden (Verhalten) besitzen diese Klassen erstmal keine, allerdings vergessen Sie nicht die Konstruktoren abzubilden
* Nur Ihre Soldaten Klasse soll später mit der Hauptklasse (`public class Main` und `public void main(String[] args)` kommunizieren können.
	* Die Klasse Soldat und seine Konstruktoren besitzen die Sichtbarkeit: `public`
	* Die Sichtbarkeit einer Personalakte ist: `package`
	* Alle Attribute haben die Sichtbarkeit: `private`

1. Modellieren Sie diese Klassen in UML, beachten Sie die Beziehung zwischen den 2 Klassen (Klassendiagramm:)

2. Überlegen Sie sich sinnvolle Attribut Namen (gerne auf Englisch) / achten Sie dabei besonders auf die Groß- und Kleinschreibung


Antwort:

```






















 ```

### 1.1 (1 Punkt)
* Wie wird ein Konstruktor bezeichnet, der keinen Parameter übergeben bekommt?
	* z.B.: `Soldat()`

Antwort:

>.  
>
>.   
>
>.   
>
>.   
>
>.   
>
>.   
>

## 2 (10 Punkte)
* Gegeben sei ein Objekt: `Erika Musterfrau`.
* Das Objekt entsteht aus der Klasse `Soldat`
* In ihrer Personalakte steht `tadellos`
* Ihre Personal Nummer lautet: `123`

1) Modellieren Sie diese(s) Objekt(e) in UML (Objektdiagramm:)

Antwort:  

>.  
>
>.   
>
>.   
>  
>.   
>  
>.   
>  
>.   
>  
>.  
>  


## 3 (4 Punkte)
Erläutern Sie die Begriffe `Objekt` und `Klasse`. Verwenden Sie dabei bitte folgende Stichwörter: `Zur Laufzeit`; `Zur Zeit der Entwicklung`; `statisches Programmelement`; `dynamisches Programmelement`

Antwort:

>.   
>
>.   
>
>.  
>
>.   
>  


## 4
Gegeben ist folgendes Codefragment:

```java

1 /**
2 *
3 * Enumeration Dienstgrad.
4 * Hier werden ein Teil der moeglichen Dienstgrade festgelegt.
5 *
6 * @author paul
7 */
8 public enum Dienstgrad {
9 UNTEROFFIZIER, OBERGEFREITER, OBERSTABSGEFREITER, GEFREITER;
10 }
```
#### 4.1 (1 Punkt)
* Wie wird der Inhalt in Zeile 1-7 genannt?

Antwort:
```java


```
#### 4.2 (6 Punkte)
* Bilden Sie dieses Enumeration korrekt in UML ab
Antwort:

```












```

# Klassen

## 1.1 (4 Punkte)

* Korrigieren Sie die Fehler des nachstehenden Quellcodes
	* 4 Fehler haben sich eingeschlichen

```java
1  public clas  Soldat
2  
3  	private String name;
4 	private _________________ meinePersonalakte
5  
6  
7  
8  //Hier ist der Platz für Konstruktoren
9  
10 // Hier werden Später Methoden geschrieben/implementiert
11
12 }
```

## 1.2 (10 Punkte)
* Schreiben Sie für die Klasse `Soldat` 2 Konstruktoren
	* Standard Kontruktor (default constructor):
		* Initialisiert den Namen mit `"Erika Musterfrau"
		* Das Attribut `meinePersonalakte` vom Datentyp `Personalakte` wird wie folgt initialisiert:
		*  `this.meinePersonalakte = new Personalakte(123);`
	* Ein Konstruktor mit 2 Parametern: Namen und Personalakte
		* `Soldat(String initName, Personalakte initPersonalakte)`
* Beide Konstruktoren sind öffentlich sichtbar (public)

```

















```

# Methoden

## 1 (10 Punkte)

* Für Ihre Klasse Soldat schreiben Sie bitte eine Ausführende Methode (ohne Rückgabewert) mit folgenden Eigenschaften:
	* Sie ist öffentlich zugänglich (public)
	* Methoden Name: `halloAnAlle`
	* Es werden keine Parameter übergeben
* Die Methode soll auf der Konsole folgendes ausgeben:
	* `Hallo ich heiße (Name des Soldaten).`
	* (Name des Soldaten) soll dabei das Attribut `name` der Klasse Soldat entsprechen
		* z.B.: `Hallo ich heiße Erika Musterfrau`

```














```

# Hauptklasse/Main
## 1 (10 Punkte)
* Erstellen Sie ein Objekt: `erika` mit Hilfe des Standard Konstruktor (default constructor)
* Das Objekt `erika` soll die Methode `halloAnAlle()` aufrufen
* Erstellen Sie ein Objekt: `testSoldat`
	* Überlegen Sie sich selbst: Namen und Personalnummer
	* zur Erinnerung: `Soldat(String initName, Personalakte initPersonalakte)`
* Das Objekt `testSoldat`soll die Methode `halloAnAlle()` aufrufen
* Weisen Sie dem Objekt `testSoldat`, mit Hilfe des Standard Konstruktor, neue Werte zu

```java
public class Main {


	public static void main(String[] args) {
















	}

}
```

# Arrays

Gegeben ist folgende Klasse:

```java
public class MyNumbers {

	int[] myNumbers = { 1, 1, 2, 3, 5, 8, 13 };

	public MyNumbers() {

	}

		public MyNumbers(int[] initNumbers) {

			this.myNumbers = initNumbers;

		}

		public int consoleOutput() {
			for (int i = 0; i < this.myNumbers.length; i++) {
				System.out.println(this.myNumbers[i]);
				}
		}
}
```
## 1 (13 Punkte)
Schreiben Sie eine Methode, die als Rückgabewert eine ganze Zahl zurückgibt. Die Methode ist öffentlich sichtbar (public).
Die Methode Addiert alle Zahlen von `myNumbers` und gibt das Ergebnis zurück. (D.h. 1+1+2+3+5+8+13)

```Java
















```

## 2 (20 Punkte)
* Schreiben Sie eine Methode, die nach einer bestimmten Zahl innerhalb ihres Arrays `myNumbers` sucht.
* Dabei soll die Methode zählen, wie oft die Zahl in dem Array vorkommt. Der Methoden Kopf soll folgend aussehen:

```Java
public int searchNumber(int numberToSearch){

}
```

* Als Rückgabewert wird die Häufigkeit der gesuchten Zahl zurück gegeben.
* Bevor die Methode Den Wert zurückgibt soll sie auf der Konsole folgendes schreiben:

> Die gesuchte Zahl `gesuchte Zahl` wurde `Anzahl der gefundenen Elemente` -Mal gefunden.

```java
public class main {
	public static void main(String[] args) {
		MyNumbers mn = new MyNumbers();
		System.out.println("Rückgabewert der Methode: " + mn.searchNumber(1));
	}
}
```
Ergebnis:
>Die gesuchte Zahl: 1 wurde 2-Mal gefunden.

>Rückgabewert der Methode: 2
