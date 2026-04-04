---
layout: single
classes: wide
title: "Csalnak-e az Ötös Lottónál?"
permalink: /otoslotto/
author_profile: true
---

# Csalnak-e az Ötös Lottónál? Megnéztük az adatokat, és van válaszunk

A magyar internet egyik örökzöld témája, hogy az Ötös Lottó húzásai nem lehetnek véletlenek. Hogy egyes számokat feltűnően sokszor húznak, másokat alig. Hogy biztosan bele van nyúlva. Fórumokon, kommentszekciókban, kocsmapultoknál rendszeresen felmerül a gyanú: a Szerencsejáték Zrt. csal.

Mi erre azt mondjuk: nézzük meg. Nem véleményt fogalmazunk meg, hanem letöltöttük a teljes nyilvános adatbázist, és hét különböző statisztikai módszerrel vizsgáltuk meg, hogy a számok azt mutatják-e, amit egy tisztességes sorsolásnál várnánk. Spoiler: igen, pontosan azt.

## 3604 húzás, 18 ezer golyó

A szerencsejatek.hu oldaláról elérhető az Ötös Lottó összes húzásának története 2004-től 2026 márciusáig. Ez összesen 3604 heti sorsolás. Mivel minden héten 90-ből húznak 5 számot, ez 18 020 kihúzott golyó. Ha a lottó fair, akkor hosszú távon minden szám nagyjából egyformán gyakran jön ki: a várt átlag számonként körülbelül 200 húzás.

## A rekorderek

A leggyakrabban kihúzott szám a **3-as**: 240-szer jött ki 22 év alatt. A legritkább a **88-as**, mindössze 158-szor. Első pillantásra ez hatalmas különbség, a 3-as másfélszer annyiszor került elő! Fogadjunk, ez a két szám van kinn minden összeesküvés-elmélet alapjaként szolgáló toplistán.

De gondoljunk bele: ha feldobunk egy érmét kétszázszor, szinte soha nem lesz pontosan száz fej és száz írás. Lesz mondjuk 112 meg 88, és az teljesen normális. A kérdés nem az, hogy van-e különbség a számok között -- persze hogy van --, hanem az, hogy ez a különbség akkora-e, amit a puszta véletlen már nem magyaráz.

## Mit mondanak a tesztek?

A legklasszikusabb módszer erre az úgynevezett khi-négyzet próba: összehasonlítja a megfigyelt gyakoriságokat azzal, amit egyenletes eloszlásnál várnánk. Az eredmény egyértelmű: a p-érték 0,084, ami azt jelenti, hogy **nincs szignifikáns eltérés**. Ilyen mértékű ingadozás a tökéletesen véletlenszerű húzásoknál is simán előfordul -- körülbelül minden tizenkettedik esetben.

<figure>
  <img src="/assets/images/otoslotto/szamgyakorisag.png" alt="Lottószámok gyakorisága">
  <figcaption>A 90 szám gyakorisága 3604 húzásban. A szaggatott vonal a várt átlag (200), a pontozott vonalak a normál ingadozás határai. Pirossal a kiugróan gyakori, zölddel a ritkán húzott számok -- de összesen csak 5 lóg ki, ami pont annyi, amennyit a véletlen alapján is várnánk.</figcaption>
</figure>

## De nem csak a gyakoriságot néztük

Ha valaki csalna, azt máshol is látnánk. Megvizsgáltuk, hogy az öt kihúzott szám összege milyen eloszlást követ. Ha a húzás fair, az összegnek egy szép, szimmetrikus haranggörbét kell rajzolnia az elméleti átlag (228) körül. Nos:

<figure>
  <img src="/assets/images/otoslotto/osszeg_eloszlas.png" alt="Húzások összegének eloszlása">
  <figcaption>A kék oszlopok a tényleges húzások összegének eloszlása, a piros vonal az elméleti haranggörbe. A kettő gyakorlatilag egymásra simul.</figcaption>
</figure>

A megfigyelt átlag 225,7, a várt 227,5. A szórás 56,5 a várt 56,8 helyett. Ez nem csak "nagyjából stimmel" -- ez rendkívül pontos egyezés közel négyezer húzásra.

## Mikor jön ki újra a kedvenc számunk?

Van egy különösen szemléletes módja annak, hogy ellenőrizzük a véletlenszerűséget. Ha egy szám kijön, mennyi idő telik el átlagosan, amíg újra kihúzzák? Ha a lottó fair, ennek az úgynevezett geometrikus eloszlást kell követnie -- a legtöbb visszatérés gyors (pár héten belül), de időnként vannak hosszabb szünetek is, és ezek jól kiszámítható valószínűséggel fordulnak elő.

<figure>
  <img src="/assets/images/otoslotto/visszateresi_ido.png" alt="Visszatérési idő eloszlása">
  <figcaption>A számok visszatérési idejének eloszlása (kék) szinte tökéletesen illeszkedik az elméleti görbére (piros). Az átlagos várakozási idő 17,9 hét -- a várt 18,0.</figcaption>
</figure>

## Forró és hideg számok?

Sokan hiszik, hogy vannak "forró" számok, amelyeket érdemes játszani, mert éppen jó sorozatban vannak. Mások a "hideg" számokat keresik, mondván, hogy azok "esedékesek". Megvizsgáltuk a két szélsőséget: a 3-ast (a leggyakoribb) és a 88-ast (a legritkább) az elmúlt 22 évben, 200 húzásos gördülő ablakkal.

<figure>
  <img src="/assets/images/otoslotto/idotrend.png" alt="Időbeli trendek">
  <figcaption>A 3-as és a 88-as szám gyakorisága az idő függvényében. A szürke sáv a normál ingadozás tartománya. Vannak ugyan hullámok, de ezek a véletlennel teljesen konzisztensek -- egyik szám sem "szökik meg" tartósan.</figcaption>
</figure>

Igen, vannak periódusok, amikor a 3-as kicsit gyakrabban jön ki, és vannak, amikor ritkábban. De ez pont olyan, mint amikor az érmedobásnál néha öt fej jön egymás után: utólag mintázatnak tűnik, de valójában a véletlen természetes velejárója. A görbe végig a szürke sávon -- a normál ingadozás tartományán -- belül marad.

## Hét teszt, egy válasz

Összesen hét különböző szempontból vizsgáltuk az adatokat: a számok egyenkénti gyakorisága, az összegek eloszlása, a páros-páratlan arány, a szomszédos számok előfordulása, a visszatérési idők, az időbeli trendek és a sorozatok hossza. **Egyetlen teszt sem mutatott statisztikailag szignifikáns eltérést a fair, véletlenszerű sorsolástól.**

Természetesen egyetlen elemzés sem tudja végérvényesen bebizonyítani, hogy soha, semmilyen manipuláció nem történt. Amit viszont kijelenthetünk: a 2004 és 2026 közötti 3604 húzás minden vizsgált dimenzióban pontosan úgy viselkedik, ahogy egy tisztességes sorsolástól elvárjuk.

Aki csalást gyanít, annak nem a lottógéppel van baja, hanem a véletlennel. A golyók nem emlékeznek a korábbi húzásokra. A mintázatok, amiket látunk, a véletlen természetes velejárói. Az Ötös Lottó -- legalábbis a számok tanúsága szerint -- tiszta játék.

---

*Az elemzés a szerencsejatek.hu nyilvános adatai alapján készült. Az adatok, a Python kód és az összes ábra elérhető [a projekt GitHub oldalán](https://github.com/gabors-data-analysis/lotto-analysis). A cikk szerzője Békés Gábor közgazdász, a [Bevezetés az adatelemzésbe](https://gabors-data-analysis.com/) tankönyv társszerzője.*
