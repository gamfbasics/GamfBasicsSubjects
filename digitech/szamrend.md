# Számrendszerek

## Főbb számrendszerek
| Neve                  | Számai                                         | Jelölése |
| --------------------- | -------------------------------------------    | -------- |
| Bináris (2-es)        | 0, 1                                           | b        |
| Oktális (8-as)        | 0, 1, 2, 3, 4, 5, 6, 7                         | o        |
| Decimális (10-es)     | 0, 1, 2, 3, 4, 5, 6, 7, 8, 9                   | d        |
| Hexadecimális (16-es) | 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F | h        |

<!-- - Bináris (2-es)        [ 0, 1 ]
- Oktális (8-as)        [ 0, 1, 2, 3, 4, 5, 6, 7 ]
- Decimális (10-es)     [ 0, 1, 2, 3, 4, 5, 6, 7, 8, 9 ]
- Hexadecimális (10-es) [ 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, F ] -->


## Számrendszer átváltások

### Decimálisba átváltás

$$234_d = 2*10^2 + 3*10^1 + 4*10^0 = 234_d$$

$$234_h = 2*16^2 + 3*16^1 + 4*16^0 = 564_d$$

$$0101_b = 0*2^3 + 1*2^2 + 0*2^1 + 1*2^0 = 5_d$$

### Decimálisból átváltás
Decimálisból más számrendszerbe úgy váltunk át, hogy az adott alap számaival folyamatosan elosztjuk a számot, és a maradékokból olvassuk ki a számjegyeket.
A maradékokat fordított sorrendben összeírva kapjuk meg a keresett számrendszerbeli alakot.

|   | Maradék | Osztás |
| - | -       | -      |
| 5 | 1       | /2     |
| 2 | 0       | /2     |
| 1 | 1       | /2     |
| 0 | 0       | -      |


$$5_d = 0101_b$$

|     | Maradék | Osztás |
| -   | -       | -      |
| 564 | 4       | /16    |
| 35  | 3       | /16    |
| 2   | 2       | /16    |
| 0   | 0       | -      |

$$564_d = 234_h$$

### Konverziók

$$1010_b = A_h = 10_d$$

$$1111\text{ }1111_b = FF_h = 255_d$$
