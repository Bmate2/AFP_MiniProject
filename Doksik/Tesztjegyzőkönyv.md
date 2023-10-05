### A tesztelési jegyzőkönyv:

**Tesztelő:** Császár Martin Krisztián

**Tesztelés dátuma:** 2023.10.04

Tesztszám | Rövid leírás | Várt eredmény | Eredmény | Megjegyzés
----------|--------------|---------------|----------|-----------
Teszt #01 | Napnyitás | A felhasználó a napi kezdő egyenleg megadásával aktiuválja a pénztárgép felületét.  | A felhasználó sikeresen felvitte az adatokat, a rendszer engedélyezte a pénztár használatát. | Nem találtam problémát.
Teszt #02 | Gombok funkciói | Az összes gomb reagál a felhasználó által adott impulzusokra  | A felhasználó az összes gomb egymás utáni végigpróbálására mindegyik gomb reagál | Nem találtam problémát
Teszt #03 | Megjelenítő | A felhasználó számára fontos számadatok és műveleti jelek megjelennek a kijelzőn | A kijelző megjeleníti az adatokat | Nem találtam hibát
Teszt #04 | Műveletek | A felhasználó a bevitt adatokkal és műveleti jelek segítségével az "egyenlő" jel megnyomásával a kijelzőn a helyes érték jelenik meg | A program helyesen számol | Nem találtam hibát
Teszt #05 | Valutaváltás | A vásárló összes árucikkének felvitele után a végösszeget lehessen euróra váltani, vagy adott esetben euróról vissza | Mindkét esetben helyes érték jelenik meg a kijelzőn az adott valutával kapcsolatban | Mindenképpen be kell vinni az adatot az "egyenlő" jellel, hogy e-funkció működjön 
Teszt #06 | Sok karakter | A felhasználó sok árat akar felvinni a számológépbe, így túlfutna a kijelzőn a műveletsorozat, így az elejét el kellene tűntetni a kijelzőről | A számok túlfutnak a programon, nem megfelelő a kijelzés | A teszt során hibát találtam
Teszt #07 | Sok karakter | A felhasználó sok árat akar felvinni a számológépbe, így túlfutna a kijelzőn a műveletsorozat, így az elejét el kellene tűntetni a kijelzőről | A számokbal oldalon eltűnnek a látható területről, de a hozzáadott árak láthatóak| A hibát kijavítottam
