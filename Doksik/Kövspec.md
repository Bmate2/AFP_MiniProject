## 1. Áttekintés

> Az alkalmazás célja, hogy szimuláljon egy butított pénztárgép működését. Az alkalmazás HTML+JavaScript+CSS nyelven fog el készülni. A felhasználó által megadott feladatokat fogja elvégezni. A program az elindítása után a felhasználó első teendője: A "NAPNYITÁS", más néven bejelentkezés a pénztárgépbe. A felhasználónak meg kell adni a nyitó készpénz összegét és ez után ennek megfelelő összeget kell be tennie a pénztárgépbe. A felhasználó különböző összegeket vihet be a pénztárgépbe. A bevitt összegeket a pénztárgép elraktározza egy gyűjtőben. A fehasználó, ha végzett az összeg bevitelével, akkor fel kell ajánlania a vevőnek, a fizetés előtt, hogyha van kuponja, akkor használhatja. A végösszegből, kupontól függően különböző nagyságú százalékot von le. A usernek meg kell kérdeznie a vevőt, hogy Euróba, vagy forintba szeretne fizetni, ezt egy "Change to EUR/HUF" gombbal tudja átállítani a felhasználó. A végleges összeg kerüljön kiírásra a képernyőre. A vásárló fizetése után, a felhasználó az "Enter" gomb lenyomásával blokkot nyomtasson a vevő részére. Ha már nincs más feladat, amit el kell látnia a butított pénztárgépnek, akkor kötelezően le kell zárni a pénztárgépet, a "NAPZÁRÁS" gombbal.

## 2. Jelenlegi helyzet leírása

> A megrendelő, egy kasszás boltos eladó, aki nincs megelégedve a jelenlegi pénztárgép működésével, ezért szeretne egy új, jobb felszereltségű gépet, könyebben használható gépet az előző helyére, amivel könnyen végezheti a munkáját.

## 3. Vágyálomrendszer leírása

> Egy minden szakmának megfelelő tudományos számológép lenne a cél. A számológép tudna átváltani valutát Euróra a napi árfolyam alapján. Képes legyen kedvezmények adása esetén %-ot számolni.

## 4. Jelenlegi üzleti folyamatok modellje

> Jelenleg a kasszás kis összegeknél fejszámolást, nagyobb összegknél és kedvezményeknél papíron számítja ki a vásárlás végösszegét. Ez időigényes folyamat, ami a legtöbb esetben reklamációhoz vezet.

## 5. Igényelt üzleti folyamatok modellje

> Egy könnyen értelmezhető és gyors számológép biztosítása, ami felgyorsítja a kiszolgálás idejét és megkönnyíti a kasszás mindennapi munkáját.

## 6. Követelménylista

| Modul       | Id  | Név            | Kifejtés                                                         |
| ----------- | --- | -------------- | ---------------------------------------------------------------- |
| Felület     | 1   | Összeg kiírása | Kiírja a kiszámolt összeget                                      |
| Felület     | 2   | Számok 0-9     | A felhasználó ezen gombok megnyomásával tudja bevinni a számokat |
| Modifikáció | 3   | Összeadás      | A felhasználó álltal beírt számok összeadása                     |
| Modifikáció | 4   | Kivonás        | A felhasználó álltal beírt számok kivonása egymásból             |
| Modifikáció | 5   | Szorzás        | A felhasználó álltal beírt számok szorzata                       |
| Modifikáció | 6   | Osztás         | A felhasználó álltal beírt számok hányadosa                      |
