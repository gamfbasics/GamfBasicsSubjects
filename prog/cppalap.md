# C++ Alapok

## Hello world program
```cpp
#include <iostream> // input-output kezelés, avagy konzolra kiírás és konzolból olvasás
using namespace std;

int main() { // Itt lépünk be a programba, itt kezdődik a program futása
  cout << "Hello, world" << endl; // Console OUTputjába kiíratjuk a "Hello, world" szöveget és rakunk egy sortörést
  return 0; // Program kilépési kódja, a 0 azt jelenti, hogy hibátlanul lefutott
}
```

## Változók
- A Változók Különböző adatokat tudnak tárolni pl.: egész / tört számok, karakterek...
- Alap típusok
- | Típus    | Mit tárol  | Példa | Mennyi bitet foglal |
  | -------- | ---------- | ----- | ------------------- |
  | `int`    | Egész szám | 21    | 32 bit (4 byte)     |
  | `float`  | Tört szám  | 1.5   | 32 bit (4 byte)     |
  | `double` | Tört szám  | 3.14  | 64 bit (8 byte)     |
  | `char`   | Karakter   | 'a'   | 8 bit (1 byte)      |
- Változó létrehozása 
  - Értékadás nélkül <**típus**> <**változó neve**>**;** pl.: int i;
  - Értékadással <**típus**> <**változó neve**> = <**érték**>**;** pl.: int i = 10;
```cpp
#include <iostream>
using namespace std;

int main() {
  // egész szám (int) változó "i" néven
  int i;
  // értékadás
  i = 21;
  // "i" változó kiírása
  cout << i << endl;
  return 0;
}
```
- A változó nevek
  - Nem lehetnek kulcsszavak pl.: int, for, if...
  - Nem kezdődhetnek számmal vagy speciális karakterekkel pl.: `!`, `)`, `3`
  - Egyedinek kell lennie

```cpp
#include <iostream>
using namespace std;

int main() {
  // egész szám (int) változó "i" néven
  int darab = 21;

  // lebegő pontos szám
  float homerseklet = 15.8;

  // tizedes pontos szám
  double pi = 3.14;

  // karakter
  char betu = 'a';
  
  // Kiírás
  cout << darab << endl;
  cout << homerseklet << endl;
  cout << pi << endl;
  cout << betu << endl;
  return 0;
}
```

## Operátorok / műveletek

```cpp
int szam = 2;

// Értékadő operátor, a szam változó értékének 4-et adunk
szam = 4; 

// Összehasonlító okerátor, megegyezik e a szam változó értéke a 4-gyel
szam == 4;

// Tagadó összehasonlító okerátor, a szam változó értéke nem egyenlő 4-gyel
szam != 4; 

// Relációs operátorok
szam < 4;
szam <= 4;
szam > 4;
szam >= 4;

// incrementáló operátorok, a szam változó értékét növeli 1-gyel
szam++; // postfix
++szam; // prefix

// Decrementáló operátorok, a szam változó értékét csökkenti 1-gyel
szam--; // postfix
--szam; // prefix
```