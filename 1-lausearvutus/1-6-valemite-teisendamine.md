# Valemite teisendamine

## Sissejuhatus

Valemite teisendamine on oluline oskus lausearvutuses, mis võimaldab meil muuta valemite kuju, säilitades nende tõeväärtuse kõigi muutujate väärtuste korral. Teisendamine on kasulik mitmel eesmärgil: valemite lihtsustamiseks, teatud tehete eemaldamiseks või valemite viimiseks standardkujule.

Valemite teisendamine põhineb samaväärsusseostel – kui teame, et valemid F ja G on samaväärsed (F ≡ G), võime ühe asendada teisega, ilma et valemi üldine tõeväärtus muutuks.

## Valemite teisendamise põhimõtted

### Substitutsiooni printsiip

Valemite teisendamise aluseks on **substitutsiooni printsiip**:

**Printsiip:** Kui valemis F asendada osavalem G temaga samaväärse valemiga H, siis saadud valem F' on samaväärne valemiga F.

See printsiip võimaldab meil kasutada teadaolevaid samaväärsusi, et muuta valemi osi samm-sammult.

### Teisendamise etapid

Tavaliselt hõlmab valemite teisendamine järgmisi etappe:

1. **Valemi analüüs** – valemi struktuuri ja komponentide tuvastamine.
2. **Teisendussammude määramine** – sobivate samaväärsuste valimine, mida rakendada.
3. **Samm-sammuline teisendamine** – valitud samaväärsuste järjestikune rakendamine.
4. **Lõpptulemuse kontrollimine** – veendumine, et teisendatud valem on samaväärne algsega.

## Tehete eemaldamine valemist

Üks tavalisemaid teisendamise eesmärke on eemaldada valemist teatud tehted, jättes alles ainult põhitehted (tavaliselt eitus, konjunktsioon ja disjunktsioon).

### Implikatsiooni eemaldamine

Implikatsiooni saab eemaldada, kasutades samaväärsust:

F ⇒ G ≡ ¬F ∨ G

**Näide:**
Eemaldame implikatsiooni valemist P ⇒ (Q ∨ R).

1. P ⇒ (Q ∨ R)
2. ¬P ∨ (Q ∨ R) (implikatsiooni eemaldamine)
3. ¬P ∨ Q ∨ R (disjunktsiooni assotsiatiivsus)

### Ekvivalentsi eemaldamine

Ekvivalentsi saab eemaldada, kasutades samaväärsust:

F ⇔ G ≡ (F ⇒ G) ∧ (G ⇒ F) ≡ (¬F ∨ G) ∧ (¬G ∨ F) ≡ (F ∧ G) ∨ (¬F ∧ ¬G)

**Näide:**
Eemaldame ekvivalentsi valemist P ⇔ Q.

1. P ⇔ Q
2. (P ⇒ Q) ∧ (Q ⇒ P) (ekvivalentsi avaldumine)
3. (¬P ∨ Q) ∧ (¬Q ∨ P) (implikatsiooni eemaldamine)

või alternatiivne tee:

1. P ⇔ Q
2. (P ∧ Q) ∨ (¬P ∧ ¬Q) (ekvivalentsi teine avaldusvorm)

## Eituse sissetoomimine

Teine oluline teisendamise eesmärk on viia eitused vahetult muutujate ette.

### De Morgani seaduste kasutamine

De Morgani seadused on olulised eituse sissetoomisel:

¬(F ∧ G) ≡ ¬F ∨ ¬G
¬(F ∨ G) ≡ ¬F ∧ ¬G

**Näide:**
Teisendame valemi ¬(P ∧ (Q ∨ R)) nii, et eitused oleksid vahetult muutujate ees.

1. ¬(P ∧ (Q ∨ R))
2. ¬P ∨ ¬(Q ∨ R) (De Morgani seadus konjunktsioonile)
3. ¬P ∨ (¬Q ∧ ¬R) (De Morgani seadus disjunktsioonile)

### Kahekordse eituse eemaldamine

Kahekordset eitust saab eemaldada, kasutades samaväärsust:

¬¬F ≡ F

**Näide:**
Teisendame valemi ¬(P ⇒ ¬Q).

1. ¬(P ⇒ ¬Q)
2. ¬(¬P ∨ ¬Q) (implikatsiooni eemaldamine)
3. ¬¬P ∧ ¬¬Q (De Morgani seadus disjunktsioonile)
4. P ∧ Q (kahekordse eituse eemaldamine)

## Valemite normaalkujule viimine

Tihti on eesmärgiks viia valem mõnele standardkujule, nagu disjunktiivne normaalkuju (DNK) või konjunktiivne normaalkuju (KNK).

### Disjunktiivne normaalkuju (DNK)

Disjunktiivne normaalkuju on lihtkonjunktsioonide disjunktsioon:

(L₁₁ ∧ L₁₂ ∧ ... ∧ L₁ₙ) ∨ (L₂₁ ∧ L₂₂ ∧ ... ∧ L₂ₙ) ∨ ... ∨ (Lₘ₁ ∧ Lₘ₂ ∧ ... ∧ Lₘₙ)

kus L on literaal (muutuja või selle eitus).

**Näide:**
Viime valemi P ∧ (Q ∨ R) disjunktiivsele normaalkujule.

1. P ∧ (Q ∨ R)
2. (P ∧ Q) ∨ (P ∧ R) (distributiivsuse omadus)

See on juba disjunktiivsel normaalkujul, kus lihtkonjunktsioonid on P ∧ Q ja P ∧ R.

### Konjunktiivne normaalkuju (KNK)

Konjunktiivne normaalkuju on lihtdisjunktsioonide konjunktsioon:

(L₁₁ ∨ L₁₂ ∨ ... ∨ L₁ₙ) ∧ (L₂₁ ∨ L₂₂ ∨ ... ∨ L₂ₙ) ∧ ... ∧ (Lₘ₁ ∨ Lₘ₂ ∨ ... ∨ Lₘₙ)

kus L on literaal (muutuja või selle eitus).

**Näide:**
Viime valemi P ∨ (Q ∧ R) konjunktiivsele normaalkujule.

1. P ∨ (Q ∧ R)
2. (P ∨ Q) ∧ (P ∨ R) (distributiivsuse omadus)

See on juba konjunktiivsel normaalkujul, kus lihtdisjunktsioonid on P ∨ Q ja P ∨ R.

## Põhjalikud teisendamisnäited

Vaatame nüüd mõnda põhjalikumat näidet, mis illustreerivad, kuidas kombineerida erinevaid teisendamisvõtteid.

### Näide 1: Keerulisema valemi lihtsustamine

Lihtsustame valemit (P ⇒ Q) ∧ (¬P ∨ R) ∧ (¬Q ⇒ ¬R).

**Lahendus:**

1. Eemaldame implikatsioonid:
   (P ⇒ Q) ∧ (¬P ∨ R) ∧ (¬Q ⇒ ¬R)
   ≡ (¬P ∨ Q) ∧ (¬P ∨ R) ∧ (¬(¬Q) ∨ ¬R)
   ≡ (¬P ∨ Q) ∧ (¬P ∨ R) ∧ (Q ∨ ¬R)

2. Rakendame distributiivsust esimese kahe liikme vahel:
   (¬P ∨ Q) ∧ (¬P ∨ R) ∧ (Q ∨ ¬R)
   ≡ (¬P ∨ (Q ∧ R)) ∧ (Q ∨ ¬R)

3. Rakendame distributiivsust saadud avaldisele:
   (¬P ∨ (Q ∧ R)) ∧ (Q ∨ ¬R)
   ≡ (¬P ∧ (Q ∨ ¬R)) ∨ ((Q ∧ R) ∧ (Q ∨ ¬R))

4. Lihtsustame viimast liiget:
   (Q ∧ R) ∧ (Q ∨ ¬R)
   ≡ Q ∧ R, sest kui Q ∧ R on tõene, siis Q on tõene, seega Q ∨ ¬R on tõene.

5. Seega saame:
   (¬P ∧ (Q ∨ ¬R)) ∨ (Q ∧ R)

6. Rakendame distributiivsust esimesele liikmele:
   (¬P ∧ Q) ∨ (¬P ∧ ¬R) ∨ (Q ∧ R)

See on meie lihtsustatud valem disjunktiivsel normaalkujul.

### Näide 2: Valemi viimine täielikule disjunktiivsele normaalkujule

Viime valemi P ⇔ (Q ∧ ¬R) täielikule disjunktiivsele normaalkujule (TDNK).

**Lahendus:**

1. Asendame ekvivalentsi:
   P ⇔ (Q ∧ ¬R)
   ≡ (P ⇒ (Q ∧ ¬R)) ∧ ((Q ∧ ¬R) ⇒ P)
   ≡ (¬P ∨ (Q ∧ ¬R)) ∧ (¬(Q ∧ ¬R) ∨ P)

2. Rakendame De Morgani seadust teisele osale:
   (¬P ∨ (Q ∧ ¬R)) ∧ ((¬Q ∨ ¬¬R) ∨ P)
   ≡ (¬P ∨ (Q ∧ ¬R)) ∧ ((¬Q ∨ R) ∨ P)
   ≡ (¬P ∨ (Q ∧ ¬R)) ∧ (¬Q ∨ R ∨ P)

3. Rakendame distributiivsust:
   (¬P ∨ Q) ∧ (¬P ∨ ¬R) ∧ (¬Q ∨ R ∨ P)

4. Nüüd, iga disjunktsioon (¬P ∨ Q), (¬P ∨ ¬R) ja (¬Q ∨ R ∨ P) sisaldab erinevaid muutujaid. Täieliku disjunktiivse normaalkuju jaoks peame koostama kõigi muutujate (P, Q, R) kõigi võimalike kombinatsioonide disjunktsiooni.

5. Koostame tõeväärtustabeli:

   | P | Q | R | P ⇔ (Q ∧ ¬R) |
   |---|---|---|---------------|
   | t | t | t | v            |
   | t | t | v | t            |
   | t | v | t | v            |
   | t | v | v | v            |
   | v | t | t | v            |
   | v | t | v | v            |
   | v | v | t | t            |
   | v | v | v | t            |

6. Valides välja read, kus valem on tõene, saame TDNK:
   (P ∧ Q ∧ ¬R) ∨ (¬P ∧ ¬Q ∧ R) ∨ (¬P ∧ ¬Q ∧ ¬R)

See on valemi P ⇔ (Q ∧ ¬R) täielik disjunktiivne normaalkuju.

## Valemite teisendamise kasutamine praktilistes ülesannetes

Valemite teisendamine on kasulik paljudes praktilistes olukordades, eriti arvutiteaduses ja elektroonikas.

### Loogikaskeemide lihtsustamine

Elektroonikaskeemides kasutatakse loogikaväravaid, mis realiseerivad erinevaid loogilisi tehteid. Valemi lihtsustamine võib vähendada vajaminevate loogikaväravate arvu, mis tähendab väiksemat, odavamat ja energiatõhusamat skeemi.

**Näide:**
Olgu meil loogikaskeem, mis realiseerib valemi (P ∧ Q) ∨ (P ∧ ¬Q).

Lihtsustame:
1. (P ∧ Q) ∨ (P ∧ ¬Q)
2. P ∧ (Q ∨ ¬Q) (distributiivsuse omadus)
3. P ∧ t (Q ∨ ¬Q on tautoloogia, seega asendame selle tähisega t)
4. P (konjunktsioon tõesega annab alati operandi enda)

Seega, selle asemel et ehitada skeem, mis realiseerib (P ∧ Q) ∨ (P ∧ ¬Q), piisab lihtsast skeemist, mis väljastab sisendi P väärtuse.

### Programmeerimistingimuste lihtsustamine

Programmeerimises on tihti vaja lihtsustada keerulisi loogilisi tingimusi. Lihtsustamine muudab koodi loetavamaks, hooldatavamaks ja võib parandada jõudlust.

**Näide:**
Olgu meil tingimuslause:
```
if ((x > 0 && y > 0) || (x > 0 && !(y > 0)))
```

Märkides P: "x > 0" ja Q: "y > 0", saame valemi (P ∧ Q) ∨ (P ∧ ¬Q), mille lihtsustasime eelmises näites kujule P.

Seega tingimuslause lihtsustub:
```
if (x > 0)
```

### Teoreemitõestajad

Automaatsed teoreemitõestajad kasutavad valemite teisendamist, et viia valemid standardvormile, mille jaoks on olemas efektiivsed tõestusalgoritmid.

**Näide:** Resolutsioonimeetod nõuab, et valemid oleksid konjunktiivsel normaalkujul, kus iga liige on literaalide disjunktsioon.

## Teisendamise keerukamad meetodid

### Karnaugh' kaardid

Karnaugh' kaardid on graafiline meetod Boole'i funktsioonide lihtsustamiseks, mis on eriti kasulik digitaalse loogika disainis. Karnaugh' kaardid kasutavad visuaalset lähenemist, et leida optimaalne disjunktiivne või konjunktiivne normaalkuju.

### Quine-McCluskey algoritm

Quine-McCluskey algoritm on formaalse meetod Boole'i funktsioonide lihtsustamiseks. See on Karnaugh' kaartide algoritmiline alternatiiv, mis sobib eriti hästi rohkem kui nelja muutujaga funktsioonide jaoks.

## Teisendamise praktilised näpunäited

1. **Alusta lihtsamatest teisendamistest** - kõigepealt eemalda keerulisemad tehted nagu implikatsioonid ja ekvivalentsid.
2. **Järgi kindlat strateegiat** - näiteks, vii eitused vahetult muutujate ette ja seejärel kasuta distributiivsust, et saada soovitud normaalkuju.
3. **Kontrolli tulemust** - veendu, et lõpptulemus on samaväärne algvalemiga, kasutades tõeväärtustabelit või teisi kontrollimeetodeid.
4. **Kasuta teadaolevaid mustreid** - teatud valemid, nagu (P ∧ Q) ∨ (P ∧ ¬Q) = P, ilmnevad sageli ja nende tundmine võib säästa palju tööd.

## Kokkuvõte

Valemite teisendamine on oluline oskus lausearvutuses, mis leiab rakendust nii teoreetilises matemaatikas kui ka praktilistes valdkondades nagu arvutiteadus ja elektroonika. Teisendamine põhineb samaväärsusseostel, mis võimaldavad meil muuta valemi kuju, säilitades selle tõeväärtuse kõigi muutujate väärtustuste korral.

Olulisemad teisendamise võtted on:
- Tehete (implikatsioon, ekvivalents) eemaldamine
- Eituse sissetoomine (De Morgani seadused)
- Distributiivsuse kasutamine normaalkujule viimiseks
- Lihtsustamisvõtete rakendamine

Selle teemaga seostuvad tihedalt ka tõeväärtustabelid, samaväärsused ja normaalkujud. Valemite teisendamine nõuab hoolikat tähelepanu ja samaväärsuste põhjalikku tundmist, kuid on võimas tööriist loogiliste probleemide lahendamisel.