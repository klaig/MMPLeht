# Predikaadid ja muutujad

## Mis on predikaat?

Lausearvutuses tegelesime lihtlausetega, millel oli kindel tõeväärtus – need olid kas tõesed või väärad. Predikaatarvutuses laiendame seda kontseptsiooni ja kasutame **predikaate**, mis on väited, mille tõeväärtus sõltub muutujate väärtustest.

**Definitsioon:** Predikaat on väide, mis sisaldab vähemalt ühte muutujat ja millele saab omistada tõeväärtuse niipea, kui muutuja(te)le on omistatud konkreetsed väärtused.

Predikaatide tähistamiseks kasutatakse suuri tähti (P, Q, R, ...) ning sulgudes näidatakse muutujad, millest predikaat sõltub, näiteks P(x), Q(x, y), R(z).

### Näited predikaatidest:

1. P(x): "x on algarv"
   - P(2) on tõene, sest 2 on algarv
   - P(4) on väär, sest 4 ei ole algarv

2. Q(x, y): "x on suurem kui y"
   - Q(5, 3) on tõene, sest 5 > 3
   - Q(2, 7) on väär, sest 2 ei ole suurem kui 7

3. R(x): "x on Eesti linn"
   - R(Tallinn) on tõene
   - R(Stockholm) on väär

## Diskursuse universum

Predikaatarvutuses on oluline roll **diskursuse universumil** (ka tuntud kui **individuaalvaldkond** või **domeeni universum**), mis määrab muutujate võimalike väärtuste piirkonna. Diskursuse universumi tähistame tavaliselt tähega D.

- Kui uurime predikaati P(x): "x on algarv", võib D olla naturaalarvude hulk N.
- Kui uurime predikaati R(x): "x on Eesti linn", on D kõigi linnade hulk.

Diskursuse universum on definitsiooni järgi mitteTühi. Muutujad võivad omandada väärtusi ainult diskursuse universumist, mitte väljastpoolt seda.

## Predikaatide liigid argsumentide arvu järgi

Predikaate liigitatakse sageli nende argumentide arvu järgi:

1. **Unaarsed predikaadid** – ühe argumendiga predikaadid, näiteks P(x).
2. **Binaarsed predikaadid** – kahe argumendiga predikaadid, näiteks Q(x, y).
3. **Ternaarsed predikaadid** – kolme argumendiga predikaadid, näiteks S(x, y, z).
4. **n-aarsed predikaadid** – n argumendiga predikaadid, näiteks T(x₁, x₂, ..., xₙ).

## Termid

**Term** on predikaatarvutuse väljend, mis tähistab objekti diskursuse universumist. Need on predikaatarvutuse "nimed" või viisid, kuidas viidata objektidele.

Termid võivad olla:
1. **Konstandid** – kindlad fikseeritud objektid diskursuse universumist (tähistame väiketähtedega a, b, c, ...)
2. **Muutujad** – objektid, mis võivad omada erinevaid väärtusi diskursuse universumist (tähistame väiketähtedega x, y, z, ...)
3. **Funktsiooniavaldised** – funktsioonid, mis sõltuvad termidest ja annavad tulemuseks termid

### Näide: 

Kui D on reaalarvude hulk, siis:
- Konstandid võiksid olla: 0, 1, π, e
- Muutujad võiksid olla: x, y, z
- Funktsiooniavaldised võiksid olla: x + y, x², sin(x)

## Muutujad predikaatarvutuses

Predikaatarvutuses on muutujad olulise tähtsusega. Nad võimaldavad meil väljendada väiteid, mis kehtivad erinevate objektide korral.

### Vabad ja seotud muutujad

Predikaatarvutuse valemites on oluline eristada kahte tüüpi muutujaid:

1. **Vaba muutuja** – muutuja, mis ei ole seotud ühegi kvantoriga. Vaba muutuja on nagu parameeter, mis võib omandada erinevaid väärtusi.

2. **Seotud muutuja** – muutuja, mis on seotud kvantoriga (∀ või ∃). Seotud muutujat saab asendada mis tahes diskursuse universumi elemendiga ilma valemi tähendust muutmata.

### Näide:

Vaatame valemit: ∀x P(x) ∧ Q(y)

Selles valemis on x seotud muutuja (seotud kvantoriga ∀), aga y on vaba muutuja. See tähendab, et valemi tõeväärtus sõltub y väärtusest, aga x väärtus võib olla ükskõik milline diskursuse universumi element.

## Laused predikaatarvutuses

**Lauseks** nimetatakse predikaatarvutuses valemit, milles kõik muutujad on seotud kvantoriga. Lausel on kindel tõeväärtus konkreetse diskursuse universumi suhtes.

### Näide:

Valem ∀x P(x) on lause, sest kõik muutujad (antud juhul ainult x) on seotud kvantoriga.
Valem P(x) ei ole lause, sest x on vaba muutuja.

## Predikaatide formaliseerimine

Predikaatarvutuse üks tugevusi on võime formaliseerida loomuliku keele väiteid täpsel ja struktureeritud viisil.

### Näide 1:

Lause: "Kõik inimesed on surelikud."

Formaliseerimine:
- Diskursuse universum D: kõigi olendite hulk
- Predikaadid:
  - I(x): "x on inimene"
  - S(x): "x on surelik"
- Formaliseeritud valem: ∀x (I(x) → S(x))

See valem loetakse: "Iga olendi x korral, kui x on inimene, siis x on surelik."

### Näide 2:

Lause: "Mõned õpilased õpivad kõiki õppeaineid."

Formaliseerimine:
- Diskursuse universum D: kõik inimesed ja õppeained
- Predikaadid:
  - Õ(x): "x on õpilane"
  - A(y): "y on õppeaine"
  - O(x,y): "x õpib õppeainet y"
- Formaliseeritud valem: ∃x (Õ(x) ∧ ∀y (A(y) → O(x,y)))

See valem loetakse: "Leidub selline x, et x on õpilane ja iga y korral, kui y on õppeaine, siis x õpib õppeainet y."

## Predikaatide kasutamine matemaatikas

Predikaatarvutus on eriti kasulik matemaatiliste ideede ja teoreemide formaliseerimiseks.

### Näide 1: Algarvu definitsioon

Definitsioon: "Naturaalarv p > 1 on algarv, kui tema ainsad naturaalarvulised jagajad on 1 ja p ise."

Formaliseerimine:
- Diskursuse universum D: naturaalarvude hulk N
- Predikaadid:
  - A(p): "p on algarv"
  - J(d,p): "d jagab p-d" (ehk p jagub d-ga)
- Formaliseeritud valem: A(p) ⟺ (p > 1 ∧ ∀d ((d ∈ N ∧ J(d,p)) → (d = 1 ∨ d = p)))

### Näide 2: Funktsioon f on pidev punktis a

Definitsioon: "Funktsioon f on pidev punktis a, kui iga ε > 0 korral leidub δ > 0 nii, et kui |x - a| < δ, siis |f(x) - f(a)| < ε."

Formaliseerimine:
- Diskursuse universum D: reaalarvude hulk R
- Predikaadid:
  - P(f,a): "funktsioon f on pidev punktis a"
- Formaliseeritud valem: P(f,a) ⟺ ∀ε (ε > 0 → ∃δ (δ > 0 ∧ ∀x (|x - a| < δ → |f(x) - f(a)| < ε)))

## Kasulikud tehnikad predikaatide formaliseerimisel

### 1. Implikatsiooni kasutamine tingimuslike väidete jaoks

Paljud laused sisaldavad tingimuslikke seoseid, mida saame väljendada implikatsiooni abil. Näiteks:

"Kõik koerad on imetajad" ⟺ ∀x (K(x) → I(x))
- K(x): "x on koer"
- I(x): "x on imetaja"

### 2. Konteksti määramine diskursuse universumi abil

Valides sobiva diskursuse universumi, saame sageli lihtsustada formaliseerimist:

"Kõik liinibussid on kollased" 
- Kui D = {kõik transpordivahendid}, siis: ∀x (L(x) → K(x))
- Kui D = {kõik liinibussid}, siis lihtsalt: ∀x K(x)

### 3. Kvantori ja implikatsiooni reeglid

Kui formaliseerime lause "kõik X-id on Y-id", saame kasutada kahte samaväärset vormi:
- ∀x (X(x) → Y(x))
- ¬∃x (X(x) ∧ ¬Y(x))

Nende samaväärsus tuleneb kvantoritega seotud loogikareeglitest, mida käsitleme põhjalikumalt järgmistes teemades.

## Harjutusülesanded

### Ülesanne 1
Formaliseerige järgmised laused predikaatarvutuses:

a) Kõik tudengid õpivad matemaatikat.
b) Mõned raamatud on huvitavad.
c) Ükski kass ei ole inimene.
d) Kui number on paarisarv, siis ta jagub 2-ga.
e) Iga reaalarvu ruut on mittenegatiivne.

**Lahendused:**

a) ∀x (T(x) → M(x)), kus 
   - T(x): "x on tudeng"
   - M(x): "x õpib matemaatikat"

b) ∃x (R(x) ∧ H(x)), kus
   - R(x): "x on raamat"
   - H(x): "x on huvitav"

c) ∀x (K(x) → ¬I(x)) või ekvivalentselt ¬∃x (K(x) ∧ I(x)), kus
   - K(x): "x on kass"
   - I(x): "x on inimene"

d) ∀x (P(x) → J(x,2)), kus
   - P(x): "x on paarisarv"
   - J(x,y): "x jagub y-ga"

e) ∀x (x ∈ ℝ → x² ≥ 0)

### Ülesanne 2
Formaliseerige järgmised matemaatilised väited:

a) Iga naturaalarvu ruut on suurem või võrdne kui arv ise.
b) Kahe järjestikuse naturaalarvu korrutis on alati paarisarv.
c) Leidub selline reaalarv, mille ruut on 2.
d) Iga positiivse reaalarvu jaoks leidub temast väiksem positiivne reaalarv.

**Lahendused:**

a) ∀x (x ∈ ℕ → x² ≥ x)

b) ∀n (n ∈ ℕ → P(n·(n+1))), kus
   - P(x): "x on paarisarv"
   Alternatiivselt: ∀n (n ∈ ℕ → ∃k (k ∈ ℕ ∧ n·(n+1) = 2k))

c) ∃x (x ∈ ℝ ∧ x² = 2)

d) ∀x ((x ∈ ℝ ∧ x > 0) → ∃y (y ∈ ℝ ∧ 0 < y < x))

### Ülesanne 3
Andke järgmistele predikaatarvutuse valemitele loomulik tõlge eesti keelde:

a) ∀x (I(x) → ∃y (I(y) ∧ V(x,y))), kus
   - I(x): "x on inimene"
   - V(x,y): "x vajab y-i"

b) ∀x (K(x) → (∃y (K(y) ∧ S(y,x)) ∨ ∃z (H(z) ∧ S(z,x)))), kus
   - K(x): "x on kass"
   - H(x): "x on inimene"
   - S(x,y): "x sööb y-i"

c) ¬∃x (T(x) ∧ ∀y (A(y) → L(x,y))), kus
   - T(x): "x on tudeng"
   - A(y): "y on õppeaine"
   - L(x,y): "x läbis õppeaine y"

**Lahendused:**

a) "Iga inimene vajab mingit teist inimest."

b) "Iga kassi sööb kas mõni teine kass või mõni inimene."

c) "Pole ühtegi tudengit, kes oleks läbinud kõik õppeained." või "Ükski tudeng pole läbinud kõiki õppeaineid."

### Ülesanne 4
Määrake, millised muutujad on vabad ja millised seotud järgmistes valemites:

a) ∀x (P(x) → Q(x,y))
b) ∃z (R(x,z) ∧ ∀x S(x,z))
c) ∀x ∃y (T(x,y,z) → ∀z U(x,y,z))

**Lahendused:**

a) x on seotud (üldisuskvantoriga ∀), y on vaba

b) z on seotud (olemasolukvantori ∃ poolt), x on algul vaba, aga teises osas seotud (üldisuskvantoriga ∀)

c) x on seotud (üldisuskvantoriga ∀), y on seotud (olemasolukvantori ∃ poolt), z on algul vaba, aga teises osas seotud (üldisuskvantoriga ∀)

## Kokkuvõte

Predikaadid on oluline osa predikaatarvutusest, mis võimaldavad meil väljendada tingimusi, mis sõltuvad muutujatest. Muutujad võivad olla vabad või seotud kvantoriga. Predikaadid koos kvantorite ja loogiliste tehetega võimaldavad väljendada keerulisi matemaatilisi ja igapäevaelu väiteid formaalses keeles.

Olulised punktid, mida meeles pidada:

1. **Predikaat** on väide, mille tõeväärtus sõltub muutuja(te) väärtustest
2. **Diskursuse universum** määrab muutujate võimalike väärtuste piirkonna
3. **Vaba muutuja** ei ole seotud ühegi kvantoriga ja võib omandada suvalisi väärtusi
4. **Seotud muutuja** on seotud kvantoriga (∀ või ∃)
5. **Lauseks** nimetatakse predikaatarvutuses valemit, milles kõik muutujad on seotud

Predikaatide korralik mõistmine on aluseks predikaatarvutuse järgmistele teemadele, eriti kvantorite kasutamisele ja eitamise reeglitele.