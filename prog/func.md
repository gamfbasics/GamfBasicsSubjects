# Függvények és makrók

## Függvény

- **Függvény**: Mőveletet végez el és értéket ad vissza
- **Eljárás**: Mőveletet végez el és értéket **NEM** ad vissza, `void` típusú
- Hasonlók a sima változókhoz, csak nem csak egy értéket tartalmaznak, hanem egész program részeket
- A `main()` függvény a program kezdőpontja
  - Függvény, mert értéket ad vissza `return 0;`, ez a hibakód (0, ha sikeresen lefutott a program)

### Függvény létrehozása
```txt
return_típus függvény_neve(paraméterek) {
  // ...
}
```
- **Return_típus**: Visszatérési érték pl.: `int`, `float`, `void`, `struct`
- **Függvény_neve**: Bárminek elnevezhetjük a függvényt, mint ahogy egy változót is
- **Paraméterek**: Opcionálisan adhatunk bemeneti értékeket

> Ha nem akarunk semmilyen értéket visszaadni, akkor arra van a `void` típus. Akkor nem is szükséges kiírni a `return`-t. Ezzel egy Eljárást hozunk létre.

- Ha a függvény / eljárás futása közben egy `return`-höz érünk, akkor nem fog tovább futni és egyből visszaadja az értékét ha van

### Függvény példák
```cpp
void hello() {
  cout << "Hello\n";
}

int kob(int num) {
  return num*num*num;
}

int max(int num1, int num2) {
  if (num1 > num2) return num1;
  else return num2;
}
```
**Használata**
```cpp
hello(); // Kiírja a "Hello" szöveget, mert a kiíratás a függvényben van

cout << max(3, 7) << endl; // Kiírja a 7-et
int maximum = max(-5, -8) // A visszaadott értéket lementhetjük egy változóba
cout << maximum << endl; // Kiírja a -5-öt

kob(2); // Önmagában nem ír ki semmit, csak ha megmondjuk neki
cout << kob(2) << endl; // Kiírja a 8-et
```

---

## Makró

- A makrók nem foglalnak memóriahelyet
- Nincsen típusa
- **Nem kell** utánuk **pontosvessző**t írni
- Hatékonyab, mint egy függvény / eljárás
- A program lefordítása előtt a **preprocess** részben a define-ok be lesznek helyettesítve ahol meg vannak hívval

### Makró létrehozása
```txt
#define MAKRÓ_NÉV(makró_paraméterek) makró_érték
```

- **MAKRÓ_NÉV**: Makrónak a neve, szokás nagy betűkkel írni
- **Makró_paraméterek**: Opcionláisan lehet maramétereket adni
- **Makró_érték**: Olyan érték, vagy kifejezés, ami be lesz helyettesítva a meghívása helyére

### Makró példák
```cpp
#define PI 3.14159
#define LED 2
#define VERSION "v8"
#define OSZT(x,y) x+y
```
**Használata**
```cpp
float terulet = PI * r * r; // Erre lesz lefordítva => 3.14159 * r * r;
cout << VERSION << endl; // Erre lesz lefordítva => cout << "v8" << endl;
cout << OSZT(1, 2.0) << endl; // Erre lesz lefordítva => cout << 1/2 << endl;
cout << OSZT(1+2, 2.0) << endl; // Erre lesz lefordítva => cout << 1+2/2 << endl; (2-t ír ki, nem 1.5-öt)
```