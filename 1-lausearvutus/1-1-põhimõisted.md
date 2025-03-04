# Lausearvutuse põhimõisted

## Mis on lausearvutuse lause?

Lausearvutuse lause on väide, millel on kindel tõeväärtus - see on kas **tõene (t)** või **väär (v)**. Lausearvutuse lauseks sobib igasugune väide, mille puhul saame rääkida selle vastavusest või mittevastavusest tegelikkusele.

**Definitsioon**: Matemaatilises loogikas nimetatakse lauseks ainult niisugust väljendit (väidet, kõnekeele lauset), mille korral saab rääkida selle sisu vastavusest või mittevastavusest tegelikkusele.

Kui lause sisu vastab tegelikkusele, siis nimetatakse seda lauset **tõeseks**. Kui lause sisu ei vasta tegelikkusele, siis nimetatakse seda lauset **vääraks**.

### Näited lausetest:

Tõesed laused:
- "Tallinn on Eesti pealinn."
- "Arv 7 on algarv."
- "2 + 2 = 4"

Väärad laused:
- "Tartu on Eesti pealinn."
- "Arv 4 on algarv."
- "2 + 2 = 5"

### Mis EI OLE lausearvutuse laused:

- "Kas sul läheb hästi?" (küsilause)
- "Palun anna mulle raamat." (käsklause)
- "Kui ilus päev!" (hüüdlause)
- "x > 5" (muutujat sisaldav avaldis - tõeväärtus sõltub x väärtusest)
- "Ma valetan praegu." (paradoksaalne lause)

## Loogika alustala: põhimõisted

### Algmõiste

**Definitsioon:** Algmõiste on loogilise süsteemi fundamentaalne mõiste, mida võetakse kasutusele ilma formaalse definitsioonita, kuna see on intuitiivselt arusaadav ja toimib keerulisemate mõistete alustalana. Algmõisteid ei saa defineerida sama süsteemi lihtsamate terminite abil.

**Näide:** Geomeetrias on "punkt" ja "sirge" algmõisted. Mõistame intuitiivselt, mida need tähendavad, kuid neid ei saa defineerida lihtsamate geomeetriliste terminite abil.

**Praktiline rakendus:** Informaatikas on "bitt" (0 või 1) sageli algmõiste, millele tuginedes ehitatakse keerulisemad andmestruktuurid.

### Aksioom

**Definitsioon:** Aksioom on väide, mida võetakse tõesena ilma tõestuseta, toimides lähtepunktina teiste väidete (teoreemide) tuletamisel loogilise arutluse kaudu. Aksioomid moodustavad loogilise või matemaatilise süsteemi vundamendi.

**Näide:** Lausearvutuses on välistatud kolmanda seadus (A ∨ ¬A) aksioom, mis väidab, et väide on kas tõene või selle eitus on tõene - kolmandat võimalust pole.

**Visuaalne esitus:**

```
Loogilise süsteemi struktuur
┌────────────────────────────────┐
│                                │
│  ┌─────────┐    ┌─────────┐    │
│  │Aksioomid│    │ Alg-    │    │
│  │         │    │ mõisted │    │
│  └─────────┘    └─────────┘    │
│         │            │         │
│         v            v         │
│     ┌───────────────────┐      │
│     │  Definitsioonid   │      │
│     └───────────────────┘      │
│              │                 │
│              v                 │
│     ┌───────────────────┐      │
│     │     Teoreemid     │      │
│     └───────────────────┘      │
│                                │
└────────────────────────────────┘
```

### Defineerimine ja definitsioon

**Defineerimine:** Defineerimine on protsess, mille käigus tutvustatakse uut mõistet või terminit, selgitades seda juba mõistetud kontseptsioonide abil.

**Definitsioon:** Definitsioon on väide, mis määratleb täpselt mingi mõiste tähenduse.

**Hea definitsiooni struktuur:**
1. Defineeritav termin
2. Laiem kategooria, kuhu see kuulub
3. Eripärad, mis eristavad seda teistest sama kategooria liikmetest

**Näide:** 
- "Ruut on ristkülik (laiem kategooria), mille kõik küljed on võrdse pikkusega (eristav omadus)."
- "Disjunktsioon on loogiline tehe (laiem kategooria), mis annab tõese tulemuse, kui vähemalt üks operandidest on tõene (eristav omadus)."

**Praktiline rakendus:** Programmeerimisel järgivad funktsioonide ja andmestruktuuride defineerimine sama mustrit - nimetame üksuse, määrame selle tüübi ja kirjeldame selle konkreetset käitumist või omadusi.

## Tõeväärtus

Lausearvutuses tähistame tõest lauset tähega **t** (või numbriga 1) ja väära lauset tähega **v** (või numbriga 0).

Lausearvutuses teeme kaks olulist eeldust:
1. **Kahevalentsuse printsiip**: Iga lause on kas tõene või väär (välistatud kolmanda seadus)
2. **Mittevasturääkivuse printsiip**: Ükski lause pole korraga tõene ja väär

## Lausemuutujad ja liitlaused

Lausearvutuses tähistame lauseid tavaliselt suurte tähtedega (X, Y, Z jne). Neid nimetatakse **lausemuutujateks** või **lihtlauseteks**.

**Liitlause** on lause, mis on moodustatud lihtlausetest, kasutades loogilisi tehteid nagu "ja", "või", "kui..., siis..." jne.

Pane tähele, et lausearvutuses lepitakse kokku:
1. Liitlauseid võib moodustada suvalistest komponentidest, eeldamata nendevahelist sisulist seost
2. Liitlause tõeväärtus sõltub ainult komponentlausete tõeväärtustest, mitte nende sisust

### Näide:

Olgu laused:
- X: "Täna on teisipäev"
- Y: "Väljas sajab vihma"

Neist saame moodustada liitlause:
- "Täna on teisipäev ja väljas sajab vihma" (X ∧ Y)

## Mõtlemisseadused ja lausearvutuse alused

Loogika põhineb mitmel fundamentaalsel mõtlemisseadusel:

1. **Samasuse seadus** - iga mõiste või väide peab ühe arutluse kestel jääma samaks. Näiteks kui räägime kolmnurgast, siis kogu arutluse vältel peab "kolmnurk" tähendama sama asja.

2. **Vasturääkivuse lubamatuse seadus** - kaks teineteist eitavat lauset ei saa olla tõesed üheaegselt. Näiteks ei saa naturaalarv olla üheaegselt algarv ja kordarv.

3. **Välistatud kolmanda seadus** - kahest teineteisele vastukäivast väitest peab üks olema tõene ja teine väär; kolmandat võimalust ei ole (ladina keeles: "tertium non datur"). Näiteks arv on kas paarisarv või paaritu arv, mõlemad korraga ei saa ta olla, aga ta peab olema üks neist.

4. **Küllaldase aluse seadus** - igal väitel peab olema kindel alus või põhjendus.

## Tautoloogia ja kontradiktsioon

**Tautoloogia** on lause, mis on tõene kõigi võimalike komponentlausete tõeväärtuste korral. Tautoloogiat nimetatakse ka **samaselt tõeseks lauseks**.

Näide tautoloogiast: "Täna on teisipäev või täna ei ole teisipäev" (X ∨ ¬X)

**Kontradiktsioon** on lause, mis on väär kõigi võimalike komponentlausete tõeväärtuste korral. Kontradiktsiooni nimetatakse ka **samaselt vääraks lauseks**.

Näide kontradiktsioonist: "Täna on teisipäev ja täna ei ole teisipäev" (X ∧ ¬X)

## Teoreem

**Definitsioon:** Teoreem on väide, mille tõesus on tõestatud, tuginedes aksioomidele, definitsioonidele ja varem tõestatud teoreemidele loogilise deduktiivse protsessi kaudu. Erinevalt aksioomidest vajavad teoreemid tõestust.

**Näide:** Väide "Kui A-st järeldub B ja B-st järeldub C, siis A-st järeldub C" on lausearvutuse teoreem (süllogismi seadus), mida saab tõestada implikatsiooni põhiaksioomide ja definitsioonide abil.

**Aksioomide, definitsioonide ja teoreemide vahelised seosed:**

1. **Aksioomid** on lähtepunktid, mis võetakse vastu ilma tõestuseta
2. **Definitsioonid** määratlevad uusi termineid, tuginedes algmõistetele või varem defineeritud terminitele
3. **Teoreemid** on tõestatud tõed, mis on tuletatud aksioomidest ja definitsioonidest loogilise deduktsiooni abil

**Praktiline näide:** 
- **Aksioom:** Arvutisüsteemis on bitt kas 0 või 1 (välistatud kolmanda seadus bittidele rakendatuna)
- **Definitsioon:** Bait on defineeritud kui 8 biti jada
- **Teoreem:** Baidil on täpselt 256 (2^8) erinevat võimalikku väärtust (seda saab tõestada, kasutades aksioomi ja definitsiooni)

**Teoreemi struktuuri visuaalne esitus:**

```
Teoreemi struktuur
┌────────────────────────────────┐
│           Teoreem              │
├────────────────────────────────┤
│                                │
│  ┌──────────┐                  │
│  │  Väide   │ → Loogiline väide│
│  └──────────┘                  │
│                                │
│  ┌──────────┐                  │
│  │ Tõestus  │ → Loogiline      │
│  │          │   tuletamine     │
│  └──────────┘                  │
│     Kasutab:                   │
│     • Aksioome                 │
│     • Definitsioone            │
│     • Varasemaid teoreeme      │
│     • Järeldusreegleid         │
│                                │
└────────────────────────────────┘
```

## Eeldus

**Definitsioon:** Eeldus on väide, mida eeldatakse olevat tõene ja mis toimib alusena järelduse tegemiseks loogilises arutluses.

**Näide:** Arutluses "Kõik arvutid kasutavad elektrit; minu kalkulaator on arvuti; järelikult kasutab minu kalkulaator elektrit" on kaks esimest väidet eeldused.

**Praktiline rakendus:** Programmikoodi silumisel alustavad programmeerijad sageli eeldustest süsteemi eri osade eeldatava käitumise kohta, et leida vigade asukohti.

## Kehtestatavus ja kummutatavus

**Kehtestatav lause** on lause, mis on tõene vähemalt ühe lausemuutujate väärtustuse korral.

Näide kehtestatavast lausest, mis pole tautoloogia: "Täna on teisipäev ja väljas sajab vihma" (X ∧ Y) - see lause on tõene, kui mõlemad komponendid on tõesed.

**Kummutatav lause** on lause, mis on väär vähemalt ühe lausemuutujate väärtustuse korral.

Näide kummutatavast lausest, mis pole kontradiktsioon: "Täna on teisipäev või väljas sajab vihma" (X ∨ Y) - see lause on väär, kui mõlemad komponendid on väärad.

## Lausete vormistamine matemaatilises tekstis

Matemaatilise teksti kirjutamisel tuleks järgida mõningaid olulisi soovitusi:

1. **Ära alusta sümboli, valemi või avaldisega.** Matemaatiline tekst järgib samu reegleid kui tavaline tekst. Näiteks peab lause alati algama suure tähega. Parem on kirjutada "Võrrandil x² - 6x + 8 = 0 on kaks erinevat reaalarvulist lahendit" kui "x² - 6x + 8 = 0 on kaks erinevat reaalarvulist lahendit."

2. **Eralda samasse loetelusse mittekuuluvad sümbolid sõnadega.** Selgemini mõistetav on "Lisaks arvule a on arv b samuti võrrandi (x − a)(x − b) = 0 lahendiks" kui "Lisaks arvule a, b on samuti võrrandi (x − a)(x − b) = 0 lahendiks."

3. **Ära ühenda omavahel sõnu ja sümboleid.** Õige on kirjutada "Iga arvust kaks suurem või võrdne täisarv on kas algarv või kordarv" mitte "Iga täisarv ≥ 2 on kas algarv või kordarv."

4. **Matemaatilistele sümbolitele ei lisata käändelõppe.** Õige on kirjutada "pideva funktsiooniga f", mitte "pideva f-ga".

## Näited ja ülesanded

### Näide 1: Lausete tõeväärtuste määramine

Määra järgmiste lausete tõeväärtused (tõene või väär):

1. "Arv 9 on algarv."
2. "Maa on Päikesesüsteemi kolmas planeet."
3. "Kui 3 > 2, siis 5 < 4."
4. "3 > 2 või 5 < 4."
5. "3 > 2 ja 5 < 4."

**Lahendus:**

1. Väär (v), sest 9 = 3 × 3, seega 9 ei ole algarv.
2. Tõene (t), sest Maa on tõepoolest Päikesesüsteemi kolmas planeet.
3. Väär (v), sest kui eeldus "3 > 2" on tõene, aga järeldus "5 < 4" on väär, siis kogu implikatsioon on väär.
4. Tõene (t), sest vähemalt üks osa, "3 > 2", on tõene, seega kogu disjunktsioon on tõene.
5. Väär (v), sest üks osa, "5 < 4", on väär, seega kogu konjunktsioon on väär.

### Näide 2: Lausearvutuse lause vs mitte-lause

Otsusta, millised järgnevatest on lausearvutuse laused:

1. "Palun aita mind ülesannete lahendamisel."
2. "Pariis on Prantsusmaa pealinn."
3. "Igal naturaalarvul n > 1 on algtegur."
4. "Kas sul on täna aega?"
5. "x² - 4 = 0"

**Lahendus:**

1. Ei ole lausearvutuse lause, sest tegemist on palvega (käsklausega), millel pole tõeväärtust.
2. On lausearvutuse lause, sest sel on kindel tõeväärtus (tõene).
3. On lausearvutuse lause, sest sel on kindel tõeväärtus (tõene).
4. Ei ole lausearvutuse lause, sest tegemist on küsilausega, millel pole tõeväärtust.
5. Ei ole lausearvutuse lause, sest tõeväärtus sõltub muutuja x väärtusest.

### Näide 3: Tautoloogia ja kontradiktsiooni eristamine

Otsusta, kas järgmised laused on tautoloogiad, kontradiktsioonid või ei kumbki:

1. "Kui täna sajab, siis täna sajab."
2. "Täna sajab ja täna ei saja."
3. "Täna sajab või homme paistab päike."

**Lahendus:**

1. See on tautoloogia, sest vorm "kui A, siis A" on alati tõene olenemata A tõeväärtusest.
2. See on kontradiktsioon, sest vorm "A ja ¬A" on alati väär olenemata A tõeväärtusest.
3. See ei ole ei tautoloogia ega kontradiktsioon, sest lause võib olla nii tõene kui ka väär sõltuvalt lausete "Täna sajab" ja "Homme paistab päike" tõeväärtustest.

### Ülesanded

1. Määra, millised järgmistest on lausearvutuse laused. Põhjenda oma vastust.
   a. "Arv π on irratsionaalne."
   b. "Osta mulle piimaa."
   c. "Kui arv on paarisarv, siis ta jagub 2-ga."
   d. "Mis on sinu nimi?"
   e. "f(x) = x² + 2x - 3"

2. Otsusta, millised järgmistest lausetest on tõesed ja millised väärad:
   a. "Arv 17 on paarisarv."
   b. "Kui 2 + 2 = 5, siis Tallinn on Eesti pealinn."
   c. "2 + 2 = 4 või Tallinn on Läti pealinn."
   d. "2 + 2 = 4 ja Tallinn on Läti pealinn."

3. Määra, millised järgmistest lausetest on tautoloogiad, millised kontradiktsioonid ja millised ei kumbki:
   a. "Maa on ümmargune või Maa ei ole ümmargune."
   b. "Kui täna sajab, siis täna sajab või paistab päike."
   c. "Täna sajab ja täna paistab päike ja täna ei saja."
   d. "Kui arv on algarv, siis ta ei jagu ühegi endast väiksema naturaalarvuga peale 1."

**Vastused:**

1. a. On lause (tõene)
   b. Ei ole lause (käsklus)
   c. On lause (tõene)
   d. Ei ole lause (küsimus)
   e. Ei ole lause (avaldis muutujaga)

2. a. Väär (v), sest 17 on paaritu arv
   b. Tõene (t), sest väär eeldus teeb implikatsiooni tõeseks
   c. Tõene (t), sest vähemalt üks osa on tõene
   d. Väär (v), sest üks osa on väär

3. a. Tautoloogia (vorm A ∨ ¬A)
   b. Tautoloogia (vorm A ⇒ (A ∨ B))
   c. Kontradiktsioon (sest sisaldab A ∧ ¬A)
   d. Tautoloogia (algarvu definitsioon)