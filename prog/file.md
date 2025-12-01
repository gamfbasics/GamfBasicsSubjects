# Fájl kezelés

> Fájlkezeléshez be kell tenni az `fstream` (file stream) állományt a programunk tetejére
```cpp
#include <fstream>
```

## Fájlba írás
- Olvasáskor `ofstream` típust kell használni
- Amennyiben nem létezik a fájl az adott helyen, akkor létrehozza (ha van engedélye)
```cpp
ofstream myFile("file_helye.txt");
```
- A fájlba írás a `cout` kiiratáshoz hasonlóan működik `<<` operátorral sorolhatjuk fe az adatokat, amiket be akarink írni
```cpp
myFile << "Hello world";
```
- Ha már nem használjuk a fájlt, akkor zárkul le a `close` fuggvénnyel
```cpp
myFile.close();
```

**Teljes program**
```cpp
#include <fstream>

using namespace std;

int main() {
  ofstream myFile("file_helye.txt");

  myFile << "Hello world\n";
  myFile << "Goodbye" << " world";

  myFile.close();

  return 0;
}
```


---

## Fájlbol olvasás
- `ifstream` típust kell használni olvasáskor
```cpp
ifstream myFile("file_helye.txt");
```
- File sorainak kiírása
> Ehhez ajánlott include-olni a string állományt `#include <string>`
>
> While cikust használunk, mert előre nem tudjuk hány soros a fájl és addig fut, ameddig nem érünk a fájl végére (**eof = end of file**)
>
> Példa fájl:
> ```txt
> Moldova 2
> Fehéroroszország 1
> Magyarország 8
> ```
```cpp
string sor;
while(!myFile.eof()) {
  getline(file, sor);
  cout << sor << endl;
}
```
- Alternatíva, ha a sorok egyes szóközzel elválasztott értékei szeretnénk
```cpp
while(!myFile.eof()) {
  string orszag;
  int hely;
  myFile >> orszag >> hely; // Így külön válzotókban vannak az egyes értékek. Ezt elmenthetjük tömbbe, vagy struct-ba
  cout << orszag << " " << hely << endl;
}
```

- A legvégén, ha már nem nyúlunk a fájl-hoz, akkor zárjuk is be
```cpp
myFile.close();
```

**Teljes program**
```cpp
#include <iostream>
#include <fstream>
#include <string>

using namespace std;

int main() {
  ifstream myFile("file_helye.txt");

  while(!myFile.eof()) {
    getline(myFile, sor);
    cout << sor << endl;
    // VAGY
    // string orszag;
    // int hely;
    // myFile >> orszag >> hely;
    // cout << orszag << " " << hely << endl;
  }

  myFile.close();

  return 0;
}
```
