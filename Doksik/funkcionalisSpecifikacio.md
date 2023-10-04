## 1. Áttekintés

Az alkalmazás célja, hogy emulálja egy egyszerű pénztárgép működését. Az alkalmazás HTML+JavaScript+CSS nyelveken fog elkészülni, és a felhasználó által megadott műveleteket hajtja végre. A program elindítása után a felhasználó első lépése az "OPEN DAY". A felhasználónak meg kell adnia a nyitó készpénz összegét, majd ezt az összeget be kell helyeznie a pénztárgépbe. A felhasználó különböző összegeket is hozzáadhat a pénztárgéphez. Az összegeket a pénztárgép tárolja egy gyűjtőben. Amikor a felhasználó befejezte az összegek hozzáadását, szóban meg kell kérdeznie a vevőtől, hogy van-e kuponja, és ha igen, akkor felajánlhatja a vásárlónak, hogy használja azt. A végösszeget a kupon alapján különböző százalékokkal csökkentheti. A felhasználónak meg kell kérdeznie a vevőt, hogy euróban vagy forintban szeretne fizetni, és ezt egy "HUF to EUR" gombbal teheti meg. A végleges összeget ki kell írni a képernyőre. A vásárló fizetése után a felhasználó a "Receipt" gombbal blokkot nyomtathat a vásárlónak. Ha nincs más feladat a pénztárgép számára, a "Lezárás" gombbal kötelezően le kell zárni a pénztárgépet.

## 2. Jelenlegi helyzet leírása

A megrendelő egy kiskereskedelmi üzletben dolgozó pénztáros, aki nem kedveli a manuális számolást, és egy hatékonyabb pénztárgépet keres, amely segítheti őt a vásárlások során. Az új pénztárgépnek képesnek kell lennie arra, hogy ha a vásárló rendelkezik kedvezménykuponnal, akkor az a kuponnal járó kedvezményes árat is könnyedén kiszámolja.

## 3. Követelménylista leírása

| Modul       | Id  | Név              | Kifejtés                                                           |
| ----------- | --- | ---------------- | ------------------------------------------------------------------ |
| Felület     | 1   | Eredmény kiírása | Kiírja a kiszámolt eredményt                                       |
| Felület     | 2   | Számok 0-9       | A felhasználó ezen gombok megnyomásával tudja bevinni a számokat   |
| Modifikáció | 3   | Összeadás        | A felhasználó álltal beírt számok összeadása                       |
| Modifikáció | 4   | Kivonás          | A felhasználó álltal beírt számok kivonása                         |
| Modifikáció | 5   | Százalék         | A felhasználó álltal beírt számnak egy bizonyos százalékát írja ki |
| Modifikáció | 6   | Euróra váltás    | A kiszámolt termékek össszárát tudja átváltani Euró pénznembe      |
| Modifikáció | 7   | Forintra váltás  | A kiszámolt termékek össszárát tudja átváltani Forint pénznembe    |
| Modifikáció | 8   | Nyugta nyomtatás | A vásárlás összegéről nyugtát nyomtat a vevő részére               |
| Modifikáció | 9   | Napi nyitó       | A felhasználó álltal beírt összeggel kezdett az adott napon        |

## 4. Jelenlegi üzleti folyamatok modellje

Jelenleg a kasszás boltos eladó manuálisan számol kisebb értékű vásárlások esetén, míg nagyobb összegű vásárlásoknál vagy kedvezmények alkalmazása esetén papíron végez számításokat a vásárlás teljes összegének kiszámításához. Ez a folyamat nagy időráfordítást igényel, és gyakran eredményez hibákat, ami további reklamációkhoz vezethet. Az eladó jelenlegi módszere nem csak időigényes, hanem könnyen hibázható is, ami nemcsak a bolt hatékonyságát csökkenti, hanem a vásárlók elégedettségét is csökkentheti. Az új pénztárgép bevezetése lehetővé tenné, hogy az eladó gyorsabban és pontosabban számolja ki a vásárlások végső összegét, és akár automatikusan érvényesítse a kedvezményeket is, ami javítaná az ügyfélszolgálat minőségét és növelné a bolt hatékonyságát.

## 5. Igényelt üzleti folyamatok modellje

Az igényelt, egyszerűsített pénztárgép olyan eszköz lenne, amely könnyen érthető és gyors szolgáltatást nyújtana. Ezáltal a boltban történő vásárlások folyamata jelentősen felgyorsulna, ami mind a vásárlók, mind pedig a kasszások számára kényelmesebb élményt nyújtana. Az egyszerűsített pénztárgép segítségével a kasszások gyorsabban és hatékonyabban tudnák kiszolgálni a vásárlókat. Az intuitív felület és a könnyen kezelhető funkciók lehetővé tennék, hogy a kasszások gyorsan és pontosan számolják ki a vásárlások végösszegét, valamint alkalmazhassák a kedvezményeket is. Ez a változás nemcsak a vásárlásokat tenné zökkenőmentesebbé, de a kasszások mindennapi munkáját is megkönnyítené. Az egyszerűsített pénztárgép alkalmazása segítene minimalizálni a hibák lehetőségét, csökkentve ezzel a reklamációk számát és javítva az ügyfélszolgálat minőségét.

## 6. Használati esetek

Az alkalmazásunk két használati esettel rendelkezik: Az első, ami a napi nyitás előtt van, csak abból áll hogy meg kell adni, hogy mennyi pénzzel kezdte az adott napot a felhasználó. A második eset amikor a usernek hozzáférése van az összes funkcióhoz a pénztárgépben.

## 7. Képernyőtervek

![image](https://github.com/Bmate2/AFP_MiniProject/assets/145013912/9482faae-c93b-41ab-b4df-77d250d6f8b9)

## 8. Forgatókönyv

A felhasználó megnyitja a programot és egy napnyitó gomb fogja fogadni, amit megnyomva felugró ablakként jelenik meg ahova beviheti azt az összeget amivel inditja a napot. A napnyitás elvégzésével feloldódik a pénztárgép, és kezdheti a munkát. A nap végén lezárja a kasszát egy nap zárása gombbal.

## 9. Fogalomszótár

user - felhasználó
OPEN DAY - Napnyitás
