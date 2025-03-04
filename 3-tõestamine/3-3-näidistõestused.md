# Näidistõestused

Selles peatükis vaatleme erinevat tüüpi tõestuste näiteid, et paremini mõista tõestamise põhimõtteid ja tehnikaid. Näidistõestuste abil saame näha, kuidas erinevaid tõestusmeetodeid praktikas rakendada ja kuidas esitada oma mõttekäiku selgelt ja loogiliselt.

## 1. Hulgateooria tõestused

### Näide 1.1: Hulkade sisalduvuse tõestamine

**Väide**: Olgu x ∈ X. Näitame, et siis x ∈ Y.

Hulkade sisalduvuse tõestamisel on oluline meeles pidada, et näitamaks X ⊂ Y, peame näitama, et iga element x, mis kuulub hulka X, kuulub ka hulka Y.

**Näide**: Tõestame, et kui A ja B on hulgad, siis A ∩ B ⊂ A ∪ B.

**Tõestus**: Olgu x suvaline element hulgast A ∩ B. Hulkade ühisosa definitsiooni kohaselt x ∈ A ja x ∈ B. Hulkade ühendi definitsiooni kohaselt, kui x ∈ A või x ∈ B, siis x ∈ A ∪ B. Kuna x ∈ A, siis x ∈ A ∪ B. Seega A ∩ B ⊂ A ∪ B.

### Näide 1.2: Hulkade võrdsuse tõestamine

**Väide**: Näitame, et kehtivad nii X ⊂ Y kui ka X ⊃ Y, ehk X = Y.

Hulkade võrdsuse tõestamisel peame näitama kahte sisalduvust: X ⊂ Y ja Y ⊂ X.

**Näide**: Tõestame, et (A ∪ B) ∩ C = (A ∩ C) ∪ (B ∩ C).

**Tõestus**:

1) Näitame, et (A ∪ B) ∩ C ⊂ (A ∩ C) ∪ (B ∩ C):
   Olgu x ∈ (A ∪ B) ∩ C. Siis x ∈ A ∪ B ja x ∈ C.
   Kuna x ∈ A ∪ B, siis kas x ∈ A või x ∈ B.
   
   Kui x ∈ A, siis kuna x ∈ C, saame et x ∈ A ∩ C, seega x ∈ (A ∩ C) ∪ (B ∩ C).
   
   Kui x ∈ B, siis kuna x ∈ C, saame et x ∈ B ∩ C, seega x ∈ (A ∩ C) ∪ (B ∩ C).
   
   Mõlemal juhul x ∈ (A ∩ C) ∪ (B ∩ C), seega (A ∪ B) ∩ C ⊂ (A ∩ C) ∪ (B ∩ C).

2) Näitame, et (A ∩ C) ∪ (B ∩ C) ⊂ (A ∪ B) ∩ C:
   Olgu x ∈ (A ∩ C) ∪ (B ∩ C). Siis kas x ∈ A ∩ C või x ∈ B ∩ C.
   
   Kui x ∈ A ∩ C, siis x ∈ A ja x ∈ C. Kuna x ∈ A, siis x ∈ A ∪ B. Ja kuna x ∈ C, siis x ∈ (A ∪ B) ∩ C.
   
   Kui x ∈ B ∩ C, siis x ∈ B ja x ∈ C. Kuna x ∈ B, siis x ∈ A ∪ B. Ja kuna x ∈ C, siis x ∈ (A ∪ B) ∩ C.
   
   Mõlemal juhul x ∈ (A ∪ B) ∩ C, seega (A ∩ C) ∪ (B ∩ C) ⊂ (A ∪ B) ∩ C.

Kuna kehtivad mõlemad sisalduvused, siis (A ∪ B) ∩ C = (A ∩ C) ∪ (B ∩ C).

## 2. Arvuteooria tõestused

### Näide 2.1: Jaguvuse tõestamine

**Väide**: Tõestame, et kui naturaalarv n jagub 3-ga, siis n² jagub 3-ga.

**Tõestus**: Olgu n naturaalarv, mis jagub 3-ga. Siis leidub täisarv k nii, et n = 3k.
Arvutame n²:
n² = (3k)² = 9k² = 3(3k²)
Kuna 3k² on täisarv, siis n² jagub 3-ga.

### Näide 2.2: Algarvu tõestus

**Väide**: Tõestame, et algarvude hulk on lõpmatu.

**Tõestus**: Kasutame vastuväitelist tõestust. Oletame, et algarvude hulk on lõplik ja algarvud on p₁, p₂, ..., pₙ.

Vaatleme arvu N = p₁ · p₂ · ... · pₙ + 1.

N on suurem kui ükski algarvudest p₁, p₂, ..., pₙ. N ei jagu ühegi algarvuga p₁, p₂, ..., pₙ, sest jagamisel jääk on alati 1. Seega, N peab olema kas algarv või jaguma mõne teise algarvuga, mida ei ole meie nimekirjas. Mõlemal juhul jõuame vastuoluni, sest eeldasime, et meie nimekiri sisaldab kõiki algarve.

See vastuolu näitab, et meie esialgne oletus oli vale ja algarvude hulk peab olema lõpmatu.

### Näide 2.3: Kongruentside tõestamine

**Väide**: Kui a ≡ b (mod m) ja c ≡ d (mod m), siis a + c ≡ b + d (mod m).

**Tõestus**: Kuna a ≡ b (mod m), siis leidub täisarv k₁ nii, et a = b + k₁m.
Kuna c ≡ d (mod m), siis leidub täisarv k₂ nii, et c = d + k₂m.

Liidame need võrdused:
a + c = b + k₁m + d + k₂m = b + d + (k₁ + k₂)m

Seega a + c ≡ b + d (mod m).

## 3. Analüüsi tõestused

### Näide 3.1: Piirprotsesside tõestamine

**Väide**: Fikseerime ε > 0. Näitame, et siis kehtib A(ε).

Piirprotsesside tõestused sisaldavad tihti ε-δ argumente, kus on vaja näidata, et kui |x - a| < δ, siis |f(x) - L| < ε.

**Näide**: Tõestame, et kui lim f(x) = L ja lim g(x) = M, siis lim (f(x) + g(x)) = L + M.
                           x→a           x→a               x→a

**Tõestus**: Fikseerime ε > 0. Piirvääruse definitsiooni kohaselt leidub δ₁ > 0 nii, et kui 0 < |x - a| < δ₁, siis |f(x) - L| < ε/2. Samuti leidub δ₂ > 0 nii, et kui 0 < |x - a| < δ₂, siis |g(x) - M| < ε/2.

Valime δ = min(δ₁, δ₂). Siis kui 0 < |x - a| < δ, siis:
|(f(x) + g(x)) - (L + M)| = |(f(x) - L) + (g(x) - M)| ≤ |f(x) - L| + |g(x) - M| < ε/2 + ε/2 = ε

Seega lim (f(x) + g(x)) = L + M.
       x→a

## 4. Algebra tõestused

### Näide 4.1: Etteantud aksioomidele tuginemine

Tõestustes on sageli vaja lähtuda teatud aksiomaatikast ehk baastõdedest, mida võime kasutada.

**Väide**: Tõestame, et kui a, b, c on täisarvud, siis (a + b) + c = a + (b + c) (liitmise assotsiatiivsus).

**Tõestus**: Väide tuleneb otseselt täisarvude liitmise aksioomist Z1, mis kinnitab, et täisarvude hulgas on liitmine assotsiatiivne.

### Näide 4.2: Omaduste tõestamine vektorruumis

**Väide**: Tõestame, et vektorruumis V kehtib 0 · v = 0 iga vektori v ∈ V korral, kus 0 on skalaar ja 0 on nullvektor.

**Tõestus**: Vektorruumi aksioomide kohaselt kehtib 1 · v = v iga v ∈ V korral. Samuti kehtib (α + β) · v = α · v + β · v iga α, β ∈ F ja v ∈ V korral (kus F on skalaaride korpus).

Valime α = 0 ja β = 0. Siis (0 + 0) · v = 0 · v + 0 · v, seega 0 · v = 0 · v + 0 · v.
Liites mõlemale poolele vektori 0 · v vastandvektori, saame 0 = 0 · v, kus 0 on nullvektor.

## 5. Kombinatoorikatõestused

### Näide 5.1: Kastide virnadesse jagamise mäng

**Väide**: Mis tahes viisil n kasti hunnikutesse jaotamisel on lõplik punktisumma alati n(n-1)/2.

**Tõestus**: Kasutame matemaatilist induktsiooni.

**Baas**: Kui n = 1, siis on meil virnas vaid üks kast. Kuna mängus ühtegi sammu teha ei ole võimalik, siis on punktisummaks 1(1-1)/2 = 0.

**Samm**: Eeldame, et väited S(1), ..., S(k) on kõik tõesed, kus S(m) on väide "m kasti hunnikutesse jaotamisel on lõplik punktisumma alati m(m-1)/2".

Näitame, et siis S(k+1) on ka tõene. Seega, olgu meil virnas k+1 kasti ning esimese sammuna jagame need kastid kahte uude virna kõrgusega i ja (k+1)−i kasti (mingi i korral, kus 1 ≤ i ≤ k).

Mängu lõppsumma moodustavad sellel esimesel käigul saadud punktide ja kõikide järgmiste käikude punktide summa. Seega:

lõppsumma = (1. käigu punktid) + (i kasti jaotamise punktid) + (k + 1 - i kasti jaotamise punktid)

= i(k + 1 - i) + i(i - 1)/2 + (k + 1 - i)(k + 1 - i - 1)/2

= i(k + 1 - i) + i(i - 1)/2 + (k + 1 - i)(k - i)/2

= i(k + 1) - i² + i² - i + (k + 1)(k - i) - (k - i)²
                    2         2

= i(k + 1) - i + (k + 1)(k - i) - (k - i)²
              2         2

Lihtsustades jõuame tulemuseni (k+1)k/2, mis ongi täpselt see, mida oli vaja näidata.

### Näide 5.2: Kombinatsioonide arvu omadused

**Väide**: Tõestame, et iga naturaalarvu n ja täisarvu k korral, kus 0 ≤ k ≤ n, kehtib C(n,k) = C(n,n-k).

**Tõestus**: 
C(n,k) = n! / (k! · (n-k)!)
C(n,n-k) = n! / ((n-k)! · (n-(n-k))!) = n! / ((n-k)! · k!)

Näeme, et need avaldised on võrdsed, seega C(n,k) = C(n,n-k).

## 6. Võrratuste tõestused

### Näide 6.1: Kolmnurga võrratus

**Väide**: Tõestame, et mis tahes reaalarvude x ja y korral kehtib |x + y| ≤ |x| + |y|.

**Tõestus**: Vaatleme nelja alamjuhtu:

a) Olgu x ≥ 0 ja y ≥ 0. Siis |x + y| = x + y = |x| + |y|.

b) Olgu x ≥ 0 ja y < 0. 
   (i) Kui x + y ≥ 0, siis |x + y| = x + y < x + 0 = |x| ≤ |x| + |y|.
   (ii) Kui x + y < 0, siis |x + y| = -(x + y) = -x - y ≤ |-x| + |-y| = |x| + |y|.

c) Olgu x < 0 ja y ≥ 0. See juht on sümmeetriline juhuga b).

d) Olgu x < 0 ja y < 0. Siis |x + y| = -(x + y) = -x - y = |x| + |y|.

Kõigil juhtudel kehtib |x + y| ≤ |x| + |y|.

## 7. Väidete ümberlükkamine ehk kontranäited

Mõnikord on vaja näidata, et mingi üldistus ei kehti, leideks selleks kontranäite.

### Näide 7.1: Kontranäite leidmine

**Väide**: Näitame, et väide "Kui a < b, siis a² < b²" pole üldjuhul tõene.

**Kontranäide**: Valime a = -2 ja b = -1. Siis a < b, sest -2 < -1, kuid a² > b², sest 4 > 1.

## 8. Tõestuste kirjutamise põhimõtted

Hea tõestuse kirjutamisel on soovitatav järgida mõningaid põhimõtteid:

1. **Selgus**: Tõestus peaks olema selge ja arusaadav. Iga samm peaks järgima loogiliselt eelmist.

2. **Täielikkus**: Tõestus peaks sisaldama kõiki olulisi samme, ilma et midagi oleks vahele jäetud.

3. **Täpsus**: Kasutage täpseid matemaatilisi termineid ja sümboleid.

4. **Struktuur**: Liigendage oma tõestus, eriti kui see on pikk või keeruline.

5. **Elegantsus**: Püüdke leida kõige lihtsam ja elegantsem tõestus. Matemaatikas hinnatakse kauneid ja kompaktseid tõestusi.

Loodan, et need näidistõestused aitavad sul paremini mõista erinevaid tõestusmeetodeid ja nende rakendamist praktikas. Tõestuste kirjutamine nõuab harjutamist, kuid aja jooksul muutub see oskus järjest paremaks.

## Kokkuvõte

Oleme vaadelnud erinevat tüüpi tõestusi erinevatest matemaatika valdkondadest:
- Hulgateooria tõestused
- Arvuteooria tõestused
- Analüüsi tõestused
- Algebra tõestused
- Kombinatoorikatõestused
- Võrratuste tõestused
- Väidete ümberlükkamine kontranäidete abil

Mida rohkem tõestusi näed ja läbi töötad, seda paremini hakkad mõistma matemaatilist mõtlemist ja tõestamise kunsti. Oluline on mitte ainult teada, et mingi tulemus on tõene, vaid mõista, miks see on tõene ja kuidas see seostub teiste matemaatiliste tõdedega.