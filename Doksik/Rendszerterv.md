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
|Program                  |Alapfunkciók elkészítése                |         3 |             10|                      12|                16|                   12|
|Program                  |Tesztelés                               |         4 |             4 |                      4 |                5 |                   5 |

### 2.4 Mérföldkövek:
   * Prototípus átadása: 2023.10.02. 12:30

## 3. Üzleti folyamatok modellje:

Az üzleti folyamatok modelljének elkészítése során célszerű ábrák és leírások segítségével bemutatni, hogyan zajlanak le az egyes tevékenységek és folyamatok a rendszerben. Az alábbiakban néhány példa található az üzleti folyamatok modelljének kialakításához:

## 3.1. Napnyitási folyamat:

Cél: Az adott munkanap pénzmennyiségének eltárolása és a pénztárgép felületére való továbblépés.

Folyamat:

 1.1. 
 * Felhasználó bejelentkezik a rendszerbe.
 1.2. 
 * A felhasználó kiválasztja a "Napnyitás" opciót.
 1.3. 
 * A rendszer lehetővé teszi a felhasználó számára a pénzmennyiség rögzítését a műszak kezdésekor.
 1.4. 
 * A rendszer engedélyezi a felhasználót, hogy továbblépjen a pénztárgép felületére.

## 3.2. Tranzakció végrehajtás folyamata:

Cél: Tranzakciók végrehajtása pénzhasználattal.

Folyamat:

 1.1. 
 * Felhasználó választ egy árucikket a kínálatból.
 1.2.
 * A rendszer lehetőséget ad az árucikk mennyiségének és értékének megadására (HUF).
 1.3.
 * Ha a vevő nagyobb összeget ad át, mint amennyi a tranzakció értéke, a rendszer kiszámolja és visszaadja a visszajárót.
 1.4.
 * A rendszer rögzíti a tranzakciót és a pénzforgalmat.

## 3.3. Napzárás folyamata:

Cél: Az adott nap pénzforgalmának logolása és átláthatóan történő tárolása.

Folyamat:

1.1. 
 * Felhasználó bejelentkezik a rendszerbe.
1.2. 
 * A felhasználó választja a "Napzárás" opciót.
1.3. 
 * A rendszer összegzi az adott nap során történt tranzakciókat és pénzmennyiségeket.

Ezek csupán példák az üzleti folyamatok modelljének elkészítéséhez. A valóságban részletes folyamatokat és ábrákat is érdemes készíteni, hogy pontosan látható legyen, hogyan működik a rendszer a felhasználók szemszögéből.

## 4. Követelmények
   * Napnyitási felület, mely tartalmazza az adott munkanap pénzmenniységének eltárolási lehetőségét a műszak kezdésekor, és továbblépést biztosít a pénztárgép felületére
   * Napzárás funkció az adott nap pénzforgalmának logolására, a napokat egy fájlban, átláthatóan feltűntetve
   * Árucikkek összegének inicializálása
   * Árucikkek összegeinek inicializálása után e-összegek párhuzamos idejőbeli összegzése
   * Valutaváltás, előzetes HUF érték eltárolása
   * Tranzakció végrehajtás funkció, az érték eltárolásával (HUF)
   * Vevő által nagyobb összeg átadása esetén visszajáró kiszámolása
   * Nyugta kinyomtatása, egyidőben a tranzakció NAV felé való közlése (HUF)

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

Az absztrakt domain modell célja, hogy általánosan és absztrakt módon ábrázolja a rendszer fő komponenseit, entitásait és azok közötti kapcsolatokat.

* Felhasználók: Felhasználók, akik a rendszert használják.
* Felhasználók jogosultságokkal rendelkeznek a pénztár-nyitás és tranzakciók végrehajtása terén.

Napnyitási Felület:
* Az adott munkanap pénzmennyiségének eltárolására szolgáló felület
* Lehetővé teszi a munkanap kezdeti pénzmennyiségének rögzítését.
* Engedélyezi a továbblépést a pénztárgép felületére.

Pénztárgép Felület: 
* Az alapfunkciók végrehajtásara szolgáló felület.
* Lehetővé teszi tranzakciók létrehozását és azok rögzítését.
* Számolja és kezeli a visszajárót.

Tranzakciók:
* Az eladások vagy vásárlások rögzített eseményei.
* Tartalmazzák az árucikkek, mennyiségek és értékek adatait.
* A tranzakciókhoz kapcsolódik a visszajáró összeg.

Ez egy egyszerű példa az absztrakt domain modellre. A valoságban a rendszer sokkal komplexebb lehet.

## 8. Architekturális terv

## 9. Alkalmazás Réteg:

### Webes Felület (Frontend):
* Az alkalmazás felhasználói felülete, amelyet a böngészőből érhetnek el a felhasználók.
* Minimalista és intuitív tervezés a könnyű használhatóság érdekében.
* A webes felület HTML, CSS és JavaScript technológiák segítségével készül.

### Kliensoldali Logika (Backend):
* A frontend-en futó JavaScript alkalmazás, amely felelős a felhasználói interakciók kezeléséért.
* Kommunikál a szerverrel API-hívások segítségével.

### Üzleti Logika Réteg:

Szerveroldali Alkalmazás:
* Ezen a rétegen fut az üzleti logika és a rendszer működésének alapja.
* Kezeli a tranzakciók, az árucikkek, a pénzkezelés és a napzárás,nyitás folyamatait.

#### A program elérése, kezelése
A programot a HTML kiterjesztésű fájllal lehet indítani, ami megnyitja online a programot.

## 10. Implementációs terv
A Webes felület főként HTML, CSS, és Javascript nyelven fog készülni.
Ezeket a technológiákat, amennyire csak lehet, külön fájlokba írva készítjük, és
úgy fogjuk egymáshoz csatolni a jobb átláthatóság, könnyebb változtathatóság,
és könnyebb bővítés érdekében.

## 11. Tesztterv

A tesztelések célja a rendszer és komponensei funkcionalitásának teljes vizsgálata,
ellenőrzése a rendszer által megvalósított üzleti szolgáltatások verifikálása.
A teszteléseket a fejlesztői csapat minden tagja elvégzi.

### Tesztesetek

 | Teszteset | Elvárt eredmény | 
 |-----------|-----------------| 
 | ... | ... |

### A tesztelési jegyzőkönyv:

**Tesztelő:** A csapat tagjai

**Tesztelés dátuma:** 2023.10.04

Tesztszám | Rövid leírás | Várt eredmény | Eredmény | Megjegyzés
----------|--------------|---------------|----------|-----------
Teszt #01 | Napnyitás | A felhasználó a napi kezdő egyenleg megadásával aktiuválja a pénztárgép felületét.  | A felhasználó sikeresen felvitte az adatokat, a rendszer engedélyezte a pénztár használatát. | Nem találtam problémát.
Teszt #02 | Gombok funkciói | Az összes gomb reagál a felhasználó által adott impulzusokra  | A felhasználó az összes gomb egymás utáni végigpróbálására mindegyik gomb reagál | Nem találtam problémát
Teszt #03 | Megjelenítő | A felhasználó számára fontos számadatok és műveleti jelek megjelennek a kijelzőn | A kijelző megjeleníti az adatokat | Nem találtam hibát
Teszt #04 | Műveletek | A felhasználó a bevitt adatokkal és műveleti jelek segítségével az "egyenlő" jel megnyomásával a kijelzőn a helyes érték jelenik meg | A program helyesen számol | Nem találtam hibát
Teszt #05 | Valutaváltás | A vásárló összes árucikkének felvitele után a végösszeget lehessen euróra váltani, vagy adott esetben euróról vissza | Mindkét esetben helyes érték jelenik meg a kijelzőn az adott valutával kapcsolatban | Mindenképpen be kell vinni az adatot az "egyenlő" jellel, hogy e-funkció működjön 

## 12. Telepítési terv
Szoftver telepítési terv: 
Nincs szükség külön telepítésre, a szoftver bármely webböngésző indításával futtatható.

## 13. Karbantartási terv

Figyelembe kell venni a felhasználó által jött visszajelzést is a programmal kapcsolatban.
Ha hibát talált, mielőbb orvosolni kell, lehet az:
*	Működéssel kapcsolatos
*	Kinézet, dizájnnal kapcsolatos