# Lausearvutuse harjutusülesanded

Selles failis on koondatud kõik lausearvutuse teemade harjutusülesanded koos lahendustega. Ülesanded on grupeeritud teemade kaupa.

## 1. Põhimõisted

### Ülesanne 1.1
Määra, millised järgmistest on lausearvutuse laused. Põhjenda oma vastust.
   a. "Arv π on irratsionaalne."
   b. "Osta mulle piima."
   c. "Kui arv on paarisarv, siis ta jagub 2-ga."
   d. "Mis on sinu nimi?"
   e. "f(x) = x² + 2x - 3"

**Vastused:**
   a. On lause (tõene), sest sellel on kindel tõeväärtus.
   b. Ei ole lause (käsklus), sest käsklusel pole tõeväärtust.
   c. On lause (tõene), sest sellel on kindel tõeväärtus.
   d. Ei ole lause (küsimus), sest küsimusel pole tõeväärtust.
   e. Ei ole lause (avaldis muutujaga), sest selle tõeväärtus sõltub muutuja x väärtusest.

### Ülesanne 1.2
Otsusta, millised järgmistest lausetest on tõesed ja millised väärad:
   a. "Arv 17 on paarisarv."
   b. "Kui 2 + 2 = 5, siis Tallinn on Eesti pealinn."
   c. "2 + 2 = 4 või Tallinn on Läti pealinn."
   d. "2 + 2 = 4 ja Tallinn on Läti pealinn."

**Vastused:**
   a. Väär (v), sest 17 on paaritu arv.
   b. Tõene (t), sest väär eeldus teeb implikatsiooni tõeseks. Implikatsioon A ⇒ B on väär ainult siis, kui A on tõene ja B on väär.
   c. Tõene (t), sest vähemalt üks osa (2 + 2 = 4) on tõene, seega kogu disjunktsioon on tõene.
   d. Väär (v), sest üks osa (Tallinn on Läti pealinn) on väär, seega kogu konjunktsioon on väär.

### Ülesanne 1.3
Määra, millised järgmistest lausetest on tautoloogiad, millised kontradiktsioonid ja millised ei kumbki:
   a. "Maa on ümmargune või Maa ei ole ümmargune."
   b. "Kui täna sajab, siis täna sajab või paistab päike."
   c. "Täna sajab ja täna paistab päike ja täna ei saja."
   d. "Kui arv on algarv, siis ta ei jagu ühegi endast väiksema naturaalarvuga peale 1."

**Vastused:**
   a. Tautoloogia (vorm A ∨ ¬A), sest see on tõene iga võimaliku tõeväärtuse korral.
   b. Tautoloogia (vorm A ⇒ (A ∨ B)), sest see on tõene iga võimaliku tõeväärtuse korral.
   c. Kontradiktsioon (sest sisaldab A ∧ ¬A), sest see on väär iga võimaliku tõeväärtuse korral.
   d. Tautoloogia (algarvu definitsioon), sest see on tõene iga võimaliku tõeväärtuse korral.

## 2. Tehted

### Ülesanne 2.1
Määra järgmiste lausete tõeväärtused, kui A = t, B = v, C = t:
   a) A ∧ (B ∨ C)
   b) ¬A ∨ B
   c) (A ⇒ B) ∧ C
   d) (A ⇔ B) ∨ ¬C

**Vastused:**
   a) A ∧ (B ∨ C) = t ∧ (v ∨ t) = t ∧ t = t
   b) ¬A ∨ B = v ∨ v = v
   c) (A ⇒ B) ∧ C = (t ⇒ v) ∧ t = v ∧ t = v
   d) (A ⇔ B) ∨ ¬C = (t ⇔ v) ∨ ¬t = v ∨ v = v

### Ülesanne 2.2
Millised järgnevatest lausetest on samaväärsed?
   a) ¬(A ∧ B)
   b) ¬A ∨ ¬B
   c) ¬A ∧ ¬B
   d) A ⇒ ¬B

**Vastused:**
Samaväärsed on a) ja b), mis vastavad De Morgani seadusele: ¬(A ∧ B) ≡ ¬A ∨ ¬B
Lisaks on samaväärsed valemid d) A ⇒ ¬B ja a) ¬(A ∧ B), sest A ⇒ ¬B ≡ ¬A ∨ ¬B ≡ ¬(A ∧ B)

### Ülesanne 2.3
Väljenda järgnevad laused lausearvutuse valemitena:
   a) Kui sajab vihma ja ma ei võta vihmavarju, siis ma saan märjaks.
   b) Selleks, et eksam sooritada, on tarvis ja piisav, et saada vähemalt 50 punkti.
   c) Ma lähen kinno siis ja ainult siis, kui film on hea ja pilet pole kallis.

**Vastused:**
   a) V ∧ ¬U ⇒ M, kus V: "Sajab vihma", U: "Ma võtan vihmavarju", M: "Ma saan märjaks"
   b) E ⇔ P, kus E: "Eksam on sooritatud", P: "Sain vähemalt 50 punkti"
   c) K ⇔ (H ∧ ¬K), kus K: "Ma lähen kinno", H: "Film on hea", K: "Pilet on kallis"

## 3. Tõeväärtustabelid

### Ülesanne 3.1
Koostage tõeväärtustabel valemile (X ∨ Y) ⇒ (X ∧ Z).

**Lahendus:**

| X | Y | Z | X ∨ Y | X ∧ Z | (X ∨ Y) ⇒ (X ∧ Z) |
|---|---|---|-------|-------|---------------------|
| t | t | t | t     | t     | t                   |
| t | t | v | t     | v     | v                   |
| t | v | t | t     | t     | t                   |
| t | v | v | t     | v     | v                   |
| v | t | t | t     | v     | v                   |
| v | t | v | t     | v     | v                   |
| v | v | t | v     | v     | t                   |
| v | v | v | v     | v     | t                   |

### Ülesanne 3.2
Otsustage tõeväärtustabeli abil, kas järgmised valemid on tautoloogiad, kontradiktsioonid või ei kumbki:
a) (X ⇒ Y) ⇔ (¬Y ⇒ ¬X)
b) X ∧ Y ⇒ X ∨ Y
c) (X ⇒ Y) ∧ (Y ⇒ Z) ⇒ (X ⇒ Z)

**Lahendus a:**

| X | Y | X ⇒ Y | ¬Y | ¬X | ¬Y ⇒ ¬X | (X ⇒ Y) ⇔ (¬Y ⇒ ¬X) |
|---|---|-------|-----|-----|---------|------------------------|
| t | t | t     | v   | v   | t       | t                      |
| t | v | v     | t   | v   | v       | t                      |
| v | t | t     | v   | t   | t       | t                      |
| v | v | t     | t   | t   | t       | t                      |

Valem on tautoloogia, sest valemi veerus on ainult tõesed väärtused.

**Lahendus b:**

| X | Y | X ∧ Y | X ∨ Y | X ∧ Y ⇒ X ∨ Y |
|---|---|-------|-------|---------------|
| t | t | t     | t     | t             |
| t | v | v     | t     | t             |
| v | t | v     | t     | t             |
| v | v | v     | v     | t             |

Valem on tautoloogia, sest valemi veerus on ainult tõesed väärtused.

**Lahendus c:**

| X | Y | Z | X ⇒ Y | Y ⇒ Z | (X ⇒ Y) ∧ (Y ⇒ Z) | X ⇒ Z | ((X ⇒ Y) ∧ (Y ⇒ Z)) ⇒ (X ⇒ Z) |
|---|---|---|-------|-------|-------------------|-------|--------------------------------|
| t | t | t | t     | t     | t                 | t     | t                              |
| t | t | v | t     | v     | v                 | v     | t                              |
| t | v | t | v     | t     | v                 | t     | t                              |
| t | v | v | v     | t     | v                 | v     | t                              |
| v | t | t | t     | t     | t                 | t     | t                              |
| v | t | v | t     | v     | v                 | t     | t                              |
| v | v | t | t     | t     | t                 | t     | t                              |
| v | v | v | t     | t     | t                 | t     | t                              |

Valem on tautoloogia, sest valemi veerus on ainult tõesed väärtused.

### Ülesanne 3.3
Kontrollige tõeväärtustabeli abil, kas valemist X ⇒ Y järeldub valem ¬X ∨ Y.

**Lahendus:**

| X | Y | X ⇒ Y | ¬X | ¬X ∨ Y |
|---|---|-------|-----|---------|
| t | t | t     | v   | t       |
| t | v | v     | v   | v       |
| v | t | t     | t   | t       |
| v | v | t     | t   | t       |

Näeme, et igal real, kus X ⇒ Y on tõene (read 1, 3, 4), on ka ¬X ∨ Y tõene. Kuna aga teisel real mõlemad valemid on väärad, siis valemite tõeväärtustabelid on identsed. Seega valemist X ⇒ Y järeldub valem ¬X ∨ Y, ning tegelikult need valemid on samaväärsed.

### Ülesanne 3.4
Ülesandepüstitus: Sissepääsukontrolli süsteemis on järgmised tingimused:
- A: "Kasutajal on võti"
- B: "Kasutaja tunneb parooli"
- C: "Kasutaja on töötaja"

Uksest pääseb sisse tingimusel: (A ∧ B) ∨ C (ehk kui kasutajal on võti ja ta tunneb parooli, või kui kasutaja on töötaja).

Kontrollige tõeväärtustabeli abil, milliste tingimuste kombinatsioonide korral saab kasutaja uksest sisse.

**Lahendus:**

| A | B | C | A ∧ B | (A ∧ B) ∨ C | Kas pääseb sisse? |
|---|---|---|-------|-------------|------------------|
| t | t | t | t     | t           | Jah              |
| t | t | v | t     | t           | Jah              |
| t | v | t | v     | t           | Jah              |
| t | v | v | v     | v           | Ei               |
| v | t | t | v     | t           | Jah              |
| v | t | v | v     | v           | Ei               |
| v | v | t | v     | t           | Jah              |
| v | v | v | v     | v           | Ei               |

Kasutaja pääseb uksest sisse järgmistel juhtudel:
1. Tal on võti JA ta tunneb parooli JA ta on töötaja
2. Tal on võti JA ta tunneb parooli JA ta ei ole töötaja
3. Tal on võti JA ta ei tunne parooli JA ta on töötaja
4. Tal ei ole võtit JA ta tunneb parooli JA ta on töötaja
5. Tal ei ole võtit JA ta ei tunne parooli JA ta on töötaja

Teisisõnu, kui kasutaja on töötaja, siis tal ei pea olema võtit ega teadma parooli. Kui aga kasutaja ei ole töötaja, siis tal peab olema nii võti kui ka teadma parooli.

## 4. Samaväärsused

### Ülesanne 4.1
Tõestage, et valemid (X ⇒ Y) ∧ (X ⇒ Z) ja X ⇒ (Y ∧ Z) on samaväärsed, kasutades samaväärsusseoseid.

**Lahendus:**
1. (X ⇒ Y) ∧ (X ⇒ Z)
2. (¬X ∨ Y) ∧ (¬X ∨ Z) (implikatsiooni avaldumine)
3. ¬X ∨ (Y ∧ Z) (distributiivsuse omadus)
4. X ⇒ (Y ∧ Z) (implikatsiooni avaldumine)

Seega (X ⇒ Y) ∧ (X ⇒ Z) ≡ X ⇒ (Y ∧ Z).

### Ülesanne 4.2
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

### Ülesanne 4.3
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

## 5. Järeldumine

### Ülesanne 5.1
Kontrollige, kas järgmised järeldumised kehtivad:
a) P ⇒ Q, Q ⇒ R ⊨ P ⇒ R
b) P ∨ Q, P ⇒ R, Q ⇒ R ⊨ R
c) P ⇒ Q, Q ⇒ P ⊨ P ⇔ Q

**Lahendus a:**
Kontrollime, kas valem (P ⇒ Q) ∧ (Q ⇒ R) ⇒ (P ⇒ R) on tautoloogia.

| P | Q | R | P ⇒ Q | Q ⇒ R | P ⇒ R | (P ⇒ Q) ∧ (Q ⇒ R) | ((P ⇒ Q) ∧ (Q ⇒ R)) ⇒ (P ⇒ R) |
|---|---|---|-------|-------|-------|-------------------|--------------------------------|
| t | t | t | t     | t     | t     | t                 | t                              |
| t | t | v | t     | v     | v     | v                 | t                              |
| t | v | t | v     | t     | t     | v                 | t                              |
| t | v | v | v     | t     | v     | v                 | t                              |
| v | t | t | t     | t     | t     | t                 | t                              |
| v | t | v | t     | v     | t     | v                 | t                              |
| v | v | t | t     | t     | t     | t                 | t                              |
| v | v | v | t     | t     | t     | t                 | t                              |

Kuna viimases veerus on kõik väärtused tõesed, on valem tautoloogia, seega järeldumine kehtib.

**Lahendus b:**
Kontrollime, kas valem (P ∨ Q) ∧ (P ⇒ R) ∧ (Q ⇒ R) ⇒ R on tautoloogia.

| P | Q | R | P ∨ Q | P ⇒ R | Q ⇒ R | (P ∨ Q) ∧ (P ⇒ R) ∧ (Q ⇒ R) | ((P ∨ Q) ∧ (P ⇒ R) ∧ (Q ⇒ R)) ⇒ R |
|---|---|---|-------|-------|-------|----------------------------|----------------------------------|
| t | t | t | t     | t     | t     | t                          | t                                |
| t | t | v | t     | v     | v     | v                          | t                                |
| t | v | t | t     | t     | t     | t                          | t                                |
| t | v | v | t     | v     | t     | v                          | t                                |
| v | t | t | t     | t     | t     | t                          | t                                |
| v | t | v | t     | t     | v     | v                          | t                                |
| v | v | t | v     | t     | t     | v                          | t                                |
| v | v | v | v     | t     | t     | v                          | t                                |

Kuna viimases veerus on kõik väärtused tõesed, on valem tautoloogia, seega järeldumine kehtib.

**Lahendus c:**
Kontrollime, kas valem (P ⇒ Q) ∧ (Q ⇒ P) ⇒ (P ⇔ Q) on tautoloogia.

Teame, et P ⇔ Q ≡ (P ⇒ Q) ∧ (Q ⇒ P), seega kontrollitav valem on kujul (P ⇒ Q) ∧ (Q ⇒ P) ⇒ (P ⇒ Q) ∧ (Q ⇒ P), mis on ilmselgelt tautoloogia. Järelikult järeldumine kehtib.

### Ülesanne 5.2
Määrake, kas järgmised arutlused on loogiliselt korrektsed:

a) Kui Mari on õpetaja, siis ta on tark.
   Mari ei ole õpetaja.
   Järelikult, Mari ei ole tark.

b) Kui sajab vihma, siis tänav on märg.
   Tänav on märg.
   Järelikult, sajab vihma.

c) Kõik linnud on lendavad olendid.
   Kõik kanad on linnud.
   Järelikult, kõik kanad on lendavad olendid.

**Lahendus a:**
Tähistame:
- P: "Mari on õpetaja"
- Q: "Mari on tark"

Arutlus on kujul:
1. P ⇒ Q
2. ¬P
3. ¬Q (järeldus)

Kontrollime, kas P ⇒ Q, ¬P ⊨ ¬Q:

| P | Q | P ⇒ Q | ¬P | ¬Q | (P ⇒ Q) ∧ ¬P | ((P ⇒ Q) ∧ ¬P) ⇒ ¬Q |
|---|---|-------|-----|-----|---------------|---------------------|
| t | t | t     | v   | v   | v             | t                   |
| t | v | v     | v   | t   | v             | t                   |
| v | t | t     | t   | v   | t             | v                   |
| v | v | t     | t   | t   | t             | t                   |

Kuna viimases veerus on väär väärtus (kolmas rida), ei ole valem tautoloogia, seega järeldumine ei kehti ja arutlus ei ole loogiliselt korrektne.

**Lahendus b:**
Tähistame:
- P: "Sajab vihma"
- Q: "Tänav on märg"

Arutlus on kujul:
1. P ⇒ Q
2. Q
3. P (järeldus)

Kontrollime, kas P ⇒ Q, Q ⊨ P:

| P | Q | P ⇒ Q | (P ⇒ Q) ∧ Q | ((P ⇒ Q) ∧ Q) ⇒ P |
|---|---|-------|-------------|-------------------|
| t | t | t     | t           | t                 |
| t | v | v     | v           | t                 |
| v | t | t     | t           | v                 |
| v | v | t     | v           | t                 |

Kuna viimases veerus on väär väärtus (kolmas rida), ei ole valem tautoloogia, seega järeldumine ei kehti ja arutlus ei ole loogiliselt korrektne.

**Lahendus c:**
See arutlus kuulub predikaatloogikasse, mitte lausearvutusse, kuid võime siiski analüüsida selle loogilist struktuuri.

Arutlus on kujul:
1. Kõik linnud on lendavad olendid.
2. Kõik kanad on linnud.
3. Kõik kanad on lendavad olendid. (järeldus)

See on klassikaline süllogismi vorm, mis on loogiliselt korrektne. Kui kõik A on B ja kõik C on A, siis kõik C on B.

Märkus: Reaalses maailmas on see järeldus väär, sest kanad ei lenda hästi, kuid loogiliselt on arutlus korrektne, eeldusel et eeldused on tõesed.

## 6. Valemite teisendamine

### Ülesanne 6.1
Teisendage valem ¬(P ⇒ (Q ∧ R)) nii, et see sisaldaks ainult tehteid ¬, ∧, ∨.

**Lahendus:**
1. ¬(P ⇒ (Q ∧ R))
2. ¬(¬P ∨ (Q ∧ R)) (implikatsiooni eemaldamine)
3. ¬¬P ∧ ¬(Q ∧ R) (De Morgani seadus disjunktsioonile)
4. P ∧ (¬Q ∨ ¬R) (De Morgani seadus konjunktsioonile ja kahekordse eituse eemaldamine)
5. (P ∧ ¬Q) ∨ (P ∧ ¬R) (distributiivsuse omadus)

Seega, ¬(P ⇒ (Q ∧ R)) ≡ (P ∧ ¬Q) ∨ (P ∧ ¬R).

### Ülesanne 6.2
Teisendage valem (P ⇔ Q) ⇒ (P ∨ Q) disjunktiivsele normaalkujule.

**Lahendus:**
1. (P ⇔ Q) ⇒ (P ∨ Q)
2. ¬(P ⇔ Q) ∨ (P ∨ Q) (implikatsiooni eemaldamine)
3. ¬((P ⇒ Q) ∧ (Q ⇒ P)) ∨ (P ∨ Q) (ekvivalentsi eemaldamine)
4. (¬(P ⇒ Q) ∨ ¬(Q ⇒ P)) ∨ (P ∨ Q) (De Morgani seadus konjunktsioonile)
5. (¬(¬P ∨ Q) ∨ ¬(¬Q ∨ P)) ∨ (P ∨ Q) (implikatsiooni eemaldamine)
6. ((¬¬P ∧ ¬Q) ∨ (¬¬Q ∧ ¬P)) ∨ (P ∨ Q) (De Morgani seadus disjunktsioonile)
7. ((P ∧ ¬Q) ∨ (Q ∧ ¬P)) ∨ (P ∨ Q) (kahekordse eituse eemaldamine)

Lihtsustame edasi:
8. (P ∧ ¬Q) ∨ (Q ∧ ¬P) ∨ P ∨ Q
9. (P ∧ ¬Q) ∨ (Q ∧ ¬P) ∨ (P ∧ Q) ∨ (P ∧ ¬Q) ∨ (Q ∧ ¬P) ∨ (Q ∧ P)
10. (P ∧ Q) ∨ (P ∧ ¬Q) ∨ (Q ∧ ¬P)

See on disjunktiivne normaalkuju.

### Ülesanne 6.3
Teisendage valem P ⇒ (Q ⇒ R) nii, et see sisaldaks ainult ühte implikatsiooni.

**Lahendus:**
1. P ⇒ (Q ⇒ R)
2. P ⇒ (¬Q ∨ R) (implikatsiooni eemaldamine sisemisele implikatsioonile)
3. ¬P ∨ (¬Q ∨ R) (implikatsiooni eemaldamine välimisele implikatsioonile)
4. ¬P ∨ ¬Q ∨ R (disjunktsiooni assotsiatiivsus)
5. (¬P ∨ ¬Q) ∨ R
6. ¬(P ∧ Q) ∨ R (De Morgani seadus)
7. (P ∧ Q) ⇒ R (implikatsiooni taastamine)

Seega, P⇒ (Q ⇒ R) ≡ (P ∧ Q) ⇒ R.

## 7. Normaalkujud

### Ülesanne 7.1
Viige valem X ⇒ (Y ∨ Z) täielikule disjunktiivsele normaalkujule.

**Lahendus:**

1. Asendame implikatsiooni:
   X ⇒ (Y ∨ Z) ≡ ¬X ∨ (Y ∨ Z) ≡ ¬X ∨ Y ∨ Z

2. Disjunktiivse normaalkuju leidmiseks:
   ¬X ∨ Y ∨ Z
   
   See on juba disjunktiivsel normaalkujul, kuid mitte täielikul.

3. Täieliku disjunktiivse normaalkuju jaoks peame moodustama disjunktsiooni, kus iga liige on täielik lihtkonjunktsioon (sisaldab kõiki muutujaid kas eitatuna või ilma eituseta).

   ¬X ∨ Y ∨ Z ≡ 
   (¬X ∧ Y ∧ Z) ∨ (¬X ∧ Y ∧ ¬Z) ∨ (¬X ∧ ¬Y ∧ Z) ∨ (¬X ∧ ¬Y ∧ ¬Z) ∨ 
   (X ∧ Y ∧ Z) ∨ (X ∧ Y ∧ ¬Z) ∨ (X ∧ ¬Y ∧ Z)

4. Kontrollime tõeväärtustabeliga:

   | X | Y | Z | X ⇒ (Y ∨ Z) |
   |---|---|---|-------------|
   | t | t | t | t           |
   | t | t | v | t           |
   | t | v | t | t           |
   | t | v | v | v           |
   | v | t | t | t           |
   | v | t | v | t           |
   | v | v | t | t           |
   | v | v | v | t           |

   Valemi tõeväärtus on väär ainult reas X = t, Y = v, Z = v. Seega täielik disjunktiivne normaalkuju on:
   
   (¬X ∧ Y ∧ Z) ∨ (¬X ∧ Y ∧ ¬Z) ∨ (¬X ∧ ¬Y ∧ Z) ∨ (¬X ∧ ¬Y ∧ ¬Z) ∨ 
   (X ∧ Y ∧ Z) ∨ (X ∧ Y ∧ ¬Z) ∨ (X ∧ ¬Y ∧ Z)

### Ülesanne 7.2
Viige valem (X ∧ Y) ∨ (¬X ∧ Z) täielikule konjunktiivsele normaalkujule.

**Lahendus:**

1. Valem on juba disjunktiivsel normaalkujul. Viime selle täielikule konjunktiivsele normaalkujule, kasutades tõeväärtustabelit.

2. Koostame tõeväärtustabeli:

   | X | Y | Z | X ∧ Y | ¬X ∧ Z | (X ∧ Y) ∨ (¬X ∧ Z) |
   |---|---|---|-------|--------|---------------------|
   | t | t | t | t     | v      | t                   |
   | t | t | v | t     | v      | t                   |
   | t | v | t | v     | v      | v                   |
   | t | v | v | v     | v      | v                   |
   | v | t | t | v     | t      | t                   |
   | v | t | v | v     | v      | v                   |
   | v | v | t | v     | t      | t                   |
   | v | v | v | v     | v      | v                   |

3. Valemi tõeväärtus on väär ridades 3, 4, 6, 8. Moodustame iga rea jaoks täieliku lihtdisjunktsiooni, kus eitame literaale, mis on tõesed, ja jätame eitamata literaalid, mis on väärad:

   - (¬X ∨ Y ∨ ¬Z) (rida 3: X = t, Y = v, Z = t)
   - (¬X ∨ Y ∨ Z) (rida 4: X = t, Y = v, Z = v)
   - (X ∨ ¬Y ∨ Z) (rida 6: X = v, Y = t, Z = v)
   - (X ∨ Y ∨ Z) (rida 8: X = v, Y = v, Z = v)

4. TKNK on:
   (¬X ∨ Y ∨ ¬Z) ∧ (¬X ∨ Y ∨ Z) ∧ (X ∨ ¬Y ∨ Z) ∧ (X ∨ Y ∨ Z)

   See lihtsustub kujule:
   (¬X ∨ Y) ∧ (X ∨ Z)

### Ülesanne 7.3
Tõestage, et kui valemi F TDNK on G ja valemi F TKNK on H, siis G ja H on duaalsed (st G saadakse H-st, asendades ∧ sümbolid ∨ sümbolitega ja vastupidi ning eitades kõiki literaale).

**Lahendus:**
Kui F TDNK on G, siis G osutab täpselt nendele väärtustuskombinatsioonidele, mille korral F on tõene.
Kui F TKNK on H, siis H osutab täpselt nendele väärtustuskombinatsioonidele, mille korral F ei ole väär.

Olgu F̄ valemi F eitus. Siis F̄ on tõene parajasti siis, kui F on väär. Seega F̄ TDNK osutab täpselt nendele väärtustuskombinatsioonidele, mille korral F on väär.

TDNK konstrueerimisel võtame tõesed väärtustekombinatsioonid ja TKNK konstrueerimisel väldime vääri kombinatsioone. Seega F̄ TDNK ja F TKNK on duaalsed.

Kuna G on F TDNK ja H on F TKNK, siis G ja H on duaalsed.

## 8. Predikaatarvutus

### Ülesanne 8.1
Formaliseerige järgmised laused predikaatarvutuses:

a) Kõik tudengid õpivad matemaatikat.
b) Mõned raamatud on huvitavad.
c) Ükski kass ei ole inimene.
d) Kui number on paarisarv, siis ta jagub 2-ga.
e) Iga reaalarvu ruut on mittenegatiivne.

**Lahendused:**

a) ∀x ∈ D (T(x) → M(x)), kus 
   - D on kõigi inimeste hulk
   - T(x): "x on tudeng"
   - M(x): "x õpib matemaatikat"

b) ∃x ∈ D (R(x) ∧ H(x)), kus
   - D on kõigi asjade hulk
   - R(x): "x on raamat"
   - H(x): "x on huvitav"

c) ∀x ∈ D (K(x) → ¬I(x)) või ekvivalentselt ¬∃x ∈ D (K(x) ∧ I(x)), kus
   - D on kõigi olendite hulk
   - K(x): "x on kass"
   - I(x): "x on inimene"

d) ∀x ∈ Z (P(x) → J(x,2)), kus
   - P(x): "x on paarisarv"
   - J(x,y): "x jagub y-ga"

e) ∀x ∈ R (x² ≥ 0)

### Ülesanne 8.2
Formaliseerige järgmised matemaatilised väited:

a) Iga naturaalarvu ruut on suurem või võrdne kui arv ise.
b) Kahe järjestikuse naturaalarvu korrutis on alati paarisarv.
c) Leidub selline reaalarv, mille ruut on 2.
d) Iga positiivse reaalarvu jaoks leidub temast väiksem positiivne reaalarv.

**Lahendused:**

a) ∀x ∈ N (x² ≥ x)

b) ∀n ∈ N (P(n·(n+1))), kus
   - P(x): "x on paarisarv"
   Alternatiivselt: ∀n ∈ N (∃k ∈ N (n·(n+1) = 2k))

c) ∃x ∈ R (x² = 2)

d) ∀x ∈ R ((x > 0) → ∃y ∈ R (0 < y < x))

### Ülesanne 8.3
Andke järgmistele predikaatarvutuse valemitele loomulik tõlge eesti keelde:

a) ∀x ∈ D (I(x) → ∃y ∈ D (I(y) ∧ V(x,y))), kus
   - D on kõigi olendite hulk
   - I(x): "x on inimene"
   - V(x,y): "x vajab y-i"

b) ∀x ∈ D (K(x) → (∃y ∈ D (K(y) ∧ S(y,x)) ∨ ∃z ∈ D (H(z) ∧ S(z,x)))), kus
   - D on kõigi olendite hulk
   - K(x): "x on kass"
   - H(x): "x on inimene"
   - S(x,y): "x sööb y-i"

c) ¬∃x ∈ D (T(x) ∧ ∀y ∈ D (A(y) → L(x,y))), kus
   - D on kõigi inimeste ja õppeainete hulk
   - T(x): "x on tudeng"
   - A(y): "y on õppeaine"
   - L(x,y): "x läbis õppeaine y"

**Lahendused:**

a) "Iga inimene vajab mingit teist inimest."

b) "Iga kassi sööb kas mõni teine kass või mõni inimene."

c) "Pole ühtegi tudengit, kes oleks läbinud kõik õppeained." või "Ükski tudeng pole läbinud kõiki õppeaineid."

### Ülesanne 8.4
Määrake, millised muutujad on vabad ja millised seotud järgmistes valemites:

a) ∀x ∈ D (P(x) → Q(x,y))
b) ∃z ∈ D (R(x,z) ∧ ∀x ∈ D S(x,z))
c) ∀x ∈ D ∃y ∈ D (T(x,y,z) → ∀z ∈ D U(x,y,z))

**Lahendused:**

a) x on seotud (üldisuskvantoriga ∀), y on vaba

b) z on seotud (olemasolukvantori ∃ poolt), x on algul vaba, aga teises osas seotud (üldisuskvantoriga ∀)

c) x on seotud (üldisuskvantoriga ∀), y on seotud (olemasolukvantori ∃ poolt), z on algul vaba, aga teises osas seotud (üldisuskvantoriga ∀)

### Ülesanne 8.5
Tõlgige järgmised predikaatarvutuse valemid tavakeelde:

a) ∀x ∈ D (Õpetaja(x) → ∃y ∈ D (Õpilane(y) ∧ Õpetab(x, y)))
b) ∃x ∈ D (Pood(x) ∧ ∀y ∈ D (Toode(y) → Müüb(x, y)))
c) ∀x ∈ D ∀y ∈ D ((Sõber(x, y) ∧ Sõber(y, z)) → Sõber(x, z))
d) ∃x ∈ D ∀y ∈ D ¬Armastab(y, x)
e) ∀x ∈ D ∃y ∈ D (x ≠ y ∧ ∀z ∈ D ((z ≠ x ∧ z ≠ y) → (Lähemal(x, z, y))))

**Lahendused:**

a) "Iga õpetaja õpetab vähemalt ühte õpilast."

b) "Leidub pood, mis müüb kõiki tooteid."

c) "Kui x on y sõber ja y on z sõber, siis x on z sõber." (NB! z pole kvantoriga seotud, see on vaba muutuja)

d) "Leidub inimene, keda keegi ei armasta."

e) "Igal objektil x on täpselt üks lähedaim naaber y, mis on lähemal kui mistahes teine objekt z."

### Ülesanne 8.6
Otsustage, kas järgmised väited on tõesed või väärad, kui diskursuse universumiks on kõik reaalarvud:

a) ∀x ∈ R ∃y ∈ R (x + y = 0)
b) ∃y ∈ R ∀x ∈ R (x + y = 0)
c) ∀x ∈ R ∀y ∈ R ∃z ∈ R (x < z < y)
d) ∃z ∈ R ∀x ∈ R ∀y ∈ R (x < z < y)
e) ∀x ∈ R ∃y ∈ R (y > x)
f) ∃y ∈ R ∀x ∈ R (y > x)

**Lahendused:**

a) Tõene. Iga reaalarvu x korral leidub selline y = -x, et x + y = 0.

b) Väär. Pole olemas sellist ühte reaalarvut y, et iga reaalarvu x korral kehtiks x + y = 0.

c) Väär. Kui x ≥ y, siis pole võimalik leida z, et x < z < y.

d) Väär. Pole olemas sellist z, et iga x ja y korral kehtiks x < z < y, sest alati saame valida x ≥ y.

e) Tõene. Iga reaalarvu x korral leidub y = x + 1, mis on suurem kui x.

f) Väär. Pole olemas suurimat reaalarvut, mis oleks suurem kõigist teistest.

### Ülesanne 8.7
Eitame järgmisi väiteid:

a) Kõik linnud lendavad.
b) Mõned õpilased on tublid.
c) Kõik arvud on positiivsed.
d) Mõnel inimesel on sinine auto.
e) Ükski kass ei oska ujuda.

**Lahendused:**

a) "Kõik linnud lendavad" formaliseerituna: ∀x ∈ D (Lind(x) → Lendab(x))
   Eitus: ¬(∀x ∈ D (Lind(x) → Lendab(x))) ≡ ∃x ∈ D (Lind(x) ∧ ¬Lendab(x))
   Tõlgendus: "Leidub lind, kes ei lenda."

b) "Mõned õpilased on tublid" formaliseerituna: ∃x ∈ D (Õpilane(x) ∧ Tubli(x))
   Eitus: ¬(∃x ∈ D (Õpilane(x) ∧ Tubli(x))) ≡ ∀x ∈ D (¬Õpilane(x) ∨ ¬Tubli(x)) ≡ ∀x ∈ D (Õpilane(x) → ¬Tubli(x))
   Tõlgendus: "Ükski õpilane ei ole tubli."

c) "Kõik arvud on positiivsed" formaliseerituna: ∀x ∈ D (Arv(x) → Positiivne(x))
   Eitus: ¬(∀x ∈ D (Arv(x) → Positiivne(x))) ≡ ∃x ∈ D (Arv(x) ∧ ¬Positiivne(x))
   Tõlgendus: "Leidub arv, mis ei ole positiivne."

d) "Mõnel inimesel on sinine auto" formaliseerituna: ∃x ∈ D (Inimene(x) ∧ OmabSinistAutot(x))
   Eitus: ¬(∃x ∈ D (Inimene(x) ∧ OmabSinistAutot(x))) ≡ ∀x ∈ D (¬Inimene(x) ∨ ¬OmabSinistAutot(x)) ≡ ∀x ∈ D (Inimene(x) → ¬OmabSinistAutot(x))
   Tõlgendus: "Ühelgi inimesel pole sinist autot."

e) "Ükski kass ei oska ujuda" formaliseerituna: ∀x ∈ D (Kass(x) → ¬OskabUjuda(x))
   Eitus: ¬(∀x ∈ D (Kass(x) → ¬OskabUjuda(x))) ≡ ∃x ∈ D (Kass(x) ∧ ¬¬OskabUjuda(x)) ≡ ∃x ∈ D (Kass(x) ∧ OskabUjuda(x))
   Tõlgendus: "Leidub kass, kes oskab ujuda."

### Ülesanne 8.8
Eitame järgmisi väiteid:

a) Iga inimese kohta leidub raamat, mida ta on lugenud.
b) Leidub film, mida kõik on näinud.
c) Igal täisarvul on algarvuline jagaja.
d) Leidub selline reaalarvude jada, mis läheneb igale reaalarvule.

**Lahendused:**

a) "Iga inimese kohta leidub raamat, mida ta on lugenud" formaliseerituna: ∀x ∈ D (Inimene(x) → ∃y ∈ D (Raamat(y) ∧ OnLugenud(x,y)))
   Eitus: ¬(∀x ∈ D (Inimene(x) → ∃y ∈ D (Raamat(y) ∧ OnLugenud(x,y)))) ≡ ∃x ∈ D (Inimene(x) ∧ ¬(∃y ∈ D (Raamat(y) ∧ OnLugenud(x,y)))) ≡ ∃x ∈ D (Inimene(x) ∧ ∀y ∈ D (¬Raamat(y) ∨ ¬OnLugenud(x,y))) ≡ ∃x ∈ D (Inimene(x) ∧ ∀y ∈ D (Raamat(y) → ¬OnLugenud(x,y)))
   Tõlgendus: "Leidub inimene, kes pole lugenud ühtegi raamatut."

b) "Leidub film, mida kõik on näinud" formaliseerituna: ∃x ∈ D (Film(x) ∧ ∀y ∈ D (Inimene(y) → OnNäinud(y,x)))
   Eitus: ¬(∃x ∈ D (Film(x) ∧ ∀y ∈ D (Inimene(y) → OnNäinud(y,x)))) ≡ ∀x ∈ D (¬Film(x) ∨ ¬(∀y ∈ D (Inimene(y) → OnNäinud(y,x)))) ≡ ∀x ∈ D (¬Film(x) ∨ ∃y ∈ D (Inimene(y) ∧ ¬OnNäinud(y,x))) ≡ ∀x ∈ D (Film(x) → ∃y ∈ D (Inimene(y) ∧ ¬OnNäinud(y,x)))
   Tõlgendus: "Iga filmi kohta leidub inimene, kes pole seda näinud."

c) "Igal täisarvul on algarvuline jagaja" formaliseerituna: ∀x ∈ Z (x ≠ 0 → ∃y ∈ Z (Algarv(y) ∧ Jagab(y,x)))
   Eitus: ¬(∀x ∈ Z (x ≠ 0 → ∃y ∈ Z (Algarv(y) ∧ Jagab(y,x)))) ≡ ∃x ∈ Z (x ≠ 0 ∧ ¬(∃y ∈ Z (Algarv(y) ∧ Jagab(y,x)))) ≡ ∃x ∈ Z (x ≠ 0 ∧ ∀y ∈ Z (¬Algarv(y) ∨ ¬Jagab(y,x))) ≡ ∃x ∈ Z (x ≠ 0 ∧ ∀y ∈ Z (Algarv(y) → ¬Jagab(y,x)))
   Tõlgendus: "Leidub nullist erinev täisarv, millel pole algarvulist jagajat."

d) "Leidub selline reaalarvude jada, mis läheneb igale reaalarvule" formaliseerituna: ∃x ∈ D (Jada(x) ∧ ∀y ∈ R (Läheneb(x,y)))
   Eitus: ¬(∃x ∈ D (Jada(x) ∧ ∀y ∈ R (Läheneb(x,y)))) ≡ ∀x ∈ D (¬Jada(x) ∨ ¬(∀y ∈ R (Läheneb(x,y)))) ≡ ∀x ∈ D (¬Jada(x) ∨ ∃y ∈ R (¬Läheneb(x,y))) ≡ ∀x ∈ D (Jada(x) → ∃y ∈ R (¬Läheneb(x,y)))
   Tõlgendus: "Iga reaalarvude jada korral leidub reaalarv, millele see jada ei lähene."