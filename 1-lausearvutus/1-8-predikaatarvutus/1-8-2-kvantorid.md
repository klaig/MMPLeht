# Kvantorid predikaatarvutuses

## Mis on kvantorid?

Predikaatarvutuse võimsus tuleneb suuresti kvantorite kasutamisest, mis võimaldavad meil teha üldistusi ja väljendada väiteid hulga kohta tervikuna või mõnede selle elementide kohta. Kvantorid on operaatorid, mis muudavad predikaadi lauseks, sidudes predikaadis esinevaid vabu muutujaid.

Predikaatarvutuses kasutatakse peamiselt kahte tüüpi kvantoreid:

1. **Üldisuskvantor (∀)**: väljendab, et mingi omadus kehtib kõikidele objektidele teatud hulgast
2. **Olemasolu kvantor (∃)**: väljendab, et leidub vähemalt üks objekt teatud hulgast, millel on mingi omadus

## Üldisuskvantor (∀)

Üldisuskvantor, mida tähistatakse sümboliga ∀, võimaldab väljendada, et mingi omadus kehtib kõigi objektide korral diskursuse universumis või mingis kitsendatud piirkonnas.

### Formaalne definitsioon

Olgu P(x) predikaat, mis sõltub muutujast x. Siis:

**∀x P(x)** tähendab, et "iga objekti x korral diskursuse universumis kehtib P(x)"

Lause ∀x P(x) on tõene parajasti siis, kui P(x) on tõene iga objekti x korral diskursuse universumis. Kui leidub kasvõi üks objekt, mille korral P(x) on väär, siis on kogu lause ∀x P(x) väär.

### Keeleline tähendus

Üldisuskvantorit väljendatakse tavakeeles sõnadega nagu:
- "kõik"
- "iga"
- "mistahes"
- "suvaline"
- "meelevaldne"

### Näited

1. **∀x (x² ≥ 0)** - "Iga arvu ruut on mittenegatiivne"
   - Kui diskursuse universumiks on reaalarvud, siis see väide on tõene

2. **∀x (Inimene(x) → Surelik(x))** - "Kõik inimesed on surelikud"
   - Kui diskursuse universumiks on kõik olendid, siis see väide väljendab, et kui x on inimene, siis x on surelik

3. **∀n (n ∈ ℕ → n + 1 > n)** - "Iga naturaalarvu korral on tema järgnev suurem kui tema ise"
   - See väide on tõene naturaalarvude hulgal

## Olemasolu kvantor (∃)

Olemasolu kvantor, mida tähistatakse sümboliga ∃, võimaldab väljendada, et leidub vähemalt üks objekt, millel on mingi omadus.

### Formaalne definitsioon

Olgu P(x) predikaat, mis sõltub muutujast x. Siis:

**∃x P(x)** tähendab, et "leidub vähemalt üks objekt x diskursuse universumis, mille korral kehtib P(x)"

Lause ∃x P(x) on tõene, kui leidub vähemalt üks objekt diskursuse universumis, mille korral P(x) on tõene. Kui selliseid objekte ei leidu, siis on lause ∃x P(x) väär.

### Keeleline tähendus

Olemasolu kvantorit väljendatakse tavakeeles sõnadega nagu:
- "leidub"
- "eksisteerib"
- "on olemas"
- "mõni"
- "vähemalt üks"

### Näited

1. **∃x (x² = 2)** - "Leidub arv, mille ruut on 2"
   - Kui diskursuse universumiks on reaalarvud, siis see väide on tõene (√2 on selline arv)
   - Kui diskursuse universumiks on ratsionaalarvud, siis see väide on väär (√2 on irratsionaalarv)

2. **∃x (Eestlane(x) ∧ NobelistiLaureaat(x))** - "Leidub eestlane, kes on Nobelisti laureaat"
   - Kui diskursuse universumiks on inimeste hulk, siis selle väite tõeväärtus sõltub faktidest

3. **∃n (n ∈ ℕ ∧ n > 100)** - "Leidub naturaalarv, mis on suurem kui 100"
   - See väide on tõene naturaalarvude hulgal

## Ainuline olemasolu (∃!)

Lisaks tavalisele olemasolu kvantorile kasutatakse mõnikord märgistust ∃!, mis tähistab "leidub täpselt üks".

**∃!x P(x)** tähendab, et "leidub täpselt üks objekt x diskursuse universumis, mille korral kehtib P(x)"

Lause ∃!x P(x) on samaväärne lausega ∃x (P(x) ∧ ∀y (P(y) → y = x)), mis ütleb, et leidub selline x, et P(x) on tõene, ja iga y korral, kui P(y) on tõene, siis y on identne x-ga.

### Näide

**∃!x (x + 3 = 5)** - "Leidub täpselt üks arv, mis liidetuna 3-ga annab 5"
- See on tõene, sest ainult arv 2 rahuldab seda tingimust

## Kvantorite piirkond ja ulatus

Kvantorite kasutamisel on oluline määratleda **kvantorite piirkond** või **ulatus** (scope), mis näitab, millise valemi osa kohta kvantor kehtib.

### Süntaktiliselt

Kvantorid ∀ ja ∃ seovad muutujat oma vahetult järgnevas valemis. Tavaliselt tähistab sulg kvantorite piirkonda.

Näiteks valemis ∀x (P(x) → Q(x)) on üldisuskvantoriga seotud kogu alamvalem P(x) → Q(x).

### Prioriteet ja järjekord

Kvantorite prioriteet on sama, mis eituse prioriteet – kõrgem kui loogilistel tehetel. See tähendab, et kui pole teisiti märgitud, on kvantorite ulatus maksimaalne.

Näiteks valem ∀x P(x) → Q(x) tõlgendatakse kui (∀x P(x)) → Q(x), mitte kui ∀x (P(x) → Q(x)).

## Kvantorite järjekord

Kvantorite järjekord on väga oluline ning võib oluliselt muuta valemi tähendust.

### Sama tüüpi kvantorid

Kui kaks või enam sama tüüpi kvantorit (kas kõik ∀ või kõik ∃) on järjestikku, siis nende järjekorda saab vahetada ilma valemi tähendust muutmata:

- ∀x ∀y P(x, y) ≡ ∀y ∀x P(x, y)
- ∃x ∃y P(x, y) ≡ ∃y ∃x P(x, y)

### Erinevat tüüpi kvantorid

Kui on kaks erinevat tüüpi kvantorit (∀ ja ∃), siis nende järjekorda vahetades muutub tavaliselt valemi tähendus:

- ∀x ∃y P(x, y) ≢ ∃y ∀x P(x, y)

Vaatame näidet:

**∀x ∃y (y > x)** - "Iga arvu x korral leidub arv y, mis on suurem kui x"
- Kui diskursuse universumiks on reaalarvud, siis see väide on tõene

**∃y ∀x (y > x)** - "Leidub selline arv y, et iga arvu x korral on y suurem kui x"
- Kui diskursuse universumiks on reaalarvud, siis see väide on väär, sest pole olemas suurimat reaalarvul

### Kvantorite permutatsioonist üldisemalt

Üldiselt kehtivad järgmised implikatsioonid:
- ∀x ∀y P(x, y) → ∀y ∀x P(x, y) (kehtib samaväärsus)
- ∃x ∃y P(x, y) → ∃y ∃x P(x, y) (kehtib samaväärsus)
- ∀x ∃y P(x, y) ← ∃y ∀x P(x, y) (implikatsioon paremalt vasakule)

Viimane implikatsioon näitab, et kui leidub üks objekt, mis rahuldab tingimust kõigi teiste objektide jaoks, siis kindlasti leidub igale objektile vastav objekt, mis rahuldab tingimust.

## Kvantorite kasutamine tingimuslike väidetega

Sageli kasutatakse kvantoreid koos implikatsiooniga, et väljendada tingimusi teatud alamhulga kohta.

### Iga x korral, kui on P, siis on Q

Tüüpiline vorm on ∀x (P(x) → Q(x)), näiteks:
- "Kõik linnud on lendavad olendid" ⟺ ∀x (Lind(x) → Lendab(x))

### Leidub x, mis on P ja Q

Tüüpiline vorm on ∃x (P(x) ∧ Q(x)), näiteks:
- "Mõned linnud on valged" ⟺ ∃x (Lind(x) ∧ Valge(x))

### Eitatud kvantorid

Kvantorite kasutamisel tingimuslike lausete eitamiseks on samuti tüüpilisi mustreid:
- "Mitte kõik linnud pole valged" ⟺ ¬∀x (Lind(x) → Valge(x)) ⟺ ∃x (Lind(x) ∧ ¬Valge(x))
- "Ükski lind pole valge" ⟺ ∀x (Lind(x) → ¬Valge(x)) ⟺ ¬∃x (Lind(x) ∧ Valge(x))

## Predikaatide formaliseerimine kvantorite abil

Predikaatarvutuse võimsus tuleb esile eriti siis, kui kombineerime kvantoreid, loogilisi tehteid ja predikaate, et formaliseerida keerulisi väiteid.

### Näide 1: Transitiivsus

"Kui üks arv on suurem kui teine ja teine on suurem kui kolmas, siis esimene on suurem kui kolmas."

Formaliseerimine:
∀x ∀y ∀z ((x > y ∧ y > z) → x > z)

### Näide 2: Pidevus

"Funktsioon f on pidev punktis a, kui iga positiivse reaalarvu ε korral leidub positiivne reaalarv δ nii, et kui kaugus punktist x punktini a on väiksem kui δ, siis kaugus f(x)-st f(a)-ni on väiksem kui ε."

Formaliseerimine:
∀ε (ε > 0 → ∃δ (δ > 0 ∧ ∀x (|x - a| < δ → |f(x) - f(a)| < ε)))

### Näide 3: Lõplikkus

"Hulk A on lõplik, kui leidub naturaalarv n ja bijektsioon hulga A ja hulga {1,2,...,n} vahel."

Formaliseerimine:
∃n (n ∈ ℕ ∧ ∃f (Bijektsioon(f) ∧ Dom(f) = A ∧ Rng(f) = {1, 2, ..., n}))

## Keerukamad kvantorite järgnevused

Praktilised matemaatilised väited sisaldavad sageli mitut erinevat kvantorit, mis loovad keerukaid struktuure. Kuigi need võivad esmapilgul tunduda keerulised, on neid võimalik süstemaatiliselt analüüsida, kui mõistame kvantorite tähendust.

### Näide: ∃∀∃-tüüpi väide

"Leidub selline naturaalarv M, et iga naturaalarvu n korral leidub naturaalarv m > M nii, et m jagub n-ga."

Formaliseeritud kujul:
∃M ∀n (n ∈ ℕ → ∃m (m ∈ ℕ ∧ m > M ∧ n|m))

kus n|m tähendab "n jagab m-i" ehk "m jagub n-ga".

Analüüsime seda väidet:
1. Esmalt, ∃M - leidub vähemalt üks naturaalarv M
2. Seejärel, ∀n - iga naturaalarvu n korral
3. Lõpuks, ∃m - leidub naturaalarv m, mis on suurem kui M ja jagub n-ga

See väide on tõene: võime võtta M = 1, siis iga n ∈ ℕ korral leidub m = 2n > 1, mis jagub n-ga.

## Kvantorite kasutamine järelduste tegemisel

Kvantorid on olulised matemaatilistes tõestustes ja järelduste tegemisel. Vaatame mõnda põhilist järeldusreeglit, mis puudutavad kvantoreid.

### Universaalne instantseerimine (UI)

Kui teame, et mingi omadus kehtib kõigi objektide korral, siis võime järeldada, et see kehtib iga konkreetse objekti korral.

∀x P(x) ⊨ P(a)

kus a on suvaline term diskursuse universumist.

### Eksistentsiaalne instantseerimine (EI)

Kui teame, et leidub objekt, millel on mingi omadus, siis võime seda objekti tähistada mingi konkreetse termiga ja järeldada, et sellel on vastav omadus.

∃x P(x) ⊨ P(c)

kus c on konstant, mis ei esine teistes eeldustes ega järelduses.

### Universaalne üldistamine (UG)

Kui saame tuletada omaduse P(x) suvalise objekti x kohta, ilma et teeks eeldusi x kohta, siis võime järeldada, et see omadus kehtib kõigi objektide korral.

P(x) ⊨ ∀x P(x)

kui x ei sõltu ühestki eeldusest.

### Eksistentsiaalne üldistamine (EG)

Kui teame, et mingi konkreetne objekt a rahuldab omadust P, siis võime järeldada, et leidub objekt, mis rahuldab seda omadust.

P(a) ⊨ ∃x P(x)

## Kvantorite kasutamine igapäevaelulistes väidetes

Kvantoritega formaliseeritud väiteid leidub sageli ka igapäevaelus, kuigi me ei pruugi neid otseselt nii mõtestada. Vaatame mõnda näidet:

### Näide 1: Ülikool

"Iga ülikooli tudeng peab sooritama vähemalt ühe eksami."

Formaliseerimine:
∀x (Tudeng(x) → ∃y (Eksam(y) ∧ Sooritab(x, y)))

### Näide 2: Restoranid

"Mõned restoranid serveerivad kõiki toite."

Formaliseerimine:
∃x (Restoran(x) ∧ ∀y (Toit(y) → Serveerib(x, y)))

### Näide 3: Transpordivahendid

"Iga inimene kasutab mingit transpordivahendit."

Formaliseerimine:
∀x (Inimene(x) → ∃y (Transpordivahend(y) ∧ Kasutab(x, y)))

## Kvantorite järjekorra tähtsus praktikas

Kvantorite järjekorra mõistmine on oluline paljudes valdkondades, sealhulgas matemaatikas, informaatikas ja andmebaasides.

### Andmebaasipäringute näide

Võtame näiteks järgmised päringud:

1. "Leia kõik kursused, millel on vähemalt üks tudeng" (∀x∃y)
   ```sql
   SELECT course_id FROM Courses 
   WHERE EXISTS (SELECT 1 FROM Enrollment WHERE Enrollment.course_id = Courses.id)
   ```

2. "Leia kõik tudengid, kes on registreeritud kõigile kursustele" (∃x∀y)
   ```sql
   SELECT student_id FROM Students s
   WHERE NOT EXISTS (
     SELECT 1 FROM Courses c
     WHERE NOT EXISTS (
       SELECT 1 FROM Enrollment e
       WHERE e.student_id = s.id AND e.course_id = c.id
     )
   )
   ```

Need kaks päringut on oluliselt erinevad ja nende järjekorra vahetamine muudaks täielikult nende tähendust.

## Kokkuvõte

Kvantorid on oluline osa predikaatarvutusest, mis võimaldavad meil väljendada üldistusi ja olemasoluväiteid objektide kohta diskursuse universumis. Nende kasutamine koos predikaatide ja loogiliste tehetega loob tugeva formaalse keele, millega saab täpselt kirjeldada keerulisi matemaatilisi ja igapäevaelulisi väiteid.

Kõige olulisemad punktid, mida kvantoritest meeles pidada:

1. **Üldisuskvantor (∀)** väljendab väidet, mis kehtib kõigi objektide korral.
2. **Olemasolu kvantor (∃)** väljendab väidet, mis kehtib vähemalt ühe objekti korral.
3. **Kvantorite järjekord** on oluline ja muudab tavaliselt valemi tähendust.
4. **Sama tüüpi kvantoreid** saab omavahel vahetada, säilitades valemi tähenduse.
5. **Erinevat tüüpi kvantorite** järjekorra vahetamine muudab üldjuhul valemi tähendust.

Kvantorite mõistmine ja korrektne kasutamine on oluline oskus paljudes valdkondades, alates matemaatikast ja loogikast kuni informaatika ja andmebaaside disainini.