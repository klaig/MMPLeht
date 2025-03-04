# Lausearvutuse samaväärsused

## Samaväärsuse mõiste

Lausearvutuses on samaväärsus üks olulisemaid mõisteid, mis võimaldab meil valemeid teisendada, lihtsustada ja analüüsida.

**Definitsioon:** Valemeid F ja G nimetatakse **loogiliselt samaväärseteks**, kui nende tõeväärtused on võrdsed igal neis valemeis esinevate muutujate väärtustusel.

Asjaolu, et valemid F ja G on samaväärsed, tähistatakse sümboliga F ≡ G.

### Samaväärsuse kontrollimise meetodid

Kahe valemi samaväärsust saab kontrollida mitmel viisil:

1. **Tõeväärtustabelite võrdlemisega** - kui kahel valemil on identsed tõeväärtuste veerud, siis need valemid on samaväärsed.

2. **Teoreemi abil** - valemid F ja G on samaväärsed parajasti siis, kui valem F ⇔ G on samaselt tõene (tautoloogia).

3. **Järeldumise abil** - valemid F ja G on samaväärsed parajasti siis, kui F ⊨ G ja G ⊨ F.

4. **Samaväärsuste kasutamisega** - rakendades tuntud samaväärsusi, saame ühte valemit teisendada teiseks.

## Põhisamaväärsused

Lausearvutuses on hulk olulisi põhisamaväärsusi, mida saame kasutada valemite teisendamisel ja lihtsustamisel. Need võib jagada erinevatesse kategooriatesse.

### 1. Idempotentsuse omadused

Idempotentsuse omadused näitavad, et tehte kordamine sama muutuja või valemiga ei muuda tulemust.

- F ∧ F ≡ F
- F ∨ F ≡ F

**Näide:** Valem X ∧ X on samaväärne valemiga X.

**Elulise näide:** Kui sa ütled "Ma olen õnnelik ja ma olen õnnelik", siis see on sama, kui ütleksid lihtsalt "Ma olen õnnelik".

### 2. Kommutatiivsuse omadused

Kommutatiivsuse omadused näitavad, et tehetes osalevatele muutujatele või valemitele vahetades kohad, tehe ei muutu.

- F ∧ G ≡ G ∧ F
- F ∨ G ≡ G ∨ F

**Näide:** Valem X ∧ Y on samaväärne valemiga Y ∧ X.

**Elulise näide:** "Ma õpin ja töötan" tähendab sama, mis "Ma töötan ja õpin".

### 3. Assotsiatiivsuse omadused

Assotsiatiivsuse omadused näitavad, et mitme tehte puhul ei ole oluline, millises järjekorras me tehted grupeerime.

- (F ∧ G) ∧ H ≡ F ∧ (G ∧ H)
- (F ∨ G) ∨ H ≡ F ∨ (G ∨ H)

**Näide:** Valem (X ∧ Y) ∧ Z on samaväärne valemiga X ∧ (Y ∧ Z).

**Elulise näide:** "Ma ostan leiba ja (piima ning juustu)" tähendab sama, mis "(Ma ostan leiba ja piima) ning juustu".

### 4. Distributiivsuse omadused

Distributiivsuse omadused näitavad, kuidas üks tehe "jaotub" teise tehte üle.

- F ∧ (G ∨ H) ≡ (F ∧ G) ∨ (F ∧ H)
- F ∨ (G ∧ H) ≡ (F ∨ G) ∧ (F ∨ H)

**Näide:** Valem X ∧ (Y ∨ Z) on samaväärne valemiga (X ∧ Y) ∨ (X ∧ Z).

**Elulise näide:** "Ma lähen kinno ja (vaatan komöödiat või draamat)" tähendab sama, mis "(Ma lähen kinno ja vaatan komöödiat) või (ma lähen kinno ja vaatan draamat)".

### 5. Neelamisomadused (absorptsioon)

Neelamisomadused näitavad, kuidas mõned tehted "neelavad" teisi.

- F ∧ (F ∨ G) ≡ F
- F ∨ (F ∧ G) ≡ F

**Näide:** Valem X ∧ (X ∨ Y) on samaväärne valemiga X.

**Elulise näide:** "Ma ostan auto ja (ma ostan auto või maja)" tähendab sama, mis lihtsalt "Ma ostan auto".

### 6. De Morgani seadused

De Morgani seadused näitavad, kuidas eitus jaotub konjunktsiooni ja disjunktsiooni üle.

- ¬(F ∧ G) ≡ ¬F ∨ ¬G
- ¬(F ∨ G) ≡ ¬F ∧ ¬G

**Näide:** Valem ¬(X ∧ Y) on samaväärne valemiga ¬X ∨ ¬Y.

**Elulise näide:** "Pole tõsi, et ma õpin ja töötan" tähendab sama, mis "Ma ei õpi või ma ei tööta".

### 7. Kahekordse eituse omadus

Kahekordne eitus taastab algse valemi.

- ¬¬F ≡ F

**Näide:** Valem ¬¬X on samaväärne valemiga X.

**Elulise näide:** "Pole tõsi, et ma ei õpi" tähendab sama, mis "Ma õpin".

### 8. Liikmete elimineerimise reeglid

Need reeglid näitavad, kuidas samaselt tõene (t) ja samaselt väär (v) valem käitub tehetega.

- F ∧ t ≡ F (kus t on samaselt tõene valem)
- F ∨ t ≡ t
- F ∧ v ≡ v (kus v on samaselt väär valem)
- F ∨ v ≡ F

**Näide:** Valem X ∧ t on samaväärne valemiga X. Valem X ∨ v on samaväärne valemiga X.

**Elulise näide:** "Ma õpin ja tõsi on, et 2+2=4" tähendab sama, mis "Ma õpin". "Ma õpin või vale on, et 2+2=4" tähendab sama, mis "Ma õpin".

### 9. Implikatsiooni avaldised konjunktsiooni, disjunktsiooni ja eituse kaudu

Implikatsiooni saab avaldada mitmel erineval viisil:

- F ⇒ G ≡ ¬F ∨ G
- F ⇒ G ≡ ¬(F ∧ ¬G)

**Näide:** Valem X ⇒ Y on samaväärne valemiga ¬X ∨ Y.

**Elulise näide:** "Kui sajab vihma, siis ma võtan vihmavarju" tähendab sama, mis "Ei saja vihma või ma võtan vihmavarju".

### 10. Konjunktsiooni ja disjunktsiooni avaldised implikatsiooni kaudu

Konjunktsiooni ja disjunktsiooni saab avaldada implikatsiooni kaudu:

- F ∧ G ≡ ¬(F ⇒ ¬G)
- F ∨ G ≡ ¬F ⇒ G

**Näide:** Valem X ∧ Y on samaväärne valemiga ¬(X ⇒ ¬Y).

### 11. Ekvivalentsi avaldised teiste tehete kaudu

Ekvivalentsi saab avaldada konjunktsiooni, disjunktsiooni, eituse ja implikatsiooni kaudu:

- F ⇔ G ≡ (F ⇒ G) ∧ (G ⇒ F)
- F ⇔ G ≡ (F ∧ G) ∨ (¬F ∧ ¬G)
- F ⇔ G ≡ ¬(F ⊕ G) (kus ⊕ tähistab sümmeetrilist vahet, XOR-tehet)

**Näide:** Valem X ⇔ Y on samaväärne valemiga (X ⇒ Y) ∧ (Y ⇒ X).

**Elulise näide:** "Ma lähen välja parajasti siis, kui ilm on ilus" tähendab sama, mis "(Kui ilm on ilus, siis ma lähen välja) ja (kui ma lähen välja, siis ilm on ilus)".

### 12. Tautoloogia ja kontradiktsioon

- F ∨ ¬F ≡ t (tautoloogia)
- F ∧ ¬F ≡ v (kontradiktsioon)

**Näide:** Valem X ∨ ¬X on samaselt tõene (tautoloogia) ja valem X ∧ ¬X on samaselt väär (kontradiktsioon).

## Samaväärsuste kasutamine

Samaväärsusi saab kasutada mitmel eesmärgil:

1. **Valemite lihtsustamine** - keeruliste valemite teisendamine lihtsamatele kujudele
2. **Valemite teisendamine normaalkujule** - valemite teisendamine standardsetele vormidele nagu disjunktiivne normaalkuju (DNK)
3. **Valemite analüüsimine** - valemite omaduste uurimine ilma tõeväärtustabelita
4. **Teoreemide tõestamine** - matemaatiliste väidete formaalse kehtivuse näitamine

## Näited samaväärsuste rakendamisest

### Näide 1: Valemi lihtsustamine

Lihtsustage valem ¬(X ∧ Y) ∨ (X ∧ ¬Y).

**Lahendus:**

1. Rakendame esimesele liikmele De Morgani seadust:
   ¬(X ∧ Y) ∨ (X ∧ ¬Y) ≡ (¬X ∨ ¬Y) ∨ (X ∧ ¬Y)

2. Kasutame assotsiatiivsuse omadust:
   (¬X ∨ ¬Y) ∨ (X ∧ ¬Y) ≡ ¬X ∨ ¬Y ∨ (X ∧ ¬Y)

3. Kasutame distributiivsuse omadust:
   ¬X ∨ ¬Y ∨ (X ∧ ¬Y) ≡ ¬X ∨ (¬Y ∨ (X ∧ ¬Y))
   ≡ ¬X ∨ ((¬Y ∨ X) ∧ (¬Y ∨ ¬Y))
   ≡ ¬X ∨ ((¬Y ∨ X) ∧ ¬Y) (idempotentsuse omadus)
   ≡ ¬X ∨ (¬Y ∧ (¬Y ∨ X)) (kommutatiivsuse omadus)
   ≡ ¬X ∨ ¬Y (neelamisomadus)

Seega, ¬(X ∧ Y) ∨ (X ∧ ¬Y) ≡ ¬X ∨ ¬Y.

### Näide 2: Implikatsiooni teisendamine

Teisendage implikatsioon (X ⇒ Y) ⇒ Z ilma implikatsioonita kujule, kasutades eitust, konjunktsiooni ja disjunktsiooni.

**Lahendus:**

1. Kõigepealt asendame implikatsiooni X ⇒ Y samaväärse kujuga ¬X ∨ Y:
   (X ⇒ Y) ⇒ Z ≡ (¬X ∨ Y) ⇒ Z

2. Nüüd asendame välimise implikatsiooni:
   (¬X ∨ Y) ⇒ Z ≡ ¬(¬X ∨ Y) ∨ Z

3. Kasutame De Morgani seadust:
   ¬(¬X ∨ Y) ∨ Z ≡ (¬¬X ∧ ¬Y) ∨ Z

4. Lihtsustame kahekordse eituse:
   (¬¬X ∧ ¬Y) ∨ Z ≡ (X ∧ ¬Y) ∨ Z

Seega, (X ⇒ Y) ⇒ Z ≡ (X ∧ ¬Y) ∨ Z.

### Näide 3: Täieliku disjunktiivse normaalkuju leidmine

Leidke valemi X ⇒ (Y ∧ Z) täielik disjunktiivne normaalkuju.

**Lahendus:**

1. Asendame implikatsiooni:
   X ⇒ (Y ∧ Z) ≡ ¬X ∨ (Y ∧ Z)

2. Kasutame distributiivsuse omadust:
   ¬X ∨ (Y ∧ Z) ≡ (¬X ∨ Y) ∧ (¬X ∨ Z)

3. Nüüd peame tagasi minema disjunktiivsele kujule. Kasutame distributiivsuse omadust vastupidi:
   (¬X ∨ Y) ∧ (¬X ∨ Z) ≡ ¬X ∨ (Y ∧ Z)
   
   Tegelikult see ei ole disjunktiivne normaalkuju. Proovime uuesti:
   
   X ⇒ (Y ∧ Z) ≡ ¬X ∨ (Y ∧ Z)
   
4. TDNK jaoks vajame kõigi muutujate kombinatsioone. Täielik disjunktiivne normaalkuju on:
   (¬X ∧ ¬Y ∧ ¬Z) ∨ (¬X ∧ ¬Y ∧ Z) ∨ (¬X ∧ Y ∧ ¬Z) ∨ (¬X ∧ Y ∧ Z) ∨ (X ∧ Y ∧ Z)

Märkus: Täieliku disjunktiivse normaalkuju leidmiseks on tihti lihtsam kasutada tõeväärtustabelit.

## Samaväärsuste rakendamise praktilised aspektid

### Miks on samaväärsused kasulikud?

1. **Efektiivsus** - tõeväärtustabelite kasutamine võib muutuda väga töömahukaks, kui valemis on palju muutujaid. Samaväärsused võimaldavad meil valemeid analüüsida ilma täieliku tõeväärtustabelita.
2. **Lihtsustamine** - samaväärsuste abil saame keerulisi valemeid lihtsustada, mis muudab neid loetavamaks ja kergemini analüüsitavaks.
3. **Teisendamine** - samaväärsused võimaldavad meil muuta valemite kuju vastavalt vajadusele, näiteks eemaldada teatud tehted või viia valem standardkujule.
4. **Probleemide lahendamine** - paljude loogikaülesannete lahendamisel on samaväärsused võtmetähtsusega.

### Kuidas valida õiget samaväärsust?

Sobiva samaväärsuse valimine sõltub kontekstist ja eesmärgist:

1. **Kui soovid eemaldada implikatsioone või ekvivalentse**, kasuta vastavaid samaväärsusi nende asendamiseks eituse, konjunktsiooni ja disjunktsiooniga.
2. **Kui soovid viia eitused vahetult muutujate ette**, kasuta De Morgani seadusi.
3. **Kui soovid lihtsustada valemit**, otsi võimalusi idempotentsuse, neelamisomaduste ja elimineerimisreeglite rakendamiseks.
4. **Kui soovid leida normaalkuju**, kasuta distributiivsuse omadusi, et viia valem vajalikule kujule.

## Samaväärsuste rakendamine praktilistes olukordades

### Loogikaskeemide optimeerimine

Samaväärsusi kasutatakse digitaalskeemide (loogikaskeemide) optimeerimiseks. Lihtsamad valemid tähendavad vähem loogikaelemente ja kiiremaid arvutusi.

**Näide:** Loogikaskeem, mis realiseerib valemi (A ∧ B) ∨ (A ∧ ¬B), saab lihtsustada kujule A, kasutades distributiivsust ja neelamisomadust:
(A ∧ B) ∨ (A ∧ ¬B) ≡ A ∧ (B ∨ ¬B) ≡ A ∧ t ≡ A

### Programmeerimistingimuste lihtsustamine

Programmeerimises võib keeruliste tingimuslausete lihtsustamine muuta koodi loetavamaks ja efektiivsemaks.

**Näide:** Tingimuslause
```
if ((x > 0 && y > 0) || (x > 0 && y <= 0))
```
saab lihtsustada samaväärsuste abil kujule
```
if (x > 0)
```
sest (x > 0 ∧ y > 0) ∨ (x > 0 ∧ ¬(y > 0)) ≡ x > 0 ∧ (y > 0 ∨ ¬(y > 0)) ≡ x > 0 ∧ t ≡ x > 0

## Harjutusülesanded

### Ülesanne 1
Tõestage, et valemid (X ⇒ Y) ∧ (X ⇒ Z) ja X ⇒ (Y ∧ Z) on samaväärsed, kasutades samaväärsusseoseid.

**Lahendus:**
1. (X ⇒ Y) ∧ (X ⇒ Z)
2. (¬X ∨ Y) ∧ (¬X ∨ Z) (implikatsiooni avaldumine)
3. ¬X ∨ (Y ∧ Z) (distributiivsuse omadus)
4. X ⇒ (Y ∧ Z) (implikatsiooni avaldumine)

Seega (X ⇒ Y) ∧ (X ⇒ Z) ≡ X ⇒ (Y ∧ Z).

### Ülesanne 2
Lihtsustage valem (X ∧ Y) ∨ (X ∧ ¬Y) ∨ (¬X ∧ Y), kasutades samaväärsusseoseid.

**Lahendus:**
1. (X ∧ Y) ∨ (X ∧ ¬Y) ∨ (¬X ∧ Y)
2. ((X ∧ Y) ∨ (X ∧ ¬Y)) ∨ (¬X ∧ Y) (assotsiatiivsuse omadus)
3. (X ∧ (Y ∨ ¬Y)) ∨ (¬X ∧ Y) (distributiivsuse omadus)
4. (X ∧ t) ∨ (¬X ∧ Y) (tautoloogia Y ∨ ¬Y ≡ t)
5. X ∨ (¬X ∧ Y) (liikmete elimineerimise reegel)
6. (X ∨ ¬X) ∧ (X ∨ Y) (distributiivsuse omadus)
7. t ∧ (X ∨ Y) (tautoloogia X ∨ ¬X ≡ t)
8. X ∨ Y (liikmete elimineerimise reegel)

Seega (X ∧ Y) ∨ (X ∧ ¬Y) ∨ (¬X ∧ Y) ≡ X ∨ Y.

### Ülesanne 3
Tõestage, et valemid ¬(X ⇔ Y) ja X ⇔ ¬Y on samaväärsed, kasutades samaväärsusseoseid.

**Lahendus:**
1. ¬(X ⇔ Y)
2. ¬((X ⇒ Y) ∧ (Y ⇒ X)) (ekvivalentsi avaldumine)
3. ¬(X ⇒ Y) ∨ ¬(Y ⇒ X) (De Morgani seadus)
4. (X ∧ ¬Y) ∨ (Y ∧ ¬X) (implikatsiooni eitus)
5. (X ∧ ¬Y) ∨ (¬X ∧ Y) (kommutatiivsuse omadus)
6. (X ⇒ ¬Y) ∧ (¬Y ⇒ X) (implikatsiooni avaldumine)
7. X ⇔ ¬Y (ekvivalentsi avaldumine)

Seega ¬(X ⇔ Y) ≡ X ⇔ ¬Y.

## Kokkuvõte

Lausearvutuse samaväärsused on võimas tööriist valemite teisendamiseks, lihtsustamiseks ja analüüsimiseks. Need võimaldavad meil:

1. Avaldada keerulisemaid tehteid lihtsamate kaudu
2. Vähendada valemite keerukust
3. Ümber formuleerida probleeme lahendataval kujul
4. Optimeerida loogikat programmeerimises ja elektroonikas

Olulisemate samaväärsuste tundmine ja õige rakendamine on oluline oskus nii matemaatikas, arvutiteaduses kui ka filosoofilises argumentatsioonis.

## Samaväärsuste meelespea

Allolev tabel võtab kokku olulisemad samaväärsused, mida peaks kindlasti teadma:

| Kategooria | Samaväärsus | Selgitus |
|------------|-------------|----------|
| **Idempotentsus** | F ∧ F ≡ F | Konjunktsiooni kordamine sama valemiga |
| | F ∨ F ≡ F | Disjunktsiooni kordamine sama valemiga |
| **Kommutatiivsus** | F ∧ G ≡ G ∧ F | Konjunktsioon ei sõltu järjekorrast |
| | F ∨ G ≡ G ∨ F | Disjunktsioon ei sõltu järjekorrast |
| **Assotsiatiivsus** | (F ∧ G) ∧ H ≡ F ∧ (G ∧ H) | Konjunktsioon ei sõltu grupeerimisest |
| | (F ∨ G) ∨ H ≡ F ∨ (G ∨ H) | Disjunktsioon ei sõltu grupeerimisest |
| **Distributiivsus** | F ∧ (G ∨ H) ≡ (F ∧ G) ∨ (F ∧ H) | Konjunktsioon jaotub disjunktsiooni üle |
| | F ∨ (G ∧ H) ≡ (F ∨ G) ∧ (F ∨ H) | Disjunktsioon jaotub konjunktsiooni üle |
| **Neelamisomadused** | F ∧ (F ∨ G) ≡ F | Konjunktsioon neelab disjunktsiooni |
| | F ∨ (F ∧ G) ≡ F | Disjunktsioon neelab konjunktsiooni |
| **De Morgan** | ¬(F ∧ G) ≡ ¬F ∨ ¬G | Konjunktsiooni eitus |
| | ¬(F ∨ G) ≡ ¬F ∧ ¬G | Disjunktsiooni eitus |
| **Kahekordne eitus** | ¬¬F ≡ F | Kahekordse eituse eemaldamine |
| **Elimineerimisreeglid** | F ∧ t ≡ F | Konjunktsioon tõesega |
| | F ∨ t ≡ t | Disjunktsioon tõesega |
| | F ∧ v ≡ v | Konjunktsioon vääraga |
| | F ∨ v ≡ F | Disjunktsioon vääraga |
| **Implikatsioon** | F ⇒ G ≡ ¬F ∨ G | Implikatsiooni avaldamine disjunktsiooniga |
| | F ⇒ G ≡ ¬(F ∧ ¬G) | Implikatsiooni avaldamine eitusega |
| **Ekvivalents** | F ⇔ G ≡ (F ⇒ G) ∧ (G ⇒ F) | Ekvivalentsi avaldamine implikatsioonidega |
| | F ⇔ G ≡ (F ∧ G) ∨ (¬F ∧ ¬G) | Ekvivalentsi avaldamine konjunktsiooni ja disjunktsiooniga |
| **Tautoloogia ja kontradiktsioon** | F ∨ ¬F ≡ t | Välistatud kolmanda seadus |
| | F ∧ ¬F ≡ v | Mittevasturääkivuse seadus |

## Praktilised rakendused igapäevaelus

### Näide: Küberturbe ligipääsuõigused

Ettevõttes on määratud ligipääsuõigused järgmiselt:
- A: "Kasutaja on administraator"
- B: "Kasutaja kuulub IT osakonda"
- C: "On tööaeg (8:00-17:00)"

Ligipääsupoliitika andmebaasile on: "Kasutaja pääseb andmebaasile ligi, kui ta on administraator, või kui ta kuulub IT osakonda ja on tööaeg."

See tingimus väljendub valemina: A ∨ (B ∧ C)

Kui süsteemi peab optimeerima ja on vaja teada teist samaväärset tingimust, võib kasutada distributiivsuse omadust:
A ∨ (B ∧ C) ≡ (A ∨ B) ∧ (A ∨ C)

See tähendab, et ligipääsuõigus on samaväärne tingimusega: "Kasutaja on administraator või kuulub IT osakonda, JA kasutaja on administraator või on tööaeg."

### Näide: Loogilise argumentatsiooni analüüs

Vaatleme argumenti: "Kui ettevõte investeerib turundusse, siis müük kasvab. Kui müük kasvab, siis kasum suureneb. Seega, kui ettevõte investeerib turundusse, siis kasum suureneb."

Tähistame:
- P: "Ettevõte investeerib turundusse"
- Q: "Müük kasvab"
- R: "Kasum suureneb"

Argument väidab, et kui (P ⇒ Q) ja (Q ⇒ R), siis (P ⇒ R).

Kontrollime seda samaväärsuste abil:
1. (P ⇒ Q) ∧ (Q ⇒ R)
2. (¬P ∨ Q) ∧ (¬Q ∨ R) (implikatsiooni avaldumine)

Kas sellest järeldub P ⇒ R ehk ¬P ∨ R?

Kui vaatame tõeväärtustabeleid, siis näeme, et see on tõesti nii. Samaväärsuste abil saaksime seda tõestada järgmiselt:

Kui (¬P ∨ Q) ∧ (¬Q ∨ R), siis võime tuletada:
- Kui P on tõene (ehk ¬P on väär), siis esimesest osast (¬P ∨ Q) saame Q peab olema tõene
- Kui Q on tõene, siis teisest osast (¬Q ∨ R) saame R peab olema tõene
- Seega kui P on tõene, siis R on tõene, mis on samaväärne väitega P ⇒ R

See on klassikaline transitiivsuse näide: kui P ⇒ Q ja Q ⇒ R, siis P ⇒ R.

## Visuaalne abimaterjal loogiliste samaväärsuste kohta

Meelespea olulisimate samaväärsuste kohta lausearvutuses:

```
┌────────────────────────────────────────────────────┐
│  Olulised loogilised samaväärsused                 │
├────────────────────────────────────────────────────┤
│                                                    │
│  De Morgani seadused:                              │
│  ¬(P ∧ Q) ≡ ¬P ∨ ¬Q                               │
│  ¬(P ∨ Q) ≡ ¬P ∧ ¬Q                               │
│                                                    │
│  Distributiivsuse omadused:                        │
│  P ∧ (Q ∨ R) ≡ (P ∧ Q) ∨ (P ∧ R)                  │
│  P ∨ (Q ∧ R) ≡ (P ∨ Q) ∧ (P ∨ R)                  │
│                                                    │
│  Implikatsiooni avaldamine:                        │
│  P → Q ≡ ¬P ∨ Q                                    │
│                                                    │
│  Kahekordse eituse omadus:                         │
│  ¬¬P ≡ P                                          │
│                                                    │
└────────────────────────────────────────────────────┘
```

## Kokkuvõte

Lausearvutuse samaväärsused on võimas tööriist valemite teisendamiseks, lihtsustamiseks ja analüüsimiseks. Need võimaldavad meil:

1. Avaldada keerulisemaid tehteid lihtsamate kaudu
2. Vähendada valemite keerukust
3. Ümber formuleerida probleeme lahendataval kujul
4. Optimeerida loogikat programmeerimises ja elektroonikas

Olulisemate samaväärsuste tundmine ja õige rakendamine on oluline oskus nii matemaatikas, arvutiteaduses kui ka filosoofilises argumentatsioonis.