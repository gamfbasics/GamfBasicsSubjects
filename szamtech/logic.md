|   A   |   B   | $$\neg A$$ | $$A \wedge B$$ | $$A \vee B$$ | $$A \rightarrow B$$ | $$A \leftrightarrow B$$ |
| :---: | :---: | :--------: | :------------: | :----------: | :-----------------: | :---------------------: |
| **I** | **I** |    H       |    I           |    I         |    I                |    I                    |
| **I** | **H** |    H       |    H           |    I         |    H                |    H                    |
| **H** | **I** |    I       |    H           |    I         |    I                |    H                    |
| **H** | **H** |    I       |    H           |    H         |    I                |    I                    |

## Ismert ekvivalenciák
1. $$A \leftrightarrow B \equiv (A \rightarrow B) \wedge (B \rightarrow A)$$
2. $$A \rightarrow B \equiv \neg A \vee B $$
3. $$A \wedge A \equiv A,     \quad\quad A \vee A \equiv A \quad (indempotencia) $$
4. $$A \wedge B \equiv B \wedge A,    \quad\quad A \vee B \equiv B \vee A \quad (kommnatitíva)$$
5. $$(A \wedge B) \wedge C \equiv A \wedge (B \wedge C),    \quad\quad (A \vee B) \vee C \equiv A \vee (B \vee C) \quad(szociativák)$$
6. $$(A \vee B) \wedge A \equiv A,    \quad\quad (A \wedge B) \vee A \equiv A \quad (abszorcitivák)$$
7. $$(A \vee B) \wedge C \equiv (A \wedge C) \vee (B \wedge C),   \quad\quad (A\wedge B) \vee C \equiv (A \vee C) \wedge (B \vee C) \quad (disztributivák)$$
8. $$\neg(A \wedge B)  \neg A \vee \neg B, \quad\quad \neg (A \vee B)  \neg A \wedge \neg B$$
9. $$\neg (\neg A) \equiv A$$
10. $$A \wedge \neg A \equiv B \wedge \neg B, \quad\quad A \vee \neg A \equiv B \vee \neg B$$
11. $$A \wedge (B \vee \neg B) \equiv A, \quad\quad A \vee (B \vee \neg B) \equiv B \vee \neg B$$
12. $$A \wedge (B \wedge \neg B) \equiv B \wedge \neg B, \quad\quad A \vee (B \wedge \neg B) \equiv A$$


## Feltételes bizonyítás
$$(a) \quad F_1, F_2, ..., F_n \vDash G \rightarrow H$$

$$(b) \quad F_1, F_2, ..., F_n, G \vDash H$$

## Indirekt bizonyítás
$$(a) \quad F_1, F_2, ..., F_n \vDash G$$

$$(b) \quad \{F_1, F_2, ..., F_n, \neg G\} \text{ nem kielégíthető} $$

## kontrapozízió bizonyítás
$$(a) \quad F_1, F_2, ..., F_n, G \vDash H$$

$$(b) \quad F_1, F_2, ..., F_n, \neg H \vDash \neg G$$
