# Normaalkujud lausearvutuses

## Sissejuhatus

Lausearvutuse valemite normaalkujud on standardsed vormid, millesse saab teisendada iga lausearvutuse valemi. Normaalkujude kasutamine muudab valemite analüüsi ja võrdlemist lihtsamaks ning on aluseks paljudele automatiseeritud teoreemitõestuse algoritmidele. Kaks kõige olulisemat normaalkuju on **disjunktiivne normaalkuju (DNK)** ja **konjunktiivne normaalkuju (KNK)**.

Normaalkuju mõte on kahandada lausearvutuse valemite süntaktilist mitmekesisust, andes neile lihtsa ja ühtse väliskuju. Lisaks sellele on täielike normaalkujude puhul lihtne välja lugeda väärtustused, millal need valemid on tõesed.

## Põhimõisted

Enne normaalkujude käsitlemist on oluline mõista mõningaid põhimõisteid:

### Literaal

**Literaal** on lausemuutuja (nt X, Y, Z) või selle eitus (nt ¬X, ¬Y, ¬Z).

**Näide:** X, ¬Y ja Z on kõik literaalid.

### Lihtkonjunktsioon (elementaarkonjunktsioon)

**Lihtkonjunktsioon** on literaalide konjunktsioon (ja-seos).

**Näide:** X ∧ Y, X ∧ ¬Z, ¬X ∧ Y ∧ Z on kõik lihtkonjunktsioonid.

### Lihtdisjunktsioon (elementaardisjunktsioon)

**Lihtdisjunktsioon** on literaalide disjunktsioon (või-seos).

**Näide:** X ∨ Y, X ∨ ¬Z, ¬X ∨ Y ∨ Z on kõik lihtdisjunktsioonid.

### Täielik lihtkonjunktsioon

**Täielik lihtkonjunktsioon** on lihtkonjunktsioon, milles iga vaadeldav muutuja esineb täpselt ühe korra (kas eitatuna või ilma eituseta).

**Näide:** Kui vaatleme muutujaid X, Y ja Z, siis X ∧ Y ∧ Z, X ∧ ¬Y ∧ Z, ¬X ∧ Y ∧ ¬Z on kõik täielikud lihtkonjunktsioonid.

### Täielik lihtdisjunktsioon

**Täielik lihtdisjunktsioon** on lihtdisjunktsioon, milles iga vaadeldav muutuja esineb täpselt ühe korra (kas eitatuna või ilma eituseta).

**Näide:** Kui vaatleme muutujaid X, Y ja Z, siis X ∨ Y ∨ Z, X ∨ ¬Y ∨ Z, ¬X ∨ Y ∨ ¬Z on kõik täielikud lihtdisjunktsioonid.

## Disjunktiivne normaalkuju (DNK)

**Definitsioon:** Lausearvutuse valemi disjunktiivne normaalkuju (DNK) on valemiga samaväärne valem, mis kujutab endast erinevate lihtkonjunktsioonide disjunktsiooni.

DNK on kujul:
(L₁₁ ∧ L₁₂ ∧ ... ∧ L₁ₙ) ∨ (L₂₁ ∧ L₂₂ ∧ ... ∧ L₂ₙ) ∨ ... ∨ (Lₘ₁ ∧ Lₘ₂ ∧ ... ∧ Lₘₙ)

kus L on literaal.

**Näide:** Valem (X ∧ Y) ∨ (¬X ∧ Z) on disjunktiivsel normaalkujul, sest see on kahe lihtkonjunktsiooni disjunktsioon.

### DNK leidmine

Valemi viimiseks disjunktiivsele normaalkujule saab kasutada järgmisi samme:

1. Eemaldada valemist implikatsioonid (⇒) ja ekvivalentsid (⇔), kasutades nende definitsioone:
   - F ⇒ G ≡ ¬F ∨ G
   - F ⇔ G ≡ (F ⇒ G) ∧ (G ⇒ F) ≡ (¬F ∨ G) ∧ (¬G ∨ F)

2. Viia eitused (¬) vahetult muutujate ette, kasutades De Morgani seadusi:
   - ¬(F ∧ G) ≡ ¬F ∨ ¬G
   - ¬(F ∨ G) ≡ ¬F ∧ ¬G
   ja eemaldades kahekordsed eitused: ¬¬F ≡ F

3. Kasutada distributiivsuse omadust, et teisendada konjunktsioonid disjunktsioonide üle:
   - F ∧ (G ∨ H) ≡ (F ∧ G) ∨ (F ∧ H)

**Näide:**
Viime valemi ¬(X ⇒ Y) disjunktiivsele normaalkujule.

1. ¬(X ⇒ Y)
2. ¬(¬X ∨ Y) (implikatsiooni eemaldamine)
3. ¬¬X ∧ ¬Y (De Morgani seadus)
4. X ∧ ¬Y (kahekordse eituse eemaldamine)

Valem X ∧ ¬Y on juba disjunktiivsel normaalkujul (üks lihtkonjunktsioon).

## Konjunktiivne normaalkuju (KNK)

**Definitsioon:** Lausearvutuse valemi konjunktiivne normaalkuju (KNK) on valemiga samaväärne valem, mis kujutab endast erinevate lihtdisjunktsioonide konjunktsiooni.

KNK on kujul:
(L₁₁ ∨ L₁₂ ∨ ... ∨ L₁ₙ) ∧ (L₂₁ ∨ L₂₂ ∨ ... ∨ L₂ₙ) ∧ ... ∧ (Lₘ₁ ∨ Lₘ₂ ∨ ... ∨ Lₘₙ)

kus L on literaal.

**Näide:** Valem (X ∨ Y) ∧ (¬X ∨ Z) on konjunktiivsel normaalkujul, sest see on kahe lihtdisjunktsiooni konjunktsioon.

### KNK leidmine

Valemi viimiseks konjunktiivsele normaalkujule saab kasutada sarnaseid samme nagu DNK puhul, ainult viimases etapis tuleb kasutada distributiivsuse teist vormi:

- F ∨ (G ∧ H) ≡ (F ∨ G) ∧ (F ∨ H)

**Näide:**
Viime valemi X ∨ (Y ∧ Z) konjunktiivsele normaalkujule.

1. X ∨ (Y ∧ Z)
2. (X ∨ Y) ∧ (X ∨ Z) (distributiivsuse omadus)

Valem (X ∨ Y) ∧ (X ∨ Z) on juba konjunktiivsel normaalkujul.

## Täielik disjunktiivne normaalkuju (TDNK)

**Definitsioon:** Lausearvutuse valemi täielik disjunktiivne normaalkuju (TDNK) on valemiga samaväärne valem, mis kujutab endast erinevate täielike lihtkonjunktsioonide disjunktsiooni.

TDNK on kujul:
(L₁₁ ∧ L₁₂ ∧ ... ∧ L₁ₙ) ∨ (L₂₁ ∧ L₂₂ ∧ ... ∧ L₂ₙ) ∨ ... ∨ (Lₘ₁ ∧ Lₘ₂ ∧ ... ∧ Lₘₙ)

kus igas lihtkonjunktsioonis esineb täpselt üks kord iga vaadeldav muutuja (kas eitatuna või ilma eituseta).

**Näide:** Kui vaatleme muutujaid X, Y ja Z, siis valem (X ∧ Y ∧ Z) ∨ (X ∧ ¬Y ∧ ¬Z) ∨ (¬X ∧ Y ∧ ¬Z) on täielikul disjunktiivsel normaalkujul.

### TDNK leidmine

TDNK leidmiseks võib kasutada kahte meetodit:

#### 1. Teisendamise teel

Kõigepealt leiame valemi disjunktiivse normaalkuju ja seejärel täiendame iga lihtkonjunktsiooni nii, et see sisaldaks kõiki muutujaid.

**Näide:**
Viime valemi X ∧ (Y ∨ ¬Z) täielikule disjunktiivsele normaalkujule.

1. X ∧ (Y ∨ ¬Z)
2. (X ∧ Y) ∨ (X ∧ ¬Z) (distributiivsuse omadus)

Nüüd täiendame iga lihtkonjunktsiooni:
3. (X ∧ Y ∧ Z) ∨ (X ∧ Y ∧ ¬Z) ∨ (X ∧ ¬Y ∧ ¬Z)

## Täielik konjunktiivne normaalkuju (TKNK)

**Definitsioon:** Lausearvutuse valemi täielik konjunktiivne normaalkuju (TKNK) on valemiga samaväärne valem, mis kujutab endast erinevate täielike lihtdisjunktsioonide konjunktsiooni.

TKNK on kujul:
(L₁₁ ∨ L₁₂ ∨ ... ∨ L₁ₙ) ∧ (L₂₁ ∨ L₂₂ ∨ ... ∨ L₂ₙ) ∧ ... ∧ (Lₘ₁ ∨ Lₘ₂ ∨ ... ∨ Lₘₙ)

kus igas lihtdisjunktsioonis esineb täpselt üks kord iga vaadeldav muutuja (kas eitatuna või ilma eituseta).

**Näide:** Kui vaatleme muutujaid X, Y ja Z, siis valem (X ∨ Y ∨ Z) ∧ (X ∨ ¬Y ∨ ¬Z) ∧ (¬X ∨ Y ∨ ¬Z) on täielikul konjunktiivsel normaalkujul.

### TKNK leidmine

TKNK leidmiseks saab kasutada sarnaseid meetodeid nagu TDNK puhul:

#### 1. Teisendamise teel

Kõigepealt leiame valemi konjunktiivse normaalkuju ja seejärel täiendame iga lihtdisjunktsiooni nii, et see sisaldaks kõiki muutujaid.

#### 2. Tõeväärtustabeli abil

1. Koostame valemi tõeväärtustabeli.
2. Valime kõik read, kus valemi tõeväärtus on v (väär).
3. Iga sellise rea jaoks moodustame täieliku lihtdisjunktsiooni, kus kõik literaalid on eitatud võrreldes tõeväärtustabeli rea väärtustega.
4. TKNK on kõigi nende täielike lihtdisjunktsioonide konjunktsioon.

**Näide:**
Leiame valemi X ∧ (Y ∨ ¬Z) TKNK tõeväärtustabeli abil.

| X | Y | Z | Y ∨ ¬Z | X ∧ (Y ∨ ¬Z) |
|---|---|---|--------|--------------|
| t | t | t | t      | t            |
| t | t | v | t      | t            |
| t | v | t | v      | v            |
| t | v | v | t      | t            |
| v | t | t | t      | v            |
| v | t | v | t      | v            |
| v | v | t | v      | v            |
| v | v | v | t      | v            |

Valemi tõeväärtus on väär ridades 3, 5, 6, 7 ja 8, mis vastavad väärtustele:
- X = t, Y = v, Z = t
- X = v, Y = t, Z = t
- X = v, Y = t, Z = v
- X = v, Y = v, Z = t
- X = v, Y = v, Z = v

Iga väära tõeväärtusega rea jaoks loome täieliku lihtdisjunktsiooni, kus eitame literaale, mis on tõesed, ja jätame eitamata literaalid, mis on väärad:
- (¬X ∨ Y ∨ ¬Z) (esimene väär rida, X = t, Y = v, Z = t)
- (X ∨ ¬Y ∨ ¬Z) (teine väär rida, X = v, Y = t, Z = t)
- (X ∨ ¬Y ∨ Z) (kolmas väär rida, X = v, Y = t, Z = v)
- (X ∨ Y ∨ ¬Z) (neljas väär rida, X = v, Y = v, Z = t)
- (X ∨ Y ∨ Z) (viies väär rida, X = v, Y = v, Z = v)

Seega on TKNK:
(¬X ∨ Y ∨ ¬Z) ∧ (X ∨ ¬Y ∨ ¬Z) ∧ (X ∨ ¬Y ∨ Z) ∧ (X ∨ Y ∨ ¬Z) ∧ (X ∨ Y ∨ Z)

## Normaalkujude omadused ja rakendused

### TDNK omadused

1. **Ühesus**: Iga lausearvutuse valemil on täpselt üks täielik disjunktiivne normaalkuju (kui literaalide järjekord lihtkonjunktsioonides on fikseeritud).

2. **Tõesustingimused**: TDNK näitab otseselt, milliste muutujate väärtuste korral on valem tõene. Iga täielik lihtkonjunktsioon vastab ühele tõesele väärtustusele.

3. **Kehtestatavuse kontroll**: Valem on kehtestatav parajasti siis, kui tema TDNK ei ole tühi (s.t. kui valemil on üldse täielik disjunktiivne normaalkuju).

**Teoreem:** Valemil eksisteerib täielik disjunktiivne normaalkuju parajasti siis, kui ta on kehtestatav (s.t leidub väärtustus, mille korral valemi väärtus on tõene).

**Näide:** Valem X ∧ ¬X ei ole kehtestatav, sest tema TDNK on tühi (pole ühtegi väärtustust, mille korral valem oleks tõene).

### TKNK omadused

1. **Ühesus**: Iga lausearvutuse valemil on täpselt üks täielik konjunktiivne normaalkuju (kui literaalide järjekord lihtdisjunktsioonides on fikseeritud).

2. **Väärustingimused**: TKNK näitab otseselt, milliste muutujate väärtuste korral on valem väär. Iga täielik lihtdisjunktsioon vastab ühele väära väärtustusega kombinatsioonile.

3. **Tautoloogsuse kontroll**: Valem on tautoloogia (samaselt tõene) parajasti siis, kui tema TKNK ei ole tühi.

### Normaalkujude praktilised rakendused

#### 1. Loogikaskeemide disain

Disjunktiivne normaalkuju vastab otseselt OR-AND struktuuriga loogikaskeemile, samas kui konjunktiivne normaalkuju vastab AND-OR struktuuriga skeemile. 

**Näide:** Valem (X ∧ Y) ∨ (¬X ∧ Z) realiseeritakse loogikaskeemina, kus on kaks AND-väravat, mille väljundid on ühendatud ühe OR-väravaga.

#### 2. Automaatne teoreemitõestamine

Paljud automaatsed teoreemitõestamise algoritmid, näiteks resolutsioonimeetod, nõuavad sisendvalemeid konjunktiivsel normaalkujul.

#### 3. SAT-lahendajad 

SAT-lahendajad (satisfiability solvers) on algoritmid, mis otsustavad, kas antud lausearvutuse valem on kehtestatav. Enamik SAT-lahendajaid eeldab, et sisendvalem on konjunktiivsel normaalkujul.

#### 4. Kvantorfitsioon

Täielikud normaalkujud võimaldavad teisendada predikaatarvutuse valemeid lausearvutuse valemiteks protsessis, mida nimetatakse kvantorfitsiooniks.

## Normaalkujude vahelised seosed

### Dualiteet

Täielik disjunktiivne normaalkuju (TDNK) ja täielik konjunktiivne normaalkuju (TKNK) on duaalsed mõisted. Kui asendame TDNK-s kõik konjunktsioonid disjunktsioonidega ja vastupidi ning eitame kõiki literaale, saame teise valemi TKNK.

**Näide:** Kui valemi TDNK on (X ∧ Y ∧ ¬Z) ∨ (¬X ∧ ¬Y ∧ Z), siis tema duaalne valem on (¬X ∨ ¬Y ∨ Z) ∧ (X ∨ Y ∨ ¬Z).

### Eituse mõju normaalkujule

Kui valem F on esitatud TDNK kujul, siis ¬F saab esitada TKNK kujul, asendades konjunktsioonid disjunktsioonidega ja vastupidi ning eitades kõiki literaale.

**Näide:** Kui valemi F TDNK on (X ∧ Y) ∨ (¬X ∧ Z), siis ¬F TKNK on (¬X ∨ ¬Y) ∧ (X ∨ ¬Z).

## Näited keerulisemate valemite normaalkujule viimisest

### Näide 1: Implikatsiooni ja ekvivalentsi sisaldava valemi TDNK

Leidame valemi (X ⇒ Y) ⇔ (Y ⇒ Z) täieliku disjunktiivse normaalkuju.

**Lahendus:**

1. Asendame ekvivalentsi:
   (X ⇒ Y) ⇔ (Y ⇒ Z)
   ≡ ((X ⇒ Y) ⇒ (Y ⇒ Z)) ∧ ((Y ⇒ Z) ⇒ (X ⇒ Y))

2. Asendame implikatsioonid:
   ≡ ((¬X ∨ Y) ⇒ (¬Y ∨ Z)) ∧ ((¬Y ∨ Z) ⇒ (¬X ∨ Y))
   ≡ (¬(¬X ∨ Y) ∨ (¬Y ∨ Z)) ∧ (¬(¬Y ∨ Z) ∨ (¬X ∨ Y))
   ≡ ((X ∧ ¬Y) ∨ ¬Y ∨ Z) ∧ ((Y ∧ ¬Z) ∨ ¬X ∨ Y)

3. Lihtsustame:
   ≡ ((X ∧ ¬Y) ∨ ¬Y ∨ Z) ∧ ((Y ∧ ¬Z) ∨ ¬X ∨ Y)
   ≡ (¬Y ∨ Z) ∧ (¬Z ∨ ¬X ∨ Y)

   Esimene lihtsustamine toimub nii: (X ∧ ¬Y) ∨ ¬Y = ¬Y ∨ (X ∧ ¬Y) = ¬Y ∨ X
   Kuid (X ∧ ¬Y) ∨ ¬Y = ¬Y ∨ (X ∧ ¬Y) = ¬Y(1 ∨ X) = ¬Y

4. Nüüd on valem konjunktiivsel normaalkujul. Viime selle disjunktiivsele normaalkujule:
   (¬Y ∨ Z) ∧ (¬Z ∨ ¬X ∨ Y)
   ≡ (¬Y ∨ Z) ∧ ((¬Z ∨ ¬X) ∨ Y)
   ≡ (¬Y ∧ (¬Z ∨ ¬X)) ∨ (Z ∧ (¬Z ∨ ¬X)) ∨ (¬Y ∧ Y) ∨ (Z ∧ Y)
   ≡ (¬Y ∧ ¬Z) ∨ (¬Y ∧ ¬X) ∨ (Z ∧ ¬Z) ∨ (Z ∧ ¬X) ∨ (¬Y ∧ Y) ∨ (Z ∧ Y)
   ≡ (¬Y ∧ ¬Z) ∨ (¬Y ∧ ¬X) ∨ (Z ∧ ¬X) ∨ (Z ∧ Y)

5. Nüüd peame iga lihtkonjunktsiooni täiendama, et saada täielik disjunktiivne normaalkuju. Näiteks, lihtkonjunktsioon ¬Y ∧ ¬Z peab täiendama nii, et see sisaldaks ka X-i:
   (¬Y ∧ ¬Z ∧ X) ∨ (¬Y ∧ ¬Z ∧ ¬X) ∨ (¬Y ∧ ¬X ∧ Z) ∨ (¬Y ∧ ¬X ∧ ¬Z) ∨ ...

See on keeruline protsess ja tihti on lihtsam kasutada tõeväärtustabelit TDNK leidmiseks.

### Näide 2: TDNK leidmine tõeväärtustabeli abil

Leidame valemi (X ⇒ Y) ⇔ (Y ⇒ Z) TDNK tõeväärtustabeli abil.

**Lahendus:**

Koostame tõeväärtustabeli:

| X | Y | Z | X ⇒ Y | Y ⇒ Z | (X ⇒ Y) ⇔ (Y ⇒ Z) |
|---|---|---|-------|-------|---------------------|
| t | t | t | t     | t     | t                   |
| t | t | v | t     | v     | v                   |
| t | v | t | v     | t     | v                   |
| t | v | v | v     | t     | v                   |
| v | t | t | t     | t     | t                   |
| v | t | v | t     | v     | v                   |
| v | v | t | t     | t     | t                   |
| v | v | v | t     | t     | t                   |

Valemi tõeväärtus on tõene ridades 1, 5, 7 ja 8, mis vastavad väärtustele:
- X = t, Y = t, Z = t
- X = v, Y = t, Z = t
- X = v, Y = v, Z = t
- X = v, Y = v, Z = v

Seega on TDNK:
(X ∧ Y ∧ Z) ∨ (¬X ∧ Y ∧ Z) ∨ (¬X ∧ ¬Y ∧ Z) ∨ (¬X ∧ ¬Y ∧ ¬Z)

Seda saab lihtsustada:
(Y ∧ Z) ∨ (¬X ∧ ¬Y)

## Erijuhud normaalkujude leidmisel

### Tautoloogia ja kontradiktsioon

**Tautoloogia** on valem, mis on tõene kõigi väärtustuste korral (nt X ∨ ¬X). Tautoloogia TDNK sisaldab kõiki võimalikke täielikke lihtkonjunktsioone, mis teeb selle väga pikaks.

**Kontradiktsioon** on valem, mis on väär kõigi väärtustuste korral (nt X ∧ ¬X). Kontradiktsioonil puudub TDNK, sest pole ühtegi väärtustust, mille korral valem oleks tõene.

### Samaselt tõesed ja samaselt väärad valemid

**Samaselt tõene valem** (tautoloogia) DNK kujul on lihtkonjunktsioonide disjunktsioon, mis sisaldab kõiki võimalikke täielikke lihtkonjunktsioone. Näiteks, kui meil on kaks muutujat X ja Y, siis tautoloogia TDNK on:
(X ∧ Y) ∨ (X ∧ ¬Y) ∨ (¬X ∧ Y) ∨ (¬X ∧ ¬Y)

**Samaselt väär valem** (kontradiktsioon) DNK kujul on tühi disjunktsioon, mida võib märkida kui v (väär).

## Normaalkujude praktiline kasutamine

### Andmebaasipäringud disjunktiivsel normaalkujul

**Disjunktiivse normaalkuju kasutamine andmebaasi otsingus:**

Kui loome otsingufunktsiooni, mis võimaldab kasutajatel leida tooteid erinevate kriteeriumide alusel, on päring sageli disjunktiivsel normaalkujul:

```sql
-- Leia tooted, mis on:
-- (Nutitelefonid JA alla 500€) VÕI (Sülearvutid JA SSD-ga)
SELECT * FROM Tooted 
WHERE (kategooria = 'Nutitelefon' AND hind < 500)
   OR (kategooria = 'Sülearvuti' AND omadused LIKE '%SSD%')
```

See on disjunktiivsel normaalkujul, kuna tegu on konjunktsioonide (AND) disjunktsiooniga (OR).

### Loogikaskeemide disainimine

**Näide loogikaskeemi optimeerimisest:**

Oletame, et meil on loogikaskeem, mis realiseerib valemi (P ∧ Q) ∨ (P ∧ ¬Q).

Lihtsustame seda:
1. (P ∧ Q) ∨ (P ∧ ¬Q)
2. P ∧ (Q ∨ ¬Q) (distributiivsuse omadus)
3. P ∧ t (Q ∨ ¬Q on tautoloogia, seega asendame selle tähisega t)
4. P (konjunktsioon tõesega annab alati operandi enda)

Seega selle asemel, et ehitada skeem, mis realiseerib (P ∧ Q) ∨ (P ∧ ¬Q), piisab lihtsast skeemist, mis väljastab sisendi P väärtuse. See vähendab oluliselt skeemi keerukust ja ressursivajadust.

## Kokkuvõte

Normaalkujud on lausearvutuses olulised standardformaadid, mis võimaldavad analüüsida ja võrrelda erinevaid valemeid ühtsel viisil. Disjunktiivne normaalkuju (DNK) on konjunktsioonide disjunktsioon, konjunktiivne normaalkuju (KNK) on disjunktsioonide konjunktsioon.

Täielikud normaalkujud (TDNK ja TKNK) on erijuhud, kus iga lihtkonjunktsioon või lihtdisjunktsioon sisaldab kõiki vaadeldavaid muutujaid. TDNK näitab otseselt, milliste muutujate väärtuste korral on valem tõene, samas kui TKNK näitab, milliste väärtuste korral valem on väär.

Normaalkujusid kasutatakse laialdaselt loogikaskeemide disainis, automaatses teoreemitõestamises ja SAT-probleemide lahendamisel. Nende leidmiseks saab kasutada kas algebralist teisendamist või tõeväärtustabeleid. ¬Z) ∨ (X ∧ ¬Y ∧ ¬Z)

Selgitame seda sammu detailsemalt. Esimese lihtkonjunktsiooni X ∧ Y täiendamiseks:
- X ∧ Y ≡ X ∧ Y ∧ (Z ∨ ¬Z) ≡ (X ∧ Y ∧ Z) ∨ (X ∧ Y ∧ ¬Z)

Teise lihtkonjunktsiooni X ∧ ¬Z täiendamiseks:
- X ∧ ¬Z ≡ X ∧ ¬Z ∧ (Y ∨ ¬Y) ≡ (X ∧ Y ∧ ¬Z) ∨ (X ∧ ¬Y ∧ ¬Z)

Kombineerides ja eemaldades korduvad liikmed, saame:
(X ∧ Y ∧ Z) ∨ (X ∧ Y ∧ ¬Z) ∨ (X ∧ ¬Y ∧ ¬Z)

#### 2. Tõeväärtustabeli abil

Teine, sageli lihtsam meetod TDNK leidmiseks on kasutada tõeväärtustabelit:

1. Koostame valemi tõeväärtustabeli.
2. Valime kõik read, kus valemi tõeväärtus on t (tõene).
3. Iga sellise rea jaoks moodustame täieliku lihtkonjunktsiooni.
4. TDNK on kõigi nende täielike lihtkonjunktsioonide disjunktsioon.

**Näide:**
Leiame valemi X ∧ (Y ∨ ¬Z) TDNK tõeväärtustabeli abil.

| X | Y | Z | Y ∨ ¬Z | X ∧ (Y ∨ ¬Z) |
|---|---|---|--------|--------------|
| t | t | t | t      | t            |
| t | t | v | t      | t            |
| t | v | t | v      | v            |
| t | v | v | t      | t            |
| v | t | t | t      | v            |
| v | t | v | t      | v            |
| v | v | t | v      | v            |
| v | v | v | t      | v            |

Valemi tõeväärtus on tõene ridades 1, 2 ja 4, mis vastavad väärtustele:
- X = t, Y = t, Z = t
- X = t, Y = t, Z = v
- X = t, Y = v, Z = v

Seega on TDNK:
(X ∧ Y ∧ Z) ∨ (X ∧ Y ∧