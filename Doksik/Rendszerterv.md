rendszerterv.md
# Rendszerterv
## 1. A rendszer célja
A rendszer célja, hogy a felhasználó bolti körülmények között tudjon tranzakciókat végrehajtani, pénzzel dolgozni. Fontos, hogy a felhasználó könnyen el tudjon igazodni a felületen, ezért minimalista felhasználói felületet kap a program. A felületen nem lehet számlázási folyamatokat végrehajtani, amíg a felhasználó el nem végzi a napi pénztár-nyitási folyamatot. A rendszer webes felületen elérhető. Mivel az alkalmazás csak webes felületen lesz elérhető, nem célunk különböző operációs rendszerekre való fejlesztése, optimalizálása. 

## 2. Projektterv

### 2.1 Projektszerepkörök, felelőségek:
   * Scrum masters: Tajti Tibor
   * Product owner: Tajti Tibor
     
### 2.2 Projektmunkások és felelőségek:
   * Fejlesztők és tesztelők: a csapat tagjai
     
### 2.3 Ütemterv:

|Funkció                  | Feladat                                | Prioritás | Becslés (óra) | Aktuális becslés (óra) | Eltelt idő (óra) | Becsült idő (óra) |
|-------------------------|----------------------------------------|-----------|---------------|------------------------|------------------|---------------------|
|Követelmény specifikáció |Megírás                                 |         1 |             1 |                      1 |                2 |                   1 |             
|Funkcionális specifikáció|Megírás                                 |         1 |             1 |                      1 |                2 |                   1 |
|Rendszerterv             |Megírás                                 |         1 |             4 |                      4 |                5 |                   4 |
|Program                  |Képernyőtervek elkészítése              |         2 |             1 |                      1 |                3 |                   2 |
|Program                  |Prototípus elkészítése                  |         3 |             8 |                      8 |                8 |                   8 |
|Program                  |Alapfunkciók elkészítése                |         3 |             10 |                      12 |                16 |                   12 |
|Program                  |Tesztelés                               |         4 |             4 |                      4 |                5 |                   5 |

### 2.4 Mérföldkövek:
   * Prototípus átadása: 2023.10.02. 12:30

## 3. Üzleti folyamatok modellje

## 4. Követelmények
   * Napnyitási felület, mely tartalmazza az adott munkanap pénzmenniységének eltárolási lehetőségét a műszak kezdésekor, és továbblépést biztosít a pénztárgép felületére
   * Napzárás funkció az adott nap pénzforgalmának logolására, a napokat egy fájlban, átláthatóan feltűntetve
   * Árucikkek összegének inicializálása
   * Árucikkek összegeinek inicializálása után e-összegek párhuzamos idejőbeli összegzése
   * Valutaváltás, előzetes HUF érték eltárolása
   * Tranzakció végrehajtás funkció, az érték eltárolásával (HUF)
   * Vevő által nagyobb összeg átadása esetén visszajáró kiszámolása
   * Nyugta kinyomtatása, egyidőben a tranzakció NAV felé való közlése (HUF)

### Funkcionális követelmények

| ID | Megnevezés | Leírás |
| --- | --- | --- |
| K1 | ... | ... |

### Nemfunkcionális követelmények

A felhasználó nem férhet hozzá az ideiglenes értéktároláshoz, azokat meg nem változtathatja.

## 5. Funkcionális terv

### 5.1 Rendszerszereplők
Felhasználó

### 5.2 Menühierarchiák
   * Napnyitás
      * Kasszában lévő nyitóegyenleg 
      * Belépés

   * Munkafelület

## 6. Fizikai környezet
   * Az alkalmazás web platformra készül
   * Van tűzfal a hálózaton és minden portot is engedélyez

### Vásárolt softwarekomponensek és külső rendszerek
   * Nincsenek megvásárolt komponensei

### Fejlesztő eszközök
   * HTML+CSS
   * JavaScript

### 7. Abszrakt domain modell

## 8. Architekturális terv

### Webszerver

### Adatbázis rendszer

### A program elérése, kezelése

## 10. Implementációs terv

## 11. Tesztterv

A tesztelések célja a rendszer és komponensei funkcionalitásának teljes vizsgálata,
ellenőrzése a rendszer által megvalósított üzleti szolgáltatások verifikálása.
A teszteléseket a fejlesztői csapat minden tagja elvégzi.
Egy teszt eredményeit a tagok dokumentálják külön fájlokba.

### Tesztesetek

 | Teszteset | Elvárt eredmény | 
 |-----------|-----------------| 
 | ... | ... |

### A tesztelési jegyzőkönyv kitöltésére egy sablon:

**Tesztelő:** Vezetéknév Keresztnév

**Tesztelés dátuma:** Év.Hónap.Nap

Tesztszám | Rövid leírás | Várt eredmény | Eredmény | Megjegyzés
----------|--------------|---------------|----------|-----------
például. Teszt #01 | Regisztráció | A felhasználó az adatok megadásával sikeresen regisztrálni tud  | A felhasználó sikeresen regisztrált | Nem találtam problémát.
... | ... | ... | ... | ...

## 12. Telepítési terv

Fizikai telepítési terv: 

Szoftver telepítési terv: 

## 13. Karbantartási terv

Fontos ellenőrizni:
...

Figyelembe kell venni a felhasználó által jött visszajelzést is a programmal kapcsolatban.
Ha hibát talált, mielőbb orvosolni kell, lehet az:
*	Működéssel kapcsolatos
*	Kinézet, dizájnnal kapcsolatos