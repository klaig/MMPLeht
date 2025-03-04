# Lausearvutuse tehted

Lausearvutuses kasutatakse mitmeid loogilisi tehteid, et lihtlausetest moodustada keerulisemaid liitlauseid. Erinevalt tavakeelest on lausearvutuses igal tehtel täpne matemaatiline definitsioon, mis määrab üheselt liitlause tõeväärtuse sõltuvalt komponentlausete tõeväärtustest.

## Loogilised tehted

Lausearvutuse põhitehted on:
1. Eitus (¬)
2. Konjunktsioon (∧)
3. Disjunktsioon (∨)
4. Implikatsioon (⇒)
5. Ekvivalents (⇔)

Vaatame iga tehet põhjalikumalt.

## 1. Eitus (¬)

Eitus on loogiline tehe, mida rakendatakse ühele lausele. Eitus muudab lause tõeväärtuse vastupidiseks: tõene muutub vääraks ja väär muutub tõeseks.

**Definitsioon:** Lause A eituseks nimetatakse lauset ¬A, mis on tõene parajasti siis, kui lause A on väär.

**Tõeväärtustabel:**

| A | ¬A |
|---|-----|
| t | v |
| v | t |

**Keeleline vaste:** "mitte", "ei ole"

**Näited:**
- Kui A = "Täna on kolmapäev", siis ¬A = "Täna ei ole kolmapäev"
- Kui A = "2 + 2 = 4", siis ¬A = "2 + 2 ≠ 4"

**Oluline omadus:** Kahekordne eitus taastab algse lause tõeväärtuse: ¬(¬A) ≡ A

## 2. Konjunktsioon (∧)

Konjunktsioon on loogiline tehe, mis vastab keeleliselt sõnale "ja". Konjunktsioon ühendab kaks lauset ning tulemus on tõene ainult siis, kui mõlemad laused on tõesed.

**Definitsioon:** Lausete A ja B konjunktsioon A ∧ B on tõene parajasti siis, kui mõlemad komponentlaused A ja B on tõesed.

**Tõeväärtustabel:**

| A | B | A ∧ B |
|---|---|-------|
| t | t | t |
| t | v | v |
| v | t | v |
| v | v | v |

**Keeleline vaste:** "ja", "ning", "aga", "kuid"

**Näited:**
- A = "Täna on kolmapäev", B = "Väljas sajab vihma"
- A ∧ B = "Täna on kolmapäev ja väljas sajab vihma"

**Omadused:**
- Konjunktsioon on kommutatiivne: A ∧ B ≡ B ∧ A
- Konjunktsioon on assotsiatiivne: (A ∧ B) ∧ C ≡ A ∧ (B ∧ C)
- Konjunktsioon on idempotentne: A ∧ A ≡ A

## 3. Disjunktsioon (∨)

Disjunktsioon on loogiline tehe, mis vastab keeleliselt sõnale "või" mittevälistavas tähenduses. Disjunktsioon ühendab kaks lauset ning tulemus on tõene, kui vähemalt üks lause on tõene.

**Definitsioon:** Lausete A ja B disjunktsioon A ∨ B on tõene parajasti siis, kui vähemalt üks komponentidest A või B on tõene.

**Tõeväärtustabel:**

| A | B | A ∨ B |
|---|---|-------|
| t | t | t |
| t | v | t |
| v | t | t |
| v | v | v |

**Keeleline vaste:** "või" (mittevälistavas tähenduses, st "kas A või B või mõlemad")

**Näited:**
- A = "Ma õpin matemaatikat", B = "Ma õpin füüsikat"
- A ∨ B = "Ma õpin matemaatikat või ma õpin füüsikat"

**Omadused:**
- Disjunktsioon on kommutatiivne: A ∨ B ≡ B ∨ A
- Disjunktsioon on assotsiatiivne: (A ∨ B) ∨ C ≡ A ∨ (B ∨ C)
- Disjunktsioon on idempotentne: A ∨ A ≡ A

## 4. Implikatsioon (⇒)

Implikatsioon on loogiline tehe, mis väljendab tingimuslikku konstruktsiooni "kui..., siis...". Implikatsioon ühendab kaks lauset, kus esimene lause on eeldus ja teine lause on järeldus.

**Definitsioon:** Lausete A ja B implikatsioon A ⇒ B on tõene parajasti siis, kui A on väär või B on tõene.

**Tõeväärtustabel:**

| A | B | A ⇒ B |
|---|---|-------|
| t | t | t |
| t | v | v |
| v | t | t |
| v | v | t |

Pane tähele, et implikatsioon on väär ainult ühel juhul: kui eeldus (A) on tõene, aga järeldus (B) on väär.

**Keelelised vasted:**
- "Kui A, siis B"
- "A-st järeldub B"
- "A on B piisav tingimus"
- "B on A tarvilik tingimus"

**Näited:**
- A = "Vihm sajab", B = "Tee on märg"
- A ⇒ B = "Kui vihm sajab, siis tee on märg"

Implikatsiooni tõeväärtusi on mõnikord raske intuitiivselt mõista. Eriti segadust tekitavad juhud, kus eeldus on väär (viimased kaks rida tõeväärtustabelis). Neid saab selgitada järgmiselt:

1. Kui eeldus on väär, siis implikatsioon loetakse tõeseks sõltumata järelduse tõeväärtusest. See tähendab, et väärast eeldusest võib "järeldada" mida iganes.

2. Seda saab mõista lubaduse kontekstis: "Kui sajab vihma, siis võtan vihmavarju." Kui vihma ei saja, siis lubaduski ei kehti - pole oluline, kas ma võtan vihmavarju või mitte.

**Implikatsiooni olulised omadused:**
- Implikatsioon EI OLE kommutatiivne: A ⇒ B ≢ B ⇒ A
- Implikatsioon on transitiivne: kui A ⇒ B ja B ⇒ C, siis A ⇒ C

**Implikatsiooni saab avaldada teiste tehete kaudu:**
- A ⇒ B ≡ ¬A ∨ B
- A ⇒ B ≡ ¬(A ∧ ¬B)

### Implikatsiooniga seotud olulised mõisted

Implikatsiooniga A ⇒ B seoses on olulised järgmised mõisted:

#### Pöördlause (Converse)

**Pöördlause** saadakse implikatsiooni eelduse ja järelduse kohad vahetades.

- Kui originaallause on A ⇒ B, siis pöördlause on B ⇒ A.

**Näide:** Kui originaallause on "Kui sajab vihma, siis tee on märg" (Vihm ⇒ MärgTee), siis pöördlause on "Kui tee on märg, siis sajab vihma" (MärgTee ⇒ Vihm).

Pöördlause **ei ole samaväärsne** originaalse implikatsiooniga. Pöördlause võib olla väär, kuigi originaalne implikatsioon on tõene. Näiteks tee võib olla märg ka muudel põhjustel kui vihm (nt tänavapesu).

#### Vastandlause (Inverse)

**Vastandlause** saadakse implikatsiooni eelduse ja järelduse eitamisega.

- Kui originaallause on A ⇒ B, siis vastandlause on ¬A ⇒ ¬B.

**Näide:** Kui originaallause on "Kui sajab vihma, siis tee on märg" (Vihm ⇒ MärgTee), siis vastandlause on "Kui ei saja vihma, siis tee ei ole märg" (¬Vihm ⇒ ¬MärgTee).

Vastandlause **ei ole samaväärsne** originaalse implikatsiooniga.

#### Pöördvastandlause (Contrapositive)

**Pöördvastandlause** saadakse implikatsiooni eelduse ja järelduse eitamisega ning seejärel nende kohtade vahetamisega.

- Kui originaallause on A ⇒ B, siis pöördvastandlause on ¬B ⇒ ¬A.

**Näide:** Kui originaallause on "Kui sajab vihma, siis tee on märg" (Vihm ⇒ MärgTee), siis pöördvastandlause on "Kui tee ei ole märg, siis ei saja vihma" (¬MärgTee ⇒ ¬Vihm).

Pöördvastandlause **on samaväärsne** originaalse implikatsiooniga. See tähendab, et A ⇒ B ≡ ¬B ⇒ ¬A.

#### Seosed implikatsiooniga seotud lausete vahel

Järgmised omadused kehtivad implikatsiooniga seotud lausete vahel:

1. A ⇒ B ≡ ¬B ⇒ ¬A (implikatsioon ja pöördvastandlause on samaväärsed)
2. ¬A ⇒ ¬B ≡ B ⇒ A (vastandlause ja pöördlause on samaväärsed)

Samas ei ole üldjuhul samaväärsed:
- A ⇒ B ≢ B ⇒ A (implikatsioon ja pöördlause)
- A ⇒ B ≢ ¬A ⇒ ¬B (implikatsioon ja vastandlause)

## 5. Ekvivalents (⇔)

Ekvivalents on loogiline tehe, mis tähendab "parajasti siis, kui" või "siis ja ainult siis, kui". Ekvivalents ühendab kaks lauset ja väljendab, et need on sama tõeväärtusega.

**Definitsioon:** Lausete A ja B ekvivalents A ⇔ B on tõene parajasti siis, kui A ja B on mõlemad tõesed või mõlemad väärad.

**Tõeväärtustabel:**

| A | B | A ⇔ B |
|---|---|-------|
| t | t | t |
| t | v | v |
| v | t | v |
| v | v | t |

**Keelelised vasted:**
- "A parajasti siis, kui B"
- "A siis ja ainult siis, kui B"
- "A on samaväärne B-ga"
- "A kui ja ainult kui B"

**Näited:**
- A = "Kolmnurk on võrdkülgne", B = "Kolmnurga kõik küljed on võrdsed"
- A ⇔ B = "Kolmnurk on võrdkülgne parajasti siis, kui kolmnurga kõik küljed on võrdsed"

**Ekvivalentsi olulised omadused:**
- Ekvivalents on kommutatiivne: A ⇔ B ≡ B ⇔ A
- Ekvivalents on assotsiatiivne: (A ⇔ B) ⇔ C ≡ A ⇔ (B ⇔ C)

**Ekvivalentsi saab avaldada teiste tehete kaudu:**
- A ⇔ B ≡ (A ⇒ B) ∧ (B ⇒ A)
- A ⇔ B ≡ (A ∧ B) ∨ (¬A ∧ ¬B)

## Tehete prioriteedid

Kui valemis on mitu tehet ilma sulgudeta, siis on oluline teada, millises järjekorras neid tuleb sooritada. Lausearvutuse tehete prioriteedid aitavad vähendada valemites kasutatavate sulgude arvu.

Tehete prioriteetide järjekord (kõrgemast madalamani):

1. ¬ (eitus)
2. ∧ (konjunktsioon)
3. ∨ (disjunktsioon)
4. ⇒ (implikatsioon)
5. ⇔ (ekvivalents)

See tähendab, et näiteks valemis A ∨ B ∧ C sooritatakse kõigepealt konjunktsioon B ∧ C ja seejärel disjunktsioon A ∨ (B ∧ C).

Kui soovime muuta tehete järjekorda, tuleb kasutada sulge.

## Näited ja ülesanded

### Näide 1: Liitlause tõeväärtuse leidmine

Leida lause "Kui arv on algarvude korrutis, siis ta ei ole algarv, või ta on algarv" tõeväärtus.

**Lahendus:**

Tähistame:
- A: "Arv on algarvude korrutis"
- B: "Arv ei ole algarv"
- C: "Arv on algarv"

Liitlause on kujul: A ⇒ (B ∨ C)

Kuna B ja C on teineteise eitused (B = ¬C), siis B ∨ C = ¬C ∨ C, mis on tautoloogia (alati tõene).

Seega kogu implikatsioon A ⇒ (B ∨ C) on tõene, sest kui implikatsiooni järeldus on tõene, on kogu implikatsioon tõene olenemata eelduse tõeväärtusest.

### Näide 2: Tehete sooritamine

Leida lause ¬(P ∧ Q) ⇒ (¬P ∨ R) tõeväärtus, kui P = t, Q = v, R = v.

**Lahendus:**

1. Asendame muutujad nende tõeväärtustega:
   ¬(t ∧ v) ⇒ (¬t ∨ v)

2. Leiame P ∧ Q tõeväärtuse:
   t ∧ v = v

3. Leiame ¬(P ∧ Q) tõeväärtuse:
   ¬(v) = t

4. Leiame ¬P tõeväärtuse:
   ¬t = v

5. Leiame ¬P ∨ R tõeväärtuse:
   v ∨ v = v

6. Leiame kogu implikatsiooni tõeväärtuse:
   t ⇒ v = v

Seega antud väärtustuse korral on lause tõeväärtus väär (v).

### Näide 3: Implikatsiooni ja ekvivalentsi erinevus

Vaatleme lauseid:
- A ⇒ B: "Kui arv on paarisarv, siis ta jagub 2-ga"
- A ⇔ B: "Arv on paarisarv parajasti siis, kui ta jagub 2-ga"

**Selgitus:**

Mõlemad laused on antud juhul tõesed, kuna paarisarvu definitsioon ongi "arv, mis jagub 2-ga". Kuid üldiselt on implikatsioon ja ekvivalents erinevad:

1. Implikatsioon A ⇒ B tähendab, et kui A on tõene, siis B on ka tõene, kuid B võib olla tõene ka siis, kui A on väär.

2. Ekvivalents A ⇔ B tähendab, et A ja B on alati sama tõeväärtusega - kas mõlemad tõesed või mõlemad väärad.

Näiteks väide "Kui arv jagub 4-ga, siis ta on paarisarv" on implikatsioon, mis on tõene, kuid vastav ekvivalents "Arv jagub 4-ga parajasti siis, kui ta on paarisarv" on väär, sest on olemas paarisarve (nt 2, 6, 10), mis ei jagu 4-ga.
