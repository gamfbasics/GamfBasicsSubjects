# Pointer

- Olyan változótípus, ami egy másik változó **memória helyét tárolja**, nem az értékét
- Pointer-nek is van **saját memóriacíme**
- Pointer típusú változó: <típus>**\*** <név>
- Egy memória helyre mutat
```cpp
int num = 10;
// a `pointer` nem a 10-et tárolja, hanem a `num` memóriacímét
int *pointer = &num;

cout << "num értéke: " << num << endl;
cout << "num címe: " << &num << endl;
cout << "pointer értéke (num címe): " << pointer << endl;
cout << "pointer által mutatott érték: " << *pointer << endl;
cout << "pointer saját memóriacíme: " << &pointer << endl;
```

## Értékadás pointer-rel
```cpp
int num = 10;
int *pointer = &num;
*pointer = 5; // a num értéke 5 lesz
```