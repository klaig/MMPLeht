# Predikaatvalemite eitamine

## Sissejuhatus eitamisse predikaatarvutuses

Predikaatvalemite eitamine on oluline oskus, mis võimaldab meil väljendada väite vastupidist tähendust, kontrollida arutluskäikude korrektsust või sõnastada teoreemide ekvivalentseid vorme. Erinevalt lausearvutusest, kus eitamine tähendab lihtsalt eituse sümboli ¬ lisamist väitele, on predikaatarvutuses eitamine keerulisem, eriti kui väide sisaldab kvantoreid.

Õppides predikaatvalemite eitamist, omandame olulise tööriista matemaatilises loogikas, mis aitab meil täpsemalt mõista väidete tähendust ja nende vastastikuseid seoseid.

## Kvantorite eitamine ja De Morgani seadused

Üks olulisemaid reegleid predikaatvalemite eitamisel on **De Morgani seadused kvantoritele**. Need kirjeldavad, kuidas eitus mõjutab kvantorite tähendust.

### Üldisuskvantori (∀) eitamine

Väite "iga objekti kohta kehtib omadus P" eituseks on "leidub objekt, mille kohta ei kehti omadus P". Formaalselt:

**¬(∀x P(x)) ≡ ∃x ¬P(x)**

### Olemasolukvantori (∃) eitamine

Väite "leidub objekt, mille kohta kehtib omadus P" eituseks on "iga objekti kohta ei kehti omadus P". Formaalselt:

**¬(∃x P(x)) ≡ ∀x ¬P(x)**

### Näited kvantorite eitamisest

**Näide 1:** Eitame väidet "Kõik tudengid on tublid."
- Originaalväide: ∀x (Tudeng(x) → Tubli(x))
- Eitus: ¬(∀x (Tudeng(x) → Tubli(x))) ≡ ∃x ¬(Tudeng(x) → Tubli(x))

Kuna implikatsiooni eitamine on ¬(A → B) ≡ A ∧ ¬B, saame:
- Eitus: ∃x (Tudeng(x) ∧ ¬Tubli(x))

Tõlgendus: "Leidub tudeng, kes ei ole tubli."

**Näide 2:** Eitame väidet "Leidub kass, kes oskab ujuda."
- Originaalväide: ∃x (Kass(x) ∧ OskabUjuda(x))
- Eitus: ¬(∃x (Kass(x) ∧ OskabUjuda(x))) ≡ ∀x ¬(Kass(x) ∧ OskabUjuda(x))

Kuna konjunktsiooni eitamine on ¬(A ∧ B) ≡ ¬A ∨ ¬B, saame:
- Eitus: ∀x (¬Kass(x) ∨ ¬OskabUjuda(x)) ≡ ∀x (Kass(x) → ¬OskabUjuda(x))

Tõlgendus: "Ükski kass ei oska ujuda."

## Mitme kvantoriga valemite eitamine

Kui valem sisaldab mitut kvantorit, tuleb eitada iga kvantorit järjest, alustades kõige välimisest.

### Üldine protseduur mitme kvantoriga valemi eitamiseks

1. Vii eitus vahetult valemi ette (juhul kui see pole juba seal)
2. Vii eitus läbi kvantorite, muutes iga ∀ kvantorit ∃-ks ja vastupidi
3. Vii eitus läbi loogiliste tehete, kasutades lausearvutuse eitamisreegleid
4. Lihtsusta tulemus, kui võimalik

### Näited mitme kvantoriga valemite eitamisest

**Näide 1:** Eitame väidet "Iga arvu kohta leidub temast suurem arv."
- Originaalväide: ∀x ∃y (y > x)
- Eitus: ¬(∀x ∃y (y > x)) ≡ ∃x ¬(∃y (y > x)) ≡ ∃x ∀y ¬(y > x) ≡ ∃x ∀y (y ≤ x)

Tõlgendus: "Leidub arv, mis on suurem või võrdne kõigist teistest arvudest."

**Näide 2:** Eitame väidet "Leidub inimene, kes meeldib kõigile."
- Originaalväide: ∃x ∀y (Meeldib(x, y))
- Eitus: ¬(∃x ∀y (Meeldib(x, y))) ≡ ∀x ¬(∀y (Meeldib(x, y))) ≡ ∀x ∃y ¬(Meeldib(x, y))

Tõlgendus: "Iga inimese kohta leidub keegi, kellele ta ei meeldi."

## Keerukate valemite eitamine

Keerukate valemite eitamisel kombineerime kvantoritega seotud eitamisreegleid ja lauseloogika eitamisreegleid.

### Samm-sammuline näide

Eitame väidet "Iga inimene on selline, et kui ta on õpetaja, siis ta õpetab vähemalt ühte õpilast."

1. Originaalväide: ∀x (Inimene(x) → (Õpetaja(x) → ∃y (Õpilane(y) ∧ Õpetab(x, y))))

2. Kvantorite eitamine:
   - ¬(∀x (...)) ≡ ∃x ¬(...)

3. Implikatsiooni eitamine:
   - ¬(A → B) ≡ A ∧ ¬B

4. Rakendame eitamisreegleid:
   - ¬(∀x (Inimene(x) → (Õpetaja(x) → ∃y (Õpilane(y) ∧ Õpetab(x, y)))))
   - ≡ ∃x ¬(Inimene(x) → (Õpetaja(x) → ∃y (Õpilane(y) ∧ Õpetab(x, y))))
   - ≡ ∃x (Inimene(x) ∧ ¬(Õpetaja(x) → ∃y (Õpilane(y) ∧ Õpetab(x, y))))
   - ≡ ∃x (Inimene(x) ∧ (Õpetaja(x) ∧ ¬(∃y (Õpilane(y) ∧ Õpetab(x, y)))))
   - ≡ ∃x (Inimene(x) ∧ Õpetaja(x) ∧ ∀y ¬(Õpilane(y) ∧ Õpetab(x, y)))
   - ≡ ∃x (Inimene(x) ∧ Õpetaja(x) ∧ ∀y (¬Õpilane(y) ∨ ¬Õpetab(x, y)))
   - ≡ ∃x (Inimene(x) ∧ Õpetaja(x) ∧ ∀y (Õpilane(y) → ¬Õpetab(x, y)))

5. Tõlgendus: "Leidub inimene, kes on õpetaja, aga kes ei õpeta ühtegi õpilast."

## Eitamise kasutamine matemaatilistes tõestustes

Eitamine on oluline tööriist matemaatikas, eriti matemaatilise analüüsi mõistete defineerimisel.

### Pidevuse ja piirväärtusetega seotud näited

**Näide: Funktsiooni pidevuse eitamine**

Funktsiooni f pidevust punktis a defineeritakse:
- ∀ε > 0 ∃δ > 0 ∀x (|x - a| < δ → |f(x) - f(a)| < ε)

Funktsiooni mittepidevus on:
- ¬(∀ε > 0 ∃δ > 0 ∀x (|x - a| < δ → |f(x) - f(a)| < ε))
- ≡ ∃ε > 0 ¬(∃δ > 0 ∀x (|x - a| < δ → |f(x) - f(a)| < ε))
- ≡ ∃ε > 0 ∀δ > 0 ¬(∀x (|x - a| < δ → |f(x) - f(a)| < ε))
- ≡ ∃ε > 0 ∀δ > 0 ∃x (|x - a| < δ ∧ |f(x) - f(a)| ≥ ε)

Tõlgendus: "Leidub positiivne ε, et ükskõik kui väikese positiivse δ korral leidub punkt x, mis on lähemal punktile a kui δ, kuid f(x) erineb f(a)-st vähemalt ε võrra."

### Vastuväitelised tõestused

Eitamist kasutatakse sageli **vastuväitelistes tõestustes** (proof by contradiction), kus eeldatakse väite eituse tõesust ja näidatakse, et see viib vastuoluni.

**Näide: √2 irratsionaalsuse tõestus**

Väide: √2 on irratsionaalarv.

Tõestus vastuväiteliselt:
1. Eeldame, et √2 ei ole irratsionaalarv (ehk √2 on ratsionaalarv).
2. Siis leiduvad naturaalarvud p ja q (ilma ühise tegurita), et √2 = p/q.
3. Seega 2 = p²/q², ehk 2q² = p².
4. Järelikult p² on paarisarv, seega p on paarisarv (kuna paaritu arvu ruut on paaritu).
5. Kui p on paarisarv, siis leidub naturaalarv k, et p = 2k.
6. Asendades: 2q² = (2k)² = 4k², ehk q² = 2k².
7. Järelikult q² on paarisarv, seega q on paarisarv.
8. Kuna nii p kui q on paarisarvud, on neil ühine tegur 2, mis on vastuolus eeldusega.
9. Seega algne eeldus on väär ja √2 on irratsionaalarv.

## Praktilised näited eitamise kasutamisest

### Näide 1: Matemaatilised definitsioonid

**Funktsioon f pole üksühene:**
- Originaalväide (üksühesus): ∀x ∀y ((x ≠ y) → (f(x) ≠ f(y)))
- Eitus: ¬(∀x ∀y ((x ≠ y) → (f(x) ≠ f(y))))
- ≡ ∃x ∃y ¬((x ≠ y) → (f(x) ≠ f(y)))
- ≡ ∃x ∃y ((x ≠ y) ∧ ¬(f(x) ≠ f(y)))
- ≡ ∃x ∃y ((x ≠ y) ∧ (f(x) = f(y)))

Tõlgendus: "Leiduvad erinevad x ja y, et f(x) = f(y)."

### Näide 2: Igapäevaelu situatsioonid

**Lause: "Kõik õpilased sooritasid kõik eksamid edukalt."**
- Originaalväide: ∀x ∀y ((Õpilane(x) ∧ Eksam(y)) → Sooritas(x, y))

**Millised on võimalikud eitused ja nende tähendused?**

1. "Mitte kõik õpilased sooritasid kõik eksamid edukalt."
   - ¬(∀x ∀y ((Õpilane(x) ∧ Eksam(y)) → Sooritas(x, y)))
   - ≡ ∃x ∃y ((Õpilane(x) ∧ Eksam(y)) ∧ ¬Sooritas(x, y))

   Tõlgendus: "Leidub õpilane ja eksam, mida see õpilane ei sooritanud."

2. "Ükski õpilane ei sooritanud ühtegi eksamit edukalt."
   - ∀x ∀y ((Õpilane(x) ∧ Eksam(y)) → ¬Sooritas(x, y))

   See pole eitus, vaid palju tugevam väide kui algse väite eitamine.

3. "Mitte ükski õpilane ei sooritanud kõiki eksameid edukalt."
   - ∀x (Õpilane(x) → ¬(∀y (Eksam(y) → Sooritas(x, y))))
   - ≡ ∀x (Õpilane(x) → ∃y (Eksam(y) ∧ ¬Sooritas(x, y)))

   Tõlgendus: "Iga õpilase kohta leidub eksam, mida ta ei sooritanud."

   See pole algse väite täielik eitus, vaid tugevam väide kui esimene variant.

## Levinud vead eitamisel

Predikaatvalemite eitamisel on mõned tüüpilised vead, mida tuleks vältida:

### 1. Kvantorite valesti muutmine

**Vale:** ¬(∀x P(x)) ≡ ∀x ¬P(x)  
**Õige:** ¬(∀x P(x)) ≡ ∃x ¬P(x)

**Vale:** ¬(∃x P(x)) ≡ ∃x ¬P(x)  
**Õige:** ¬(∃x P(x)) ≡ ∀x ¬P(x)

### 2. Implikatsiooni eitamise vale

**Vale:** ¬(A → B) ≡ ¬A → ¬B  
**Õige:** ¬(A → B) ≡ A ∧ ¬B

### 3. Kvantorite järjekorra ebaõige muutmine

**Vale:** ¬(∀x ∃y P(x,y)) ≡ ∀y ∃x ¬P(x,y)  
**Õige:** ¬(∀x ∃y P(x,y)) ≡ ∃x ∀y ¬P(x,y)

### 4. Vaba ja seotud muutujate vale käsitlemine

**Probleem:** Kui valemis on nii vabu kui ka seotud muutujaid, tuleb hoolikalt jälgida, millised muutujad on kvantoriga seotud ja milliseid mitte.

**Näide:** 
Eitame valemit ∀x (P(x) ∧ Q(x,y)), kus y on vaba muutuja.
¬(∀x (P(x) ∧ Q(x,y))) ≡ ∃x ¬(P(x) ∧ Q(x,y)) ≡ ∃x (¬P(x) ∨ ¬Q(x,y))

Vaba muutuja y jääb ka eitatud valemis vabaks.

## Praktilised meetodid eitamise harjutamiseks

### 1. Samm-sammuline lähenemine

Keeruliste valemite eitamisel on kasulik järgida kindlat järjekorda:
1. Vii eitus kõige sisemale tasemele, muutes kvantorid (∀ → ∃, ∃ → ∀)
2. Rakenda lauseloogika eitamisreegleid valemiosadele
3. Lihtsusta tulemus, kui võimalik

### 2. Tabel kvantorite eitamise jaoks

|  Originaal   |    Eitus     |
|--------------|--------------|
|  ∀x P(x)     |  ∃x ¬P(x)    |
|  ∃x P(x)     |  ∀x ¬P(x)    |
| ∀x ∃y P(x,y) | ∃x ∀y ¬P(x,y) |
| ∃x ∀y P(x,y) | ∀x ∃y ¬P(x,y) |

### 3. Keelelise tõlgenduse kasutamine

Sageli aitab eituse õigesti moodustamisel väite tavakeelne tõlgendamine:

- "Kõik on P" eitus on "Mõned pole P"
- "Mõned on P" eitus on "Ükski pole P" või "Kõik pole P"
- "Iga X kohta leidub Y" eitus on "Leidub selline X, et ükski Y ei sobi"

## Eitamine ja loomuliku keele mitmeti mõistetavus

Loomulik keel võib olla mitmeti mõistetav, mistõttu predikaatvalemi korrektne formaalne eitamine aitab meil paremini mõista väidete täpset tähendust.

**Näide:** Vaatame lauset "Kõik rebased ei ole kavalpead."

See lause on mitmeti mõistetav:
1. "Ükski rebane pole kaval" – ∀x (Rebane(x) → ¬Kaval(x))
2. "Mõni rebane ei ole kaval" – ¬∀x (Rebane(x) → Kaval(x)) ≡ ∃x (Rebane(x) ∧ ¬Kaval(x))

Predikaatarvutus aitab meil neid kahte tõlgendust selgelt eristada.

## Kokkuvõte

Predikaatvalemite eitamine on oluline oskus, mis võimaldab meil täpselt väljendada väidete eitusi ning mõista kvantorite ja loogiliste tehete koostoimimist. Peamised reeglid, mida meeles pidada:

1. Üldisuskvantori eitus muutub olemasolukvantoriks: ¬(∀x P(x)) ≡ ∃x ¬P(x)
2. Olemasolukvantori eitus muutub üldisuskvantoris: ¬(∃x P(x)) ≡ ∀x ¬P(x)
3. Mitme kvantoriga valemite eitamisel tuleb läbida kõik kvantorid järjest, muutes nende tüüpi
4. Eituse järel tuleb rakendada sobivaid lauseloogika eitamisreegleid

Predikaatvalemite eitamise oskust saab rakendada mitmel pool:
- Matemaatiliste definitsioonide ja teoreemide formuleerimisel
- Vastuväitelisel tõestamisel
- Loomuliku keele väidete formaalseks muutmisel
- Loogiliste järelduste kontrollimisel

Eitamise meisterlikkus tuleb praktikast, seega on oluline lahendada palju erinevaid ülesandeid, mis hõlmavad erinevaid kvantorite kombinatsioone ja loogiliste tehete struktuure.