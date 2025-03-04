# Järeldumine lausearvutuses

## Järeldumise mõiste

Järeldumine on üks olulisemaid loogilisi kontseptsioone, mis moodustab matemaatilise arutluse aluse. Järeldumise mõiste võimaldab meil analüüsida, kas antud eeldustest saab korrektselt tuletada mingit järeldust.

**Definitsioon:** Öeldakse, et valemitest F₁, F₂, ..., Fₙ **järeldub** valem G, kui igal neis valemeis esinevate muutujate väärtustusel, millel F₁, F₂, ..., Fₙ on tõesed, on ka G tõene.

Asjaolu, et valemitest F₁, F₂, ..., Fₙ järeldub valem G, tähistatakse sümboliga:
F₁, F₂, ..., Fₙ ⊨ G

Sümbolit ⊨ loetakse sõnaga "järeldub".

### Järeldumise intuitiivne tähendus

Intuitiivselt tähendab järeldumine seda, et kui võtame kõik eeldused (F₁, F₂, ..., Fₙ) tõestena, siis peab ka järeldus (G) olema tõene. Kui leidub kasvõi üks olukord, kus kõik eeldused on tõesed, aga järeldus on väär, siis järeldumine ei kehti.

**Märkus:** Järeldumist F₁, F₂, ..., Fₙ ⊨ G ei tohi segi ajada implikatsiooniga F₁ ∧ F₂ ∧ ... ∧ Fₙ ⇒ G. Implikatsioon on tehe, mis annab tulemuseks lause, järeldumine aga on väide kahe lause või valemi vahelise suhte kohta.

## Järeldumise kontrollimine

Järeldumise kontrollimiseks on mitu meetodit:

### 1. Tõeväärtustabeli abil

Tõeväärtustabelis valime välja kõik read, kus valemid F₁, F₂, ..., Fₙ on kõik tõesed, ja kontrollime, kas ka valem G on nendes ridades tõene. Kui leidub kasvõi üks rida, kus F₁, F₂, ..., Fₙ on kõik tõesed, aga G on väär, siis järeldumine ei kehti.

**Näide:** Kontrollime, kas valemitest X ∧ Y ja Y ⇒ Z järeldub valem X ⇒ Z.

Koostame tõeväärtustabeli:

| X | Y | Z | X ∧ Y | Y ⇒ Z | X ⇒ Z |
|---|---|---|-------|-------|-------|
| t | t | t | t     | t     | t     |
| t | t | v | t     | v     | v     |
| t | v | t | v     | t     | t     |
| t | v | v | v     | t     | v     |
| v | t | t | v     | t     | t     |
| v | t | v | v     | v     | t     |
| v | v | t | v     | t     | t     |
| v | v | v | v     | t     | t     |

Vaatame ridu, kus X ∧ Y ja Y ⇒ Z on mõlemad tõesed:
- Esimene rida: X = t, Y = t, Z = t, kus ka X ⇒ Z = t
- Ridade 3, 5, 7, 8 puhul X ∧ Y = v, seega neid ei pea arvestama
- Ridade 2 ja 6 puhul Y ⇒ Z = v, seega neid ei pea arvestama
- Rida 4: X = t, Y = v, Z = v, X ∧ Y = v, so seda rida ei pea arvestama

Ainus rida, kus X ∧ Y ja Y ⇒ Z on mõlemad tõesed, on esimene rida, ja selles on ka X ⇒ Z tõene. Seega järeldumine kehtib: X ∧ Y, Y ⇒ Z ⊨ X ⇒ Z.

### 2. Teoreemi abil

Järeldumist saab kontrollida ka ilma täieliku tõeväärtustabelita, kasutades järgmist teoreemi:

**Teoreem:** Valemitest F₁, F₂, ..., Fₙ järeldub valem G parajasti siis, kui valem F₁ ∧ F₂ ∧ ... ∧ Fₙ ⇒ G on samaselt tõene (tautoloogia).

See teoreem võimaldab taandada järeldumise kontrollimise ühe valemi samaselt tõesuse kontrollimisele.

**Näide:** Kontrollime uuesti, kas valemitest X ∧ Y ja Y ⇒ Z järeldub valem X ⇒ Z.

Teoreemi kohaselt peame kontrollima, kas valem (X ∧ Y) ∧ (Y ⇒ Z) ⇒ (X ⇒ Z) on tautoloogia.

Koostame tõeväärtustabeli:

| X | Y | Z | X ∧ Y | Y ⇒ Z | (X ∧ Y) ∧ (Y ⇒ Z) | X ⇒ Z | ((X ∧ Y) ∧ (Y ⇒ Z)) ⇒ (X ⇒ Z) |
|---|---|---|-------|-------|-------------------|-------|--------------------------------|
| t | t | t | t     | t     | t                 | t     | t                              |
| t | t | v | t     | v     | v                 | v     | t                              |
| t | v | t | v     | t     | v                 | t     | t                              |
| t | v | v | v     | t     | v                 | v     | t                              |
| v | t | t | v     | t     | v                 | t     | t                              |
| v | t | v | v     | v     | v                 | t     | t                              |
| v | v | t | v     | t     | v                 | t     | t                              |
| v | v | v | v     | t     | v                 | t     | t                              |

Kuna viimases veerus on kõik väärtused tõesed, on valem (X ∧ Y) ∧ (Y ⇒ Z) ⇒ (X ⇒ Z) tautoloogia, seega kehtib järeldumine X ∧ Y, Y ⇒ Z ⊨ X ⇒ Z.

## Tähtsamad järeldusreeglid

Järgnevad on mõned olulisemad järeldusreeglid, mida kasutatakse sageli loogilistes arutlustes:

### 1. Modus Ponens (jaatav moodus)

Kui teame, et väide A on tõene ja A implikeerib B, siis võime järeldada, et B on tõene.

A, A ⇒ B ⊨ B

**Näide:** Kui on teada, et "Täna sajab vihma" ja "Kui täna sajab vihma, siis tee on märg", siis võime järeldada, et "Tee on märg".

### 2. Modus Tollens (eitav moodus)

Kui teame, et väide B on väär ja A implikeerib B, siis võime järeldada, et A on väär.

¬B, A ⇒ B ⊨ ¬A

**Näide:** Kui on teada, et "Tee ei ole märg" ja "Kui täna sajab vihma, siis tee on märg", siis võime järeldada, et "Täna ei saja vihma".

### 3. Hüpoteetiline süllogism (transitiivsus)

Kui A implikeerib B ja B implikeerib C, siis A implikeerib C.

A ⇒ B, B ⇒ C ⊨ A ⇒ C

**Näide:** Kui on teada, et "Kui täna sajab vihma, siis tee on märg" ja "Kui tee on märg, siis jalutuskäik jääb ära", siis võime järeldada, et "Kui täna sajab vihma, siis jalutuskäik jääb ära".

### 4. Disjunktiivne süllogism

Kui teame, et kas A või B on tõene, ja A on väär, siis B peab olema tõene.

A ∨ B, ¬A ⊨ B

**Näide:** Kui on teada, et "Kas lähme kinno või jääme koju" ja "Me ei lähe kinno", siis võime järeldada, et "Me jääme koju".

### 5. Konjunktsiooni lisamine

Kui A on tõene ja B on tõene, siis A ja B on mõlemad tõesed.

A, B ⊨ A ∧ B

**Näide:** Kui on teada, et "Täna on kolmapäev" ja "Väljas sajab vihma", siis võime järeldada, et "Täna on kolmapäev ja väljas sajab vihma".

### 6. Lihtsustamine

Kui A ja B on mõlemad tõesed, siis A on tõene (ja B on tõene).

A ∧ B ⊨ A
A ∧ B ⊨ B

**Näide:** Kui on teada, et "Täna on kolmapäev ja väljas sajab vihma", siis võime järeldada, et "Täna on kolmapäev".

### 7. Lisamine

Kui A on tõene, siis A või ükskõik milline teine väide B on tõene.

A ⊨ A ∨ B

**Näide:** Kui on teada, et "Täna on kolmapäev", siis võime järeldada, et "Täna on kolmapäev või väljas sajab vihma".

### 8. Dilemma (konstruktiivne dilemma)

Kui teame, et kas A või B on tõene, ja A implikeerib C ning B implikeerib D, siis kas C või D peab olema tõene.

A ∨ B, A ⇒ C, B ⇒ D ⊨ C ∨ D

**Näide:** Kui on teada, et "Kas lähen ülikooli või tööle", "Kui lähen ülikooli, siis saan hariduse" ja "Kui lähen tööle, siis saan raha", siis võime järeldada, et "Kas saan hariduse või saan raha".

## Järeldumisreeglite kasutamine arutluste analüüsimisel

Järeldumisreeglite abil saab kontrollida, kas mingi arutlus on loogiliselt korrektne.

### Näide 1: Arutluse korrektsuse kontrollimine

Analüüsime järgmist arutlust:
1. Kui õpin hästi, siis saan head hinded.
2. Kui saan head hinded, siis mind võetakse ülikooli.
3. Ma ei pääsenud ülikooli.
4. Järelikult ma ei õppinud hästi.

Tähistame:
- P: "Õpin hästi"
- Q: "Saan head hinded"
- R: "Mind võetakse ülikooli"

Antud arutlus väljendub valemitega:
1. P ⇒ Q
2. Q ⇒ R
3. ¬R
4. ¬P (järeldus)

Kontrollime, kas eeldustest 1-3 järeldub väide 4:
P ⇒ Q, Q ⇒ R, ¬R ⊨ ¬P

Lahenduskäik:
1. P ⇒ Q, Q ⇒ R ⊨ P ⇒ R (hüpoteetiline süllogism)
2. P ⇒ R, ¬R ⊨ ¬P (modus tollens)

Seega arutlus on loogiliselt korrektne.

### Näide 2: Vigase arutluse tuvastamine

Analüüsime järgmist arutlust:
1. Kui täna sajab vihma, siis tee on märg.
2. Tee on märg.
3. Järelikult täna sajab vihma.

Tähistame:
- P: "Täna sajab vihma"
- Q: "Tee on märg"

Antud arutlus väljendub valemitega:
1. P ⇒ Q
2. Q
3. P (järeldus)

Kontrollime, kas eeldustest 1-2 järeldub väide 3:
P ⇒ Q, Q ⊨ P

See ei ole korrektne järeldumine. Siin on tegemist levinud loogilise veaga, mida nimetatakse "implikatsiooni tagasisuuna veaks" (fallacy of affirming the consequent).

Tõeväärtustabeli abil näeme, et rida, kus P = v ja Q = t, on vastuväide:

| P | Q | P ⇒ Q | P ⇒ Q ∧ Q | (P ⇒ Q ∧ Q) ⇒ P |
|---|---|-------|-----------|-------------------|
| t | t | t     | t         | t                 |
| t | v | v     | v         | t                 |
| v | t | t     | t         | v                 |
| v | v | t     | v         | t                 |

Kuna (P ⇒ Q ∧ Q) ⇒ P ei ole tautoloogia (kolmandas reas on väär), ei kehti järeldumine P ⇒ Q, Q ⊨ P.

See on loogiline, sest kui tee on märg, võib see olla tingitud ka muudest põhjustest, mitte ainult vihmasajust (näiteks keegi kastis aeda või tänavapesijad tegid oma tööd).

## Järeldumise ja samaväärsuse seos

Järeldumine ja samaväärsus on omavahel tihedalt seotud:

**Teoreem:** Valemid F ja G on samaväärsed parajasti siis, kui valemist F järeldub valem G ja valemist G järeldub valem F.

Teisisõnu: F ≡ G parajasti siis, kui F ⊨ G ja G ⊨ F.

**Näide:** Näitame, et valemid X ⇒ Y ja ¬X ∨ Y on samaväärsed.

1. Kontrollime, kas X ⇒ Y ⊨ ¬X ∨ Y:
   - Koostame tõeväärtustabeli:
   
   | X | Y | X ⇒ Y | ¬X | ¬X ∨ Y |
   |---|---|-------|-----|---------|
   | t | t | t     | v   | t       |
   | t | v | v     | v   | v       |
   | v | t | t     | t   | t       |
   | v | v | t     | t   | t       |
   
   - Kõikidel juhtudel, kus X ⇒ Y on tõene (read 1, 3, 4), on ka ¬X ∨ Y tõene.
   - Seega X ⇒ Y ⊨ ¬X ∨ Y.

2. Kontrollime, kas ¬X ∨ Y ⊨ X ⇒ Y:
   - Sama tõeväärtustabeli põhjal näeme, et kõikidel juhtudel, kus ¬X ∨ Y on tõene (read 1, 3, 4), on ka X ⇒ Y tõene.
   - Seega ¬X ∨ Y ⊨ X ⇒ Y.

Kuna kehtivad mõlemad järeldumised, on valemid X ⇒ Y ja ¬X ∨ Y samaväärsed.

## Järeldumise kasutamine praktilistes olukordades

Järeldumise mõiste on oluline mitte ainult matemaatikas, vaid ka igapäevaelus, kus teeme pidevalt järeldusi olemasoleva info põhjal.

### Näide 1: Õigussüsteemis

Õigussüsteemis on loogiline arutlus kesksel kohal. Näiteks:

1. Kui isik paneb toime kuriteo, siis ta väärib karistust.
2. Kui on tõendeid, et isik pani toime kuriteo, siis isik pani toime kuriteo.
3. Kui ei ole tõendeid, et isik pani toime kuriteo, siis ei saa väita, et isik pani toime kuriteo.
4. Kui ei saa väita, et isik pani toime kuriteo, siis isik ei vääri karistust.

Tähistame:
- K: "Isik pani toime kuriteo"
- T: "On tõendeid, et isik pani toime kuriteo"
- V: "Isik väärib karistust"

Väljendades need lausearvutuse valemitena:
1. K ⇒ V
2. T ⇒ K
3. ¬T ⇒ ¬K (mis on ekvivalentne lausega K ⇒ T)
4. ¬K ⇒ ¬V (mis on ekvivalentne lausega V ⇒ K)

Nüüd võime kontrollida, kas näiteks väitest "Pole tõendeid, et isik pani toime kuriteo" järeldub "Isik ei vääri karistust":
¬T ⊨ ¬V

Lahenduskäik:
1. ¬T ⇒ ¬K (eeldus 3)
2. ¬K ⇒ ¬V (eeldus 4)
3. ¬T ⇒ ¬V (hüpoteetiline süllogism)

Seega ¬T ⊨ ¬V ehk "Kui pole tõendeid, et isik pani toime kuriteo, siis isik ei vääri karistust", mis on kooskõlas süütuse presumptsiooni põhimõttega.

### Näide 2: Programmeerimine

Programmeerimisel on loogiline arutlus samuti väga oluline. Näiteks:

```
if (userHasPermission || userIsAdmin) {
    allowAccess();
} else {
    denyAccess();
}
```

Siin on loogiline arutlus:
1. Kui kasutajal on luba või kasutaja on administraator, siis võimaldame juurdepääsu.
2. Kui kasutajal pole luba ja kasutaja pole administraator, siis keelame juurdepääsu.

Tähistame:
- P: "Kasutajal on luba"
- A: "Kasutaja on administraator"
- J: "Võimaldame juurdepääsu"

Valemite kujul:
1. P ∨ A ⇒ J
2. ¬(P ∨ A) ⇒ ¬J

Samaväärsuste abil saame näidata, et teine valem on samaväärne valemiga ¬P ∧ ¬A ⇒ ¬J, mis omakorda De Morgani seaduse abil on samaväärne valemiga J ⇒ P ∨ A.

Seega kood väljendab kahte loogilist järeldust:
- P ∨ A ⊨ J (Kui kasutajal on luba või ta on administraator, siis tal on juurdepääs)
- J ⊨ P ∨ A (Kui kasutajal on juurdepääs, siis tal on kas luba või ta on administraator)

## Järeldumise kasutamine matemaatilises tõestamises

Matemaatilises tõestamises kasutatakse järeldumisreegleid lausete tõesuse tuletamiseks teiste, juba teada olevate lausete tõesusest.

### Näide: Matemaatiline tõestus

Tõestatav teoreem: "Kui arv on paarisarv, siis tema ruut on paarisarv."

Tähistame:
- P: "Arv n on paarisarv"
- Q: "Arvu n ruut on paarisarv"

Peame tõestama, et P ⊨ Q.

Tõestus:
1. Kui n on paarisarv, siis leidub täisarv k nii, et n = 2k (paarisarvu definitsioon).
2. Arvu n ruut on n² = (2k)² = 4k² = 2(2k²).
3. Kuna 2k² on täisarv, siis n² = 2(2k²) on paarisarv (paarisarvu definitsioon).
4. Seega, kui n on paarisarv, siis n² on paarisarv.

See tõestus kasutab järeldumisreeglite ahelat, et näidata, et eeldusest "n on paarisarv" järeldub "n² on paarisarv".

## Mõned keerulisemad järeldumisreeglid

Lisaks eelnevalt mainitud põhilistele järeldumisreeglitele kasutatakse matemaatilises loogikas ka keerulisemaid reegleid:

### 1. Resolutsioonireegel

Kui kehtivad disjunktsioonid A ∨ B ja ¬A ∨ C, siis järeldub B ∨ C.

A ∨ B, ¬A ∨ C ⊨ B ∨ C

See on üldistus disjunktiivsest süllogismist ja on automaatse teoreemitõestamise olulisim reegel.

**Näide:** Kui on teada, et "Mari on kodus või kontoris" ja "Mari ei ole kodus või ta on arvutiga", siis järeldub, et "Mari on kontoris või ta on arvutiga".

### 2. Ekvivalentsireegel

Kui kehtib ekvivalents A ⇔ B ja lause A on tõene, siis on tõene ka lause B.

A ⇔ B, A ⊨ B

Samuti: A ⇔ B, B ⊨ A

**Näide:** Kui on teada, et "Inimene on täisealine parajasti siis, kui ta on vähemalt 18-aastane" ja "Jüri on täisealine", siis järeldub, et "Jüri on vähemalt 18-aastane".

### 3. Konstruktiivne reductio ad absurdum

Kui eelduse A lisamine olemasolevale eelduste hulgale viib vastuoluni, siis järeldub ¬A.

H, A ⊨ B ∧ ¬B siis H ⊨ ¬A

kus H on mõni eelduste hulk.

**Näide:** Kui eeldusest "Arv x on ratsionaalarv" järeldub vastuolu, siis järeldub, et "Arv x ei ole ratsionaalarv". Seda meetodit kasutatakse tihti irratsionaalarvude olemasolu tõestamisel.

## Järeldumise tähtsus arvutiteaduses

Järeldumine on kesksel kohal paljudes arvutiteaduse valdkondades:

### Automaatne teoreemitõestamine

Automaatne teoreemitõestamine kasutab järeldumisreegleid, et tuletada automaatselt teoreeemide tõestusi. Üks populaarne meetod on resolutsioonil põhinev tõestamine, mis kasutab resolutsioonireeglit.

### Teadmiste esitamise süsteemid ja tehisintellekt

Teadmiste esitamise süsteemides ja tehisintellektis kasutatakse järeldumisreegleid, et tuletada uusi teadmisi olemasolevate teadmiste baasil.

### Verifitseerimine ja valideerimine

Arvutiprogrammide formaalne verifitseerimine kasutab järeldumist, et tõestada programmi korrektsust. Näiteks, kui meil on programmi spetsifikatsioon S ja programmi implementatsioon I, siis tahame näidata, et I ⊨ S.

## Kokkuvõte

Järeldumine on üks matemaatilise loogika põhimõisteid, mis võimaldab meil analüüsida, kas antud eeldustest saab korrektselt tuletada järeldust. Järeldumist tähistatakse sümboliga ⊨ ja seda saab kontrollida tõeväärtustabelite või teoreemide abil.

Olulisemad järeldumisreeglid on:
- Modus ponens (A, A ⇒ B ⊨ B)
- Modus tollens (¬B, A ⇒ B ⊨ ¬A)
- Hüpoteetiline süllogism (A ⇒ B, B ⇒ C ⊨ A ⇒ C)
- Disjunktiivne süllogism (A ∨ B, ¬A ⊨ B)

Järeldumine on kesksel kohal nii igapäevaelus, õigussüsteemis, programmeerimises kui ka matemaatilistes tõestustes. Loogiliselt korrektse arutluse tundmine aitab meil vältida levinud loogilisi vigu ja teha õigeid järeldusi olemasolevast infost.