# Tõeväärtustabelid

Tõeväärtustabel on oluline vahend lausearvutuses, mis võimaldab süstemaatiliselt analüüsida valemite tõeväärtusi erinevate komponentlausete väärtustuste korral. Tõeväärtustabel annab täieliku ülevaate sellest, kuidas valemi tõeväärtus sõltub tema komponentide tõeväärtustest.

## Tõeväärtustabeli olemus

Tõeväärtustabel on tabel, mis näitab lause või valemi tõeväärtust kõikide võimalike komponentlausete tõeväärtuste kombinatsioonide korral. Kui lausearvutuse valemis on n erinevat lausemuutujat, siis tõeväärtustabelis on 2^n rida, mis vastavad kõigile võimalikele lausemuutujate väärtustuste kombinatsioonidele.

### Tõeväärtustabeli eesmärgid:

1. **Valemi tõeväärtuse määramine** - leiame valemi tõeväärtuse iga komponentlausete väärtustuse korral
2. **Tautoloogia ja kontradiktsiooni kontroll** - kui valemi veerus on ainult t-d, on tegemist tautoloogiaga, kui ainult v-d, siis kontradiktsiooniga
3. **Valemite samaväärsuse kontrollimine** - kui kahel valemil on identsed tõeväärtustabelid, siis need valemid on samaväärsed
4. **Järeldumise kontrollimine** - selgitame, kas ühest valemist järeldub teine valem

## Tõeväärtustabeli koostamine

Tõeväärtustabeli koostamisel järgime alljärgnevaid samme:

1. **Identifitseeri kõik erinevad lausemuutujad** valemis (nt X, Y, Z)
2. **Loo tabelisse veerud kõigi lausemuutujate jaoks** ja täida need kõikide võimalike tõeväärtuste kombinatsioonidega
3. **Lisa veerud iga alamavaldise jaoks**, mis esineb valemis, alustades lihtsamatest ja liikudes keerulisemate poole
4. **Lõpuks määra kogu valemi tõeväärtus** iga rea jaoks, kasutades eelnevalt arvutatud alamavaldiste tõeväärtusi

## Näide 1: Lihtsa tõeväärtustabeli koostamine

Koostame tõeväärtustabeli valemile X ∧ (Y ∨ ¬X).

**Samm 1:** Lausemuutujad on X ja Y.

**Samm 2:** Kuna meil on 2 muutujat, on tabelis 2^2 = 4 rida:

| X | Y |
|---|---|
| t | t |
| t | v |
| v | t |
| v | v |

**Samm 3 ja 4:** Arvutame järk-järgult alamavaldiste tõeväärtused:

| X | Y | ¬X | Y ∨ ¬X | X ∧ (Y ∨ ¬X) |
|---|---|-----|---------|--------------|
| t | t | v   | t       | t            |
| t | v | v   | v       | v            |
| v | t | t   | t       | v            |
| v | v | t   | t       | v            |

Arvutuskäik esimese rea jaoks:
1. ¬X = ¬t = v
2. Y ∨ ¬X = t ∨ v = t
3. X ∧ (Y ∨ ¬X) = t ∧ t = t

## Näide 2: Keerukama valemi tõeväärtustabel

Koostame tõeväärtustabeli valemile (X ⇒ Y) ⇔ (¬X ∨ Y).

**Samm 1:** Lausemuutujad on X ja Y.

**Samm 2:** Tabel 4 reaga:

| X | Y |
|---|---|
| t | t |
| t | v |
| v | t |
| v | v |

**Samm 3 ja 4:** Arvutame järk-järgult:

| X | Y | X ⇒ Y | ¬X | ¬X ∨ Y | (X ⇒ Y) ⇔ (¬X ∨ Y) |
|---|---|-------|-----|---------|---------------------|
| t | t | t     | v   | t       | t                   |
| t | v | v     | v   | v       | t                   |
| v | t | t     | t   | t       | t                   |
| v | v | t     | t   | t       | t                   |

Näeme, et valemi veerus on ainult tõesed väärtused, mis tähendab, et valem on tautoloogia. Samuti näitab see, et implikatsiooni X ⇒ Y saab alati avaldada kui ¬X ∨ Y, need on samaväärsed.

## Tõeväärtustabelite rakendused

### 1. Tautoloogia ja kontradiktsiooni tuvastamine

**Tautoloogia** on lause, mis on tõene kõigi väärtustuste korral. Tõeväärtustabelis on sel juhul valemi veerus ainult tõesed väärtused.

**Näide:** X ∨ ¬X on tautoloogia.

| X | ¬X | X ∨ ¬X |
|---|-----|-------|
| t | v   | t     |
| v | t   | t     |

**Kontradiktsioon** on lause, mis on väär kõigi väärtustuste korral. Tõeväärtustabelis on sel juhul valemi veerus ainult väärad väärtused.

**Näide:** X ∧ ¬X on kontradiktsioon.

| X | ¬X | X ∧ ¬X |
|---|-----|-------|
| t | v   | v     |
| v | t   | v     |

### 2. Valemite samaväärsuse kontrollimine

Kaks valemit on samaväärsed, kui neil on identsed tõeväärtustabelid.

**Näide:** Kontrollime, kas De Morgani seadus ¬(X ∧ Y) ≡ ¬X ∨ ¬Y kehtib.

| X | Y | X ∧ Y | ¬(X ∧ Y) | ¬X | ¬Y | ¬X ∨ ¬Y |
|---|---|-------|----------|-----|-----|---------|
| t | t | t     | v        | v   | v   | v       |
| t | v | v     | t        | v   | t   | t       |
| v | t | v     | t        | t   | v   | t       |
| v | v | v     | t        | t   | t   | t       |

Kuna ¬(X ∧ Y) ja ¬X ∨ ¬Y veerud on identsed, on valemid samaväärsed.

### 3. Järeldumise kontrollimine

Valemist A järeldub valem B (A ⊨ B), kui igal real, kus A on tõene, on ka B tõene.

**Näide:** Kontrollime, kas valemist X ∧ Y järeldub valem X.

| X | Y | X ∧ Y | X |
|---|---|-------|---|
| t | t | t     | t |
| t | v | v     | t |
| v | t | v     | v |
| v | v | v     | v |

Valemil X ∧ Y on vaid üks tõene väärtustus (esimene rida). Sellel real on ka X tõene, seega X ∧ Y ⊨ X.

## Tõeväärtustabelite kasutamine probleemide lahendamisel

### Näide 1: Valemite teisendamine

Osutage tõeväärtustabelit kasutades, et valemid ¬(X ⇒ Y) ja X ∧ ¬Y on samaväärsed.

**Lahendus:**

Koostame tõeväärtustabeli:

| X | Y | X ⇒ Y | ¬(X ⇒ Y) | ¬Y | X ∧ ¬Y |
|---|---|-------|----------|-----|---------|
| t | t | t     | v        | v   | v       |
| t | v | v     | t        | t   | t       |
| v | t | t     | v        | v   | v       |
| v | v | t     | v        | t   | v       |

Näeme, et veerud ¬(X ⇒ Y) ja X ∧ ¬Y on identsed, seega valemid on samaväärsed.

### Näide 2: Loogiliste tingimuste analüüs

Programmeerijal on vaja kirjutada tingimus, mis kontrollib, kas kasutaja saab juurdepääsu süsteemile. Juurdepääsu tingimused on järgmised:
- A: Kasutajal on pääsu tase 2 või kõrgem
- B: Kasutaja on administraator
- C: On tööaeg (9:00-17:00)

Juurdepääs antakse, kui:
- Kasutaja on administraator, või
- Kasutajal on tase 2 või kõrgem ja on tööaeg

Koodis võiks see tingimus olla: (B ∨ (A ∧ C))

Kontrollige tõeväärtustabeliga, kas see tingimus on samaväärne tingimusega: ((A ∧ C) ∨ B)

**Lahendus:**

| A | B | C | A ∧ C | B ∨ (A ∧ C) | (A ∧ C) ∨ B |
|---|---|---|-------|-------------|-------------|
| t | t | t | t     | t           | t           |
| t | t | v | v     | t           | t           |
| t | v | t | t     | t           | t           |
| t | v | v | v     | v           | v           |
| v | t | t | v     | t           | t           |
| v | t | v | v     | t           | t           |
| v | v | t | v     | v           | v           |
| v | v | v | v     | v           | v           |

Mõlema valemi tõeväärtused on identsed, seega need on samaväärsed ja programmeerija võib kasutada ükskõik millist neist.

## Tõeväärtustabelite piirangud ja praktilised kaalutlused

Tõeväärtustabelite peamine piirang on see, et valemite puhul, mis sisaldavad palju erinevaid lausemuutujaid, muutub tabel väga suureks. Näiteks 10 muutujaga valemi analüüsimiseks oleks vaja 2^10 = 1024 rida.

Samuti tuleb meeles pidada, et tõeväärtustabelid ei ole ainus viis valemite analüüsimiseks. Paljudel juhtudel on efektiivsem kasutada teisi meetodeid, näiteks algebralist lähenemist põhisamaväärsuste abil.

## Tõeväärtustabelite kasutamine igapäevaelus

Tõeväärtustabeleid saab kasutada igapäevaelu otsustusprotsesside analüüsimiseks.

### Näide: Reisiotsus

Oletame, et pead otsustama, kas minna reisile või mitte, ning sul on järgmised tingimused:
- A: "Piletid on soodsad"
- B: "Ilm on hea"
- C: "Mul on piisavalt vaba aega"

Ütleme, et su otsustusreegel on: "Ma lähen reisile, kui piletid on soodsad JA (ilm on hea VÕI mul on piisavalt vaba aega)".

See avaldub valemina: A ∧ (B ∨ C)

Analüüsime seda tõeväärtustabeliga:

| A | B | C | B ∨ C | A ∧ (B ∨ C) | Kas lähen reisile? |
|---|---|---|-------|-------------|-------------------|
| t | t | t | t     | t           | Jah               |
| t | t | v | t     | t           | Jah               |
| t | v | t | t     | t           | Jah               |
| t | v | v | v     | v           | Ei                |
| v | t | t | t     | v           | Ei                |
| v | t | v | t     | v           | Ei                |
| v | v | t | t     | v           | Ei                |
| v | v | v | v     | v           | Ei                |

Tabelist näeme, et lähed reisile ainult siis, kui piletid on soodsad JA (ilm on hea VÕI sul on piisavalt vaba aega).

## Kokkuvõte

Tõeväärtustabelid on võimas tööriist lausearvutuse valemite analüüsimiseks. Nendega saab:
- Määrata valemi tõeväärtuse kõigi võimalike muutujate väärtuste kombinatsioonide korral
- Tuvastada tautoloogiaid ja kontradiktsioone
- Kontrollida valemite samaväärsust
- Analüüsida järeldumist
- Lahendada praktilisi probleeme

Kuigi suurte valemite puhul võib tõeväärtustabeli koostamine olla töömahukas, on see siiski üks kõige otsesemaid ja kindlamaid meetodeid lausearvutuse ülesannete lahendamiseks.