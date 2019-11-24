-Seite 7

**Name:**

# Arrays

Gegeben ist folgende Klasse:

```java
public class MyNumbers {

	int[] myNumbers = { 1, 1, 2, 3, 5, 8, 13 };

	public MyNumbers() {
    //default constructor
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
