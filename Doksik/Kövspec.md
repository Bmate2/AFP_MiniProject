## 1. Áttekintés

Az alkalmazás célja, hogy szimuláljon egy butított pénztárgép működését. Az alkalmazást webes felületen szeretnénk használni. A felhasználó által megadott feladatokat fogja elvégezni. A program az elindítása után a felhasználó első teendője: A "OPEN DAY", más néven bejelentkezés a pénztárgépbe. A felhasználónak meg kell adni a nyitó készpénz összegét és ez után ennek megfelelő összeget kell be tennie a pénztárgépbe. A felhasználó különböző összegeket vihet be a pénztárgépbe. A bevitt összegeket a pénztárgép elraktározza egy gyűjtőben. A fehasználó, ha végzett az összeg bevitelével, akkor fel kell ajánlania a vevőnek, a fizetés előtt, hogyha van kuponja, akkor használhatja. A végösszegből, kupontól függően különböző nagyságú százalékot von le. A usernek meg kell kérdeznie a vevőt, hogy Euróba, vagy forintba szeretne fizetni, ezt egy "Change to EUR" gombbal tudja átállítani a felhasználó. A végleges összeg kerüljön kiírásra a képernyőre. A vásárló fizetése után, a felhasználó az "Reciept" gomb lenyomásával blokkot nyomtasson a vevő részére. Ha már nincs más feladat, amit el kell látnia a butított pénztárgépnek, akkor kötelezően le kell zárni a pénztárgépet, a "CLOSE DAY" gombbal.

## 2. Jelenlegi helyzet leírása

> A megrendelő egy kiskereskedelmi üzletben dolgozó pénztáros, aki nincs megelégedve a jelenlegi pénztárgépek működésével, ezért szeretne egy új, jobb felszereltségű, könyebben használható prototípust az előző helyére, amivel könnyebben végezheti a munkáját. A legnagyobb problémája, azzal van,  hogy gyakran lefagynak a pénztárgépek, mert túl sok adat halmozódik fel bennük. A megoldás az lenne, ha gyorsabb, kevesebb gombnyomással működő pénztárgépeket használnának, hogy gyorsabban haladhassanak a sorok és ez által ne terhelődjenek le a pénztárgépek.

## 3. Vágyálomrendszer leírása

A project célja, egy olyan egyszerű pénztárgép, amivel megkönyíthetjük a kasszánál dolgozó alkalmazottak életét. A tervezett gépünk könnyen kezelhető, kevés gombnyomást igénylő szerkezet. Könnyen elvégezhető a pénztárgépen a kötelező napi nyitás, illetve napi zárás. A vevő kiszolgálásnál az összegek könnyen felvihetők a pénztárgépbe. A felvitel után lehetőség nyílik arra, hogy a vevő használjon különböző kupont a fizetés előtt. A külföldi vevők számára biztosítunk eurós fizetési lehetőséget is. Az összeg felvitele után egy gombnyomással átváltható a forintban kiszámolt végösszeg euróba. Ha kifizette a vevő a vásárolt termékeket, a pénztárgép egy billentyű lenyomásával blokkot nyomtat a vevő számára a vett termékekről és azok árairól.

## 4. Jelenlegi üzleti folyamatok modellje

Felhasználói funkció - A felhasználó a napi nyitás elvégezte után, hozzáférést kap az egész pénztárgép funkcióihoz.
Ez után feltudja vinni a vevő által vásárolt termékek összegét a pénztárgépbe, majd a vásárlás végeztével blokkot tud nyomtatni. A nap végén pedig a nap végi zárást követően kezdődik újra ez a folyamat.

## 5. Igényelt üzleti folyamatok modellje

Egy könnyen értelmezhető és gyors pénztárgép biztosítása, ami felgyorsítja a kiszolgálás idejét és megkönnyíti a kasszás mindennapi munkáját.

## 6. Követelménylista

| Modul       | Id  | Név            | Kifejtés                                                                         |
| ----------- | --- | -------------- | -------------------------------------------------------------------------------- |
| Felület     | 1   | Összeg kiírása | Kiírja a kiszámolt összeget                                                      |
| Felület     | 2   | Számok 0-9     | A felhasználó ezen gombok megnyomásával tudja bevinni a számokat                 |
| Felület     | 3   | Funkciógombok  | A felhasználó ezen gombok megnyomásával tudja elvégezni a bizonyos műveleteket   |
| Modifikáció | 4   | Összeadás      | A felhasználó álltal felvitt termékek árát össze adja                            |
| Modifikáció | 5   | Kivonás        | A felhasználó álltal fevitt termékek árát kivonja egymásból                      |
| Modifikáció | 6   | Számolás       | A felhasználó a felvitt adatokat elvégezteti a programmal                        |
| Modifikáció | 7   | NAPNYITÁS      | A felhasználónak fel kell vinnie a napi kezdő összeget                           |
| Modifikáció | 8   | NAPZÁRÁS       | A felhasználónak fel kell vinnie a napi záró összeget                            |
| Modifikáció | 9   | RECIEPT        | A felhasználó blokkot nyomtat a vevő számára                                     |
| Modifikáció | 10  | Change to EUR  | A felhasználó át váltja a forintban lévő összeget euróba                         |
| Modifikáció | 11  | Change to HUF  | A felhasználó át váltja az euróban lévő összeget forintba                        |
| Modifikáció | 12  | Kupon          | A végösszegből százalékosan levon bizonyos mennyiségű összeget                   |

