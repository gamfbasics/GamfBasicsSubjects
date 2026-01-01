# Minterm

## Fogalmak
- Hamming távolság
  - 2 bináris érték között hány bit eltérés van
  - 011**0** és 011**1** hamming távolsága 1
  - **0**11**0** és **1**11**1** hamming távolsága 2

## Mintermek
- ![minterm](https://res.cloudinary.com/dpyvopqfn/video/upload/v1766957900/minterm_csosgs.mp4)
- Teljes minterm alak

## Maxterm
- Maxterm tábla
  - Minterm táblában cseréljük fel a 0 és 1-es biteket
  - Cseréljük fel az Változókat a negáltjukra ($$A = \overline{A}$$)
  - Keressünk 2 hatványa oldalhosszúságú 1-es bitű csoportokat
  - Ha $$Q = BD+\overline{B} \text{ } \overline{D}$$, akkor ez lesz a maxterm alak: $$Q = (B + D) * (\overline{B} + \overline{D})$$
  - ![minterm-maxterm](https://res.cloudinary.com/dpyvopqfn/video/upload/v1766945580/minterm-maxterm_ndapvc.mp4)
