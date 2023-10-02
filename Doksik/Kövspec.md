## 1. Áttekintés

Az alkalmazás célja, hogy szimuláljon egy butított pénztárgép működését. Az alkalmazás HTML+JavaScript+CSS nyelven fog el készülni. A felhasználó által megadott feladatokat fogja elvégezni. A program az elindítása után a felhasználó első teendője: A "NAPNYITÁS", más néven bejelentkezés a pénztárgépbe. A felhasználónak meg kell adni a nyitó készpénz összegét és ez után ennek megfelelő összeget kell be tennie a pénztárgépbe. A felhasználó különböző összegeket vihet be a pénztárgépbe. A bevitt összegeket a pénztárgép elraktározza egy gyűjtőben. A fehasználó, ha végzett az összeg bevitelével, akkor fel kell ajánlania a vevőnek, a fizetés előtt, hogyha van kuponja, akkor használhatja. A végösszegből, kupontól függően különböző nagyságú százalékot von le. A usernek meg kell kérdeznie a vevőt, hogy Euróba, vagy forintba szeretne fizetni, ezt egy "Change to EUR/HUF" gombbal tudja átállítani a felhasználó. A végleges összeg kerüljön kiírásra a képernyőre. A vásárló fizetése után, a felhasználó az "Enter" gomb lenyomásával blokkot nyomtasson a vevő részére. Ha már nincs más feladat, amit el kell látnia a butított pénztárgépnek, akkor kötelezően le kell zárni a pénztárgépet, a "NAPZÁRÁS" gombbal.

## 2. Jelenlegi helyzet leírása

> A megrendelő, egy árúház vezető, aki nincs megelégedve a jelenlegi pénztárgépek működésével, ezért szeretne egy új, jobb felszereltségű, könyebben használható prototípust az előző helyére, amivel könnyebben végezhetik a munkát az alkalmazottjai. A legnagyobb problémája, azzal van, hogy túl nagyok a sorok a kasszáknál, nehéz a haladás, ezért kevesebben vásárolnak. A másik problémája, hogy gyakran lefagynak a pénztárgépek, mert túl sok adat halmozódik fel bennük. A megoldás az lenne, ha gyorsabb, kevesebb gombnyomással működő pénztárgépeket használnának, hogy gyorsabban haladhassanak a sorok, ne terhelődjenek le a pénztárgépek annyira és ez által többen vásároljanak. 

## 3. Vágyálomrendszer leírása

A project célja, egy olyan egyszerű pénztárgép, amivel megkönyíthetjük a kasszánál dolgozó alkalmazottak életét. A tervezett gépünk könnyen kezelhető, kevés gombnyomást igénylő szerkezet. Könnyen elvégezhető a pénztárgépen a kötelező napi nyitás, illetve napi zárás. A vevő kiszolgálásnál az összegek könnyen felvihetők a pénztárgépbe. A felvitel után lehetőség nyílik arra, hogy a vevő használjon különböző kupont a fizetés előtt. A külföldi vevők számára biztosítunk eurós fizetési lehetőséget is. Az összeg felvitele után egy gombnyomással átváltható a forintban kiszámolt végösszeg euróba. Ha kifizette a vevő a vásárolt termékeket, a pénztárgép egy billentyű lenyomásával blokkot nyomtat a vevő számára a vett termékekről és azok árairól.

## 4. Jelenlegi üzleti folyamatok modellje

Jelenleg a kasszás kis összegeknél fejszámolást, nagyobb összegknél és kedvezményeknél papíron számítja ki a vásárlás végösszegét. Ez időigényes folyamat, ami a legtöbb esetben reklamációhoz vezet.

## 5. Igényelt üzleti folyamatok modellje

Egy könnyen értelmezhető és gyors számológép biztosítása, ami felgyorsítja a kiszolgálás idejét és megkönnyíti a kasszás mindennapi munkáját.

## 6. Követelménylista

| Modul       | Id  | Név            | Kifejtés                                                         |
| ----------- | --- | -------------- | ---------------------------------------------------------------- |
| Felület     | 1   | Összeg kiírása | Kiírja a kiszámolt összeget                                      |
| Felület     | 2   | Számok 0-9     | A felhasználó ezen gombok megnyomásával tudja bevinni a számokat |
| Modifikáció | 3   | Összeadás      | A felhasználó álltal beírt számok összeadása                     |
| Modifikáció | 4   | Kivonás        | A felhasználó álltal beírt számok kivonása egymásból             |
| Modifikáció | 5   | Szorzás        | A felhasználó álltal beírt számok szorzata                       |
| Modifikáció | 6   | Osztás         | A felhasználó álltal beírt számok hányadosa                      |
