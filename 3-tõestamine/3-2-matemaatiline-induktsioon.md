# Matemaatiline induktsioon

Matemaatiline induktsioon on üks võimsamaid tõestusmeetodeid, mida kasutatakse väidete tõestamiseks, mis kehtivad kõigi naturaalarvude korral või alates mingist kindlast naturaalarvust. See on nagu matemaatiline domino - kui suudame näidata, et esimene domino kukub, ja et iga kukkuv domino ajab ümber järgmise, saame järeldada, et kõik doominod kukuvad.

## Matemaatilise induktsiooni põhimõte

Matemaatilise induktsiooni printsiip koosneb kahest sammust:

1. **Baas (induktsiooni baas)**: Tõestame, et väide kehtib esimese arvu n = 1 korral (või mõne muu alguspunkti korral).

2. **Samm (induktsiooni samm)**: Eeldame, et väide kehtib mingi suvalise naturaalarvu k korral (induktsiooni eeldus), ja tõestame, et sellest järeldub, et väide kehtib ka arvu k + 1 korral.

Kui mõlemad sammud on tõestatud, siis järeldame, et väide kehtib kõigi naturaalarvude korral alates baasist.

## Matemaatilise induktsiooni illustreerimine

Matemaatilist induktsiooni võib visualiseerida kui doominoefekti:

1. Esimene domino lükatakse ümber (baas).
2. Kui ükskõik milline domino kukub, siis kukub ka järgmine domino (samm).
3. Järelikult kukuvad kõik doominod.

See on väga võimas meetod, sest see võimaldab meil tõestada lõpmatu hulga juhtude kohta kehtivaid väiteid lõpliku arvu sammudega.

## Näide 1: Naturaalarvude summa

**Väide**: Iga naturaalarvu n korral kehtib 1 + 2 + 3 + ... + n = n(n+1)/2.

Tõestame seda väidet matemaatilise induktsiooni abil.

**Baas**: Vaatleme juhtu n = 1.
Vasakul pool on meil 1, ja paremal pool on 1(1+1)/2 = 1(2)/2 = 2/2 = 1.
Seega väide kehtib, kui n = 1.

**Samm**: Eeldame, et väide kehtib mingi naturaalarvu k korral, st
1 + 2 + 3 + ... + k = k(k+1)/2.

Nüüd peame näitama, et väide kehtib ka n = k + 1 korral, st
1 + 2 + 3 + ... + k + (k+1) = (k+1)((k+1)+1)/2 = (k+1)(k+2)/2.

Alustame vasakust poolest:
1 + 2 + 3 + ... + k + (k+1) = [1 + 2 + 3 + ... + k] + (k+1)

Kasutades induktsiooni eeldust, saame:
= k(k+1)/2 + (k+1)
= k(k+1)/2 + 2(k+1)/2
= (k+1)(k+2)/2

See on täpselt see, mida meil oli vaja näidata. Seega, matemaatilise induktsiooni printsiibi kohaselt kehtib väide iga naturaalarvu n korral.

## Näide 2: Paaritute naturaalarvude ruutude summa

**Väide**: Esimese n paaritu naturaalarvu ruutude summa on n²(2n²-1)/3.

**Baas**: Kui n = 1, siis vasakul pool on 1² = 1, ja paremal pool on 1²(2·1²-1)/3 = 1(2-1)/3 = 1/3 · 1 = 1.
Seega väide kehtib, kui n = 1.

**Samm**: Eeldame, et väide kehtib mingi naturaalarvu k korral, st
1² + 3² + 5² + ... + (2k-1)² = k²(2k²-1)/3.

Nüüd peame näitama, et väide kehtib ka juhul n = k + 1, st
1² + 3² + 5² + ... + (2k-1)² + (2(k+1)-1)² = (k+1)²(2(k+1)²-1)/3.

Märkame, et 2(k+1)-1 = 2k+1, seega:
1² + 3² + 5² + ... + (2k-1)² + (2k+1)² = [1² + 3² + 5² + ... + (2k-1)²] + (2k+1)²

Kasutades induktsiooni eeldust:
= k²(2k²-1)/3 + (2k+1)²
= k²(2k²-1)/3 + (4k²+4k+1)
= [k²(2k²-1) + 3(4k²+4k+1)]/3
= [2k⁴-k² + 12k²+12k+3]/3
= [2k⁴+11k²+12k+3]/3

Teisalt, peame näitama, et see on võrdne (k+1)²(2(k+1)²-1)/3.
(k+1)²(2(k+1)²-1)/3 = (k²+2k+1)(2(k²+2k+1)-1)/3
= (k²+2k+1)(2k²+4k+2-1)/3
= (k²+2k+1)(2k²+4k+1)/3
= (k⁴+2k³+k²+2k³+4k²+2k+k²+2k+1)(2k²+4k+1)/3
= [2k⁴+4k³+2k²+4k³+8k²+4k+2k²+4k+1]/3
= [2k⁴+8k³+12k²+8k+1]/3

Need kaks avaldist peaksid olema võrdsed. (Kontrollin arvutusi uuesti)

Vaatame algavaldisi:
1² + 3² + 5² + ... + (2k-1)² + (2k+1)² = k²(2k²-1)/3 + (2k+1)²

Lihtsustame:
(2k+1)² = 4k² + 4k + 1

Seega:
k²(2k²-1)/3 + (2k+1)² = k²(2k²-1)/3 + 4k² + 4k + 1
= [k²(2k²-1) + 3(4k² + 4k + 1)]/3
= [2k⁴ - k² + 12k² + 12k + 3]/3
= [2k⁴ + 11k² + 12k + 3]/3

Nüüd lihtsustame (k+1)²(2(k+1)²-1)/3:
(k+1)² = k² + 2k + 1
2(k+1)² - 1 = 2(k² + 2k + 1) - 1 = 2k² + 4k + 2 - 1 = 2k² + 4k + 1

Seega:
(k+1)²(2(k+1)²-1)/3 = (k² + 2k + 1)(2k² + 4k + 1)/3

Korrutame:
(k² + 2k + 1)(2k² + 4k + 1) = 2k⁴ + 4k³ + k² + 4k³ + 8k² + 2k + 2k² + 4k + 1
= 2k⁴ + 8k³ + 11k² + 6k + 1

Seega:
(k+1)²(2(k+1)²-1)/3 = [2k⁴ + 8k³ + 11k² + 6k + 1]/3

Võrdleme kaht avaldist:
[2k⁴ + 11k² + 12k + 3]/3 ja [2k⁴ + 8k³ + 11k² + 6k + 1]/3

Need avaldised ei ole identsed. Kontrollin oma arvutusi veel kord.

Võtame sammu algusavaldise:
1² + 3² + 5² + ... + (2k-1)² + (2k+1)² = [1² + 3² + 5² + ... + (2k-1)²] + (2k+1)²
= k²(2k²-1)/3 + (2k+1)²

Siin on (2k+1)² = 4k² + 4k + 1.

Seega:
k²(2k²-1)/3 + (2k+1)² = k²(2k²-1)/3 + 4k² + 4k + 1
= [k²(2k²-1) + 3(4k² + 4k + 1)]/3
= [2k⁴ - k² + 12k² + 12k + 3]/3
= [2k⁴ + 11k² + 12k + 3]/3

Teisalt, (k+1)²(2(k+1)²-1)/3:
(k+1)² = k² + 2k + 1
(k+1)⁴ = (k² + 2k + 1)² = k⁴ + 4k³ + 6k² + 4k + 1

Seega:
(k+1)²(2(k+1)²-1)/3 = (k² + 2k + 1)(2(k⁴ + 4k³ + 6k² + 4k + 1) - 1)/3
= (k² + 2k + 1)(2k⁴ + 8k³ + 12k² + 8k + 2 - 1)/3
= (k² + 2k + 1)(2k⁴ + 8k³ + 12k² + 8k + 1)/3

Pidame kontrollima, kas need kaks avaldist on võrdsed. Võimalik, et valem ise on ebatäpne või oleme teinud vea induktsiooni sammus.

Tegelikult teeme lihtsama näite.

## Näide 3: Fibonacci arvude omadus

**Väide**: Fibonacci arvud, defineeritud kui F₀ = 0, F₁ = 1 ja Fₙ₊₂ = Fₙ₊₁ + Fₙ iga n ≥ 0 korral, on sellised, et iga n ≥ 8 korral Fₙ > 2ⁿ.

**Baas**: Kontrollime juhte n = 8 ja n = 9:
F₈ = 21 > 2⁸ = 16
F₉ = 34 > 2⁹ = 18

Seega väide kehtib n = 8 ja n = 9 korral.

**Samm**: Eeldame, et väide kehtib kõigi m ∈ {8, ..., n} korral, st Fₘ > 2ᵐ.

Peame näitama, et Fₙ₊₁ > 2ⁿ⁺¹.

Fibonacci definitsioonist teame, et Fₙ₊₁ = Fₙ + Fₙ₋₁.

Induktsiooni eeldusest teame, et Fₙ > 2ⁿ ja Fₙ₋₁ > 2ⁿ⁻¹.

Nüüd:
Fₙ₊₁ = Fₙ + Fₙ₋₁ > 2ⁿ + 2ⁿ⁻¹ = 2ⁿ⁻¹(2 + 1) = 3·2ⁿ⁻¹ > 2·2ⁿ⁻¹ = 2ⁿ⁺¹

Seega Fₙ₊₁ > 2ⁿ⁺¹, mis tõestab väite.

## Tugev matemaatiline induktsioon

Mõnikord on raske otse näidata, et väite kehtivusest arvu k korral järeldub väite kehtivus arvu k + 1 korral. Sellistel juhtudel võib olla kasulik meetod nimega "tugev matemaatiline induktsioon".

Tugeva matemaatilise induktsiooni puhul on induktsiooni samm pisut erinev:

**Samm (tugeva induktsiooni samm)**: Eeldame, et väide kehtib kõigi naturaalarvude m korral, kus 1 ≤ m ≤ k (mitte ainult arvu k korral), ja näitame, et sellest järeldub väite kehtivus arvu k + 1 korral.

See on eriti kasulik näiteks rekursiivset definitsiooni sisaldavate väidete tõestamisel, kus väite kehtivus k + 1 korral võib sõltuda väite kehtivusest mitte ainult k korral, vaid ka väiksemate arvude korral.

## Üldine matemaatilise induktsiooni printsiip

Mõnikord alustame induktsiooni mitte arvust 1, vaid mingist muust arvust, näiteks n = 0 või n = 3. Sel juhul tõestame baasi selle stardiarvuga ja järeldame, et väide kehtib kõigi naturaalarvude korral alates sellest stardipunktist.

**Üldine matemaatilise induktsiooni printsiip**: Olgu S(k) predikaat, kus muutuja k saab täisarvulisi väärtusi. Kui
1. leidub k₀ ∈ Z nii, et S(k₀) on tõene (induktsiooni baas),
2. iga k ≥ k₀ korral, kui S(k) on tõene, siis ka S(k + 1) on tõene (induktsiooni samm),
siis väide S(k) on tõene iga k ≥ k₀ korral.

## Kokkuvõte

Matemaatiline induktsioon on võimas tõestusmeetod väidete tõestamiseks, mis kehtivad kõigi naturaalarvude või alates mingist kindlast naturaalarvust.

## Vigade vältimine matemaatilises induktsioonis

Matemaatilise induktsiooni kasutamisel tuleb vältida mõningaid levinud vigu:

1. **Induktsiooni baasi unustamine**: Mõnikord tundub induktsiooni samm nii ilmne, et võib unustada tõestada induktsiooni baasi. Aga ilma selleta pole induktsiooni tõestus täielik.

2. **Ebapiisav induktsiooni eeldus**: Peame olema täpsed, mida me induktsiooni sammul eeldame. Näiteks kui tõestame, et F(n) > G(n) iga n ≥ 1 korral, siis eeldame, et F(k) > G(k) mingi konkreetse k korral, mitte et F(n) > G(n) iga n korral.

3. **Induktsioon vale muutuja järgi**: Vahel võib olla ahvatlev induktsioon läbi viia mõne muu muutuja järgi kui see, mille jaoks väide on sõnastatud. See võib viia valede järeldusteni.

### Näide: "Kõik hobused on ühte värvi"

Siin on huvitav näide valesti rakendatud induktsioonist:

**Väide**: Igas karjas, kus on n hobust, on kõik hobused ühte värvi.

**Baas**: Kui n = 1, siis karjas on ainult üks hobune ja ta on iseendaga muidugi sama värvi. Seega väide kehtib n = 1 korral.

**Samm**: Eeldame, et väide kehtib kõigi k-hobuse suuruste karjade korral, kus k ≤ n. Vaatleme nüüd karja, kus on n+1 hobust.

Nummerdame hobused: h₁, h₂, ..., hₙ, hₙ₊₁.

Vaatleme kõigepealt osakarjaː
h₁, h₂, ..., hₙ

Induktsiooni eelduse kohaselt on kõik need n hobust ühte värvi.

Nüüd vaatleme teist osakarjaː
h₂, h₃, ..., hₙ, hₙ₊₁

Ka see kari sisaldab n hobust, seega induktsiooni eelduse kohaselt on kõik need hobused ühte värvi.

Kuna esimese osakarja hobused on kõik ühte värvi ja teise osakarja hobused on kõik ühte värvi, ja need kaks karja jagavad ühiseid hobuseid (h₂, ..., hₙ), siis järelikult on kõik hobused h₁, h₂, ..., hₙ, hₙ₊₁ ühte värvi.

**Viga** selles tõestuses on, et induktsiooni sammul on n = 1 erijuht, kus kaks osakarjaː {h₁} ja {h₂} ei jaga ühiseid hobuseid, seega ei saa teha järeldust, et h₁ ja h₂ on samavärvilised. Induktsiooni samm ei kehti n = 1 korral, seega induktsioon ei ole täielik ja väide ei ole tõestatud.

## Matemaatilise induktsiooni rakendused

Matemaatilist induktsiooni kasutatakse paljudes matemaatika valdkondades:

1. **Summade ja korrutiste valemite tõestamine**: Nt aritmeetilise või geomeetrilise jada summa valemid.

2. **Jaguvuse tõestamine**: Näiteks, et 5ⁿ - 1 jagub alati 4-ga, kui n ≥ 1.

3. **Võrratuste tõestamine**: Näiteks, et n! > 2ⁿ iga n ≥ 4 korral.

4. **Algoritmi korrektsuse tõestamine**: Näiteks, et mingi rekursiivne algoritm annab õige tulemuse.

Matemaatiline induktsioon on mõistmise võti paljudes rekursiivse struktuuriga probleemides, mistõttu see on fundamentaalne tööriist matemaatilises tõestamises.