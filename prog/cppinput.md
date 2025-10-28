# Bemenet kezelés

- Bementetet a konzolból a `cin` utatítással kaphatunk meg
- Az `iostream` állományt bele kell rakni

```cpp
#include <iostream>
using namespace std;

int main() { 
  // szám bekérése
  int szam;
  cin >> szam;
  cout << szam << endl;

  // szöveg bekérése (ha szóközt tartalmaz, akkor csak a szóköz előtti részét kapjuk meg)
  char nev[25];
  cin >> nev;
  cout << nev << endl;

  // Ha szóközt is akarunk tárolni akkor a 'cin.getline' függvényt használjuk
  // Első paramétere a változó ahova tároljuk, a második, hogy mennyi karaktert fogad el max
  cin.getline(nev, 25);
  cout << nev << endl;
  return 0;
}
```