# Hulgatehted

Hulgatehted on operatsioonid, mis võimaldavad meil kombineerida hulki erinevatel viisidel, luues uusi hulki. Need tehted on hulgateooria põhitööriistad, mille abil saame hulki analüüsida ja nende vahelisi seoseid väljendada. Sarnaselt sellele, kuidas aritmeetikas kombineerime arve (liites, lahutades, korrutades), kombineerime hulgateorias hulki erinevate tehete abil.

## Hulkade ühend (union)

**Definitsioon:** Hulkade A ja B ühendiks nimetatakse hulka, mille moodustavad kõik elemendid, mis kuuluvad vähemalt ühte hulkadest A või B. Ühendi tähistamiseks kasutatakse sümbolit ∪.

Formaalselt:
A ∪ B = {x | x ∈ A või x ∈ B}

Intuitiivselt võib ühendi mõista kui "kõik elemendid, mis on hulgas A VÕI hulgas B (või mõlemas)". Sidesõna "või" kasutatakse siin mittevälistavas tähenduses, mis tähendab, et element võib kuuluda nii hulka A kui ka hulka B.

**Näited:**
- Kui A = {1, 2, 3} ja B = {3, 4, 5}, siis A ∪ B = {1, 2, 3, 4, 5}
- Kui C = {a, b, c} ja D = {d, e, f}, siis C ∪ D = {a, b, c, d, e, f}
- Kui E = {1, 2, 3} ja F = {1, 2, 3}, siis E ∪ F = {1, 2, 3}

**Omadused:**
1. **Kommutatiivsus:** A ∪ B = B ∪ A
2. **Assotsiatiivsus:** (A ∪ B) ∪ C = A ∪ (B ∪ C)
3. **Idempotentsus:** A ∪ A = A
4. **Neeldumisomadus:** A ∪ (A ∩ B) = A
5. **Identiteet tühja hulgaga:** A ∪ ∅ = A
6. **Identiteet universumiga:** A ∪ U = U

## Hulkade ühisosa (intersection)

**Definitsioon:** Hulkade A ja B ühisosaks (või lõikeks) nimetatakse hulka, mille moodustavad kõik elemendid, mis kuuluvad samaaegselt nii hulka A kui ka hulka B. Ühisosa tähistamiseks kasutatakse sümbolit ∩.

Formaalselt:
A ∩ B = {x | x ∈ A ja x ∈ B}

Intuitiivselt võib ühisosa mõista kui "kõik elemendid, mis on hulgas A JA hulgas B".

**Näited:**
- Kui A = {1, 2, 3} ja B = {3, 4, 5}, siis A ∩ B = {3}
- Kui C = {a, b, c} ja D = {d, e, f}, siis C ∩ D = ∅ (tühi hulk)
- Kui E = {1, 2, 3} ja F = {1, 2, 3}, siis E ∩ F = {1, 2, 3}

**Omadused:**
1. **Kommutatiivsus:** A ∩ B = B ∩ A
2. **Assotsiatiivsus:** (A ∩ B) ∩ C = A ∩ (B ∩ C)
3. **Idempotentsus:** A ∩ A = A
4. **Neeldumisomadus:** A ∩ (A ∪ B) = A
5. **Identiteet universumiga:** A ∩ U = A
6. **Identiteet tühja hulgaga:** A ∩ ∅ = ∅

## Hulkade vahe (difference)

**Definitsioon:** Hulkade A ja B vaheks nimetatakse hulka, mille moodustavad kõik elemendid, mis kuuluvad hulka A, aga ei kuulu hulka B. Vahe tähistamiseks kasutatakse sümboleid A \ B või A - B.

Formaalselt:
A \ B = {x | x ∈ A ja x ∉ B}

Intuitiivselt võib hulkade vahet mõista kui "kõik elemendid, mis on hulgas A, aga EI OLE hulgas B". 

**Näited:**
- Kui A = {1, 2, 3, 4, 5} ja B = {4, 5, 6, 7}, siis A \ B = {1, 2, 3}
- Kui C = {a, b, c} ja D = {d, e, f}, siis C \ D = {a, b, c}
- Kui E = {1, 2, 3} ja F = {1, 2, 3}, siis E \ F = ∅

**Omadused:**
1. **Vahe tühja hulgaga:** A \ ∅ = A
2. **Vahe iseendaga:** A \ A = ∅
3. **Vahe universumiga:** A \ U = ∅
4. **Tühja hulga vahe:** ∅ \ A = ∅
5. **Vahe pole kommutatiivne:** Üldiselt A \ B ≠ B \ A
6. **Distributiivsus ühisosaga:** A \ (B ∩ C) = (A \ B) ∪ (A \ C)

Märkus: Erinevalt ühendist ja ühisosast ei ole vahe kommutatiivne tehe, mis tähendab, et A \ B ei ole üldiselt sama, mis B \ A. Näiteks, kui A = {1, 2, 3} ja B = {3, 4, 5}, siis A \ B = {1, 2}, aga B \ A = {4, 5}.

## Sümmeetriline vahe (symmetric difference)

**Definitsioon:** Hulkade A ja B sümmeetriliseks vaheks nimetatakse hulka, mille moodustavad elemendid, mis kuuluvad kas hulka A või hulka B, aga mitte mõlemasse korraga. Sümmeetrilist vahet tähistatakse sümboliga △ või ⊕.

Formaalselt:
A △ B = (A \ B) ∪ (B \ A) = (A ∪ B) \ (A ∩ B)

Intuitiivselt võib sümmeetrilist vahet mõista kui "kõik elemendid, mis on ainult ühes hulgas, aga mitte mõlemas".

**Näited:**
- Kui A = {1, 2, 3, 4} ja B = {3, 4, 5, 6}, siis A △ B = {1, 2, 5, 6}
- Kui C = {a, b, c} ja D = {d, e, f}, siis C △ D = {a, b, c, d, e, f}
- Kui E = {1, 2, 3} ja F = {1, 2, 3}, siis E △ F = ∅

**Omadused:**
1. **Kommutatiivsus:** A △ B = B △ A
2. **Assotsiatiivsus:** (A △ B) △ C = A △ (B △ C)
3. **Identiteet tühja hulgaga:** A △ ∅ = A
4. **Inversioon iseendaga:** A △ A = ∅
5. **Kasutatav osahulga tingimusena:** A ⊆ B parajasti siis, kui A △ B = B \ A

Märkus: Sümmeetriline vahe on oluline matemaatikas ja arvutiteaduses, eriti hulkade vaheliste erinevuste analüüsimisel.

## Hulga täiend (complement)

**Definitsioon:** Hulga A täiendiks universumi U suhtes nimetatakse hulka, mille moodustavad kõik universumi elemendid, mis ei kuulu hulka A. Täiendit tähistatakse tavaliselt sümboliga A', A^c või Ā.

Formaalselt:
A' = U \ A = {x | x ∈ U ja x ∉ A}

Intuitiivselt võib täiendit mõista kui "kõik elemendid universumist, mis EI OLE hulgas A".

**Näited:**
- Kui universumiks on U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10} ja A = {1, 3, 5, 7, 9}, siis A' = {2, 4, 6, 8, 10}
- Kui universumiks on naturaalarvud ℕ ja B = {paaris naturaalarvud}, siis B' = {paaritud naturaalarvud}
- Kui universumiks on reaalsed arvud ℝ ja C = [0, 1] (kõik reaalarvud 0 ja 1 vahel, kaasa arvatud), siis C' = (-∞, 0) ∪ (1, ∞)

**Omadused:**
1. **Kahekordne täiend:** (A')' = A
2. **Tühja hulga täiend:** ∅' = U
3. **Universumi täiend:** U' = ∅
4. **Täiend ja ühend (De Morgani seadus):** (A ∪ B)' = A' ∩ B'
5. **Täiend ja ühisosa (De Morgani seadus):** (A ∩ B)' = A' ∪ B'

## De Morgani seadused

De Morgani seadused on hulgateooria olulised tulemused, mis kirjeldavad seoseid hulgatehete ja täiendi vahel.

**De Morgani I seadus:**
(A ∪ B)' = A' ∩ B'

See tähendab, et hulkade ühendi täiend on võrdne hulkade täiendite ühisosaga.

**De Morgani II seadus:**
(A ∩ B)' = A' ∪ B'

See tähendab, et hulkade ühisosa täiend on võrdne hulkade täiendite ühendiga.

Neid seadusi saab illustreerida järgmise näitega:

**Näide:**
Olgu U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}, A = {1, 2, 3, 4} ja B = {3, 4, 5, 6}.

Kontrollime De Morgani I seadust:
- A ∪ B = {1, 2, 3, 4, 5, 6}
- (A ∪ B)' = {7, 8, 9, 10}

- A' = {5, 6, 7, 8, 9, 10}
- B' = {1, 2, 7, 8, 9, 10}
- A' ∩ B' = {7, 8, 9, 10}

Näeme, et (A ∪ B)' = A' ∩ B'.

De Morgani seadused laienevad ka suuremale hulkade arvule:
- (A₁ ∪ A₂ ∪ ... ∪ Aₙ)' = A₁' ∩ A₂' ∩ ... ∩ Aₙ'
- (A₁ ∩ A₂ ∩ ... ∩ Aₙ)' = A₁' ∪ A₂' ∪ ... ∪ Aₙ'

De Morgani seadused on kasulikud mitte ainult hulgateooria kontekstis, vaid ka loogikas ja digitaalsete skeemide disainis.

## Hulgatehete omadused

Hulgatehete vahel on mitmeid olulisi seoseid ja omadusi, mis meenutavad arvude korral kehtivaid algebralisi omadusi. Olulisemad neist on:

### Distributiivsuse seadused

1. A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C)
2. A ∪ (B ∩ C) = (A ∪ B) ∩ (A ∪ C)

Need seadused näitavad, kuidas ühisosa ja ühend jaotuvad üksteise üle, sarnaselt korrutamise ja liitmise distributiivsusele arvude korral.

### Tõestatusvõtted hulgatehete puhul

Hulgatehete omaduste tõestamiseks on mitu viisi:

1. **Elementide meetod**: Näidatakse, et x ∈ vasakpoolne avaldis ⟺ x ∈ parempoolne avaldis.
2. **Otsene arvutamine**: Arvutame hulgatehted välja ja vaatame, kas tulemus on sama.
3. **Venni diagrammid**: Visuaalselt näitame, et kaks hulka kattuvad.

**Näide elementide meetodist**: Tõestame, et A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C).

Tõestus:
- x ∈ A ∩ (B ∪ C)
- ⟺ x ∈ A ja x ∈ (B ∪ C)
- ⟺ x ∈ A ja (x ∈ B või x ∈ C)
- ⟺ (x ∈ A ja x ∈ B) või (x ∈ A ja x ∈ C)
- ⟺ x ∈ (A ∩ B) või x ∈ (A ∩ C)
- ⟺ x ∈ (A ∩ B) ∪ (A ∩ C)

## Boole'i algebra hulkadel

Hulgatehted moodustavad algebralise struktuuri, mida nimetatakse Boole'i algebraks (George Boole'i auks). Boole'i algebra hulkade korral hõlmab järgmisi operatsioone ja elemente:

- Kaks binaarset operatsiooni: ühend (∪) ja ühisosa (∩)
- Unaarne operatsioon: täiend (')
- Kaks erilist elementi: tühi hulk (∅) ja universum (U)

Boole'i algebra leiab rakendust digitaalelektroonikas, kus:
- Ühend (∪) vastab OR-loogikale
- Ühisosa (∩) vastab AND-loogikale
- Täiend (') vastab NOT-loogikale
- Tühi hulk (∅) vastab loogilisele 0-le
- Universum (U) vastab loogilisele 1-le

## Kartesiaanlik korrutis (Cartesian product)

Lisaks klassikalistele hulgatehetele on oluliseks tehteks ka **kartesiaanlik korrutis** (nimetatud René Descartes'i järgi).

**Definitsioon:** Hulkade A ja B kartesiaanliku korrutise A × B all mõistetakse kõigi selliste järjestatud paaride (a, b) hulka, kus a ∈ A ja b ∈ B.

Formaalselt:
A × B = {(a, b) | a ∈ A, b ∈ B}

Intuitiivselt võib kartesiaanlikku korrutist mõista kui "kõik võimalikud paarid, kus esimene element on hulgast A ja teine element on hulgast B".

**Näited:**
- Kui A = {1, 2} ja B = {a, b, c}, siis 
  A × B = {(1, a), (1, b), (1, c), (2, a), (2, b), (2, c)}
- Kui C = {x, y} ja D = {x, y}, siis 
  C × D = {(x, x), (x, y), (y, x), (y, y)}
- Kui E = {1, 2, 3} ja F = ∅, siis E × F = ∅

**Omadused:**
1. |A × B| = |A| × |B| (kartesiaanliku korrutise võimsus on hulkade võimsuste korrutis)
2. Üldjuhul A × B ≠ B × A (kartesiaanlik korrutis ei ole kommutatiivne)
3. A × (B ∪ C) = (A × B) ∪ (A × C)
4. A × (B ∩ C) = (A × B) ∩ (A × C)
5. Kui A ≠ ∅ ja B ≠ ∅, siis A × B ≠ ∅

Kartesiaanlikku korrutist saab laiendada rohkem kui kahele hulgale:
A₁ × A₂ × ... × Aₙ = {(a₁, a₂, ..., aₙ) | a₁ ∈ A₁, a₂ ∈ A₂, ..., aₙ ∈ Aₙ}

Kartesiaanlik korrutis on oluline mõiste mitmetes matemaatika valdkondades:
- Koordinaattasand on kartesiaanlik korrutis R × R (või lühidalt R²)
- Relatsioonid defineeritakse kui kartesiaanliku korrutise alamhulgad
- Funktsioonid f: A → B defineeritakse kui erilised relatsioonid A × B

## Hulkade perekonna tehted

Kui meil on hulkade kogu (hulkade perekond), tähistatakse seda tavaliselt {Aₗ}ᵢ₌₁..ₙ või lihtsalt {Aᵢ} (kus i on indeks).

Sellise hulkade perekonna korral saame defineerida:

**Ühendi** ⋃ᵢ₌₁ⁿAᵢ = A₁ ∪ A₂ ∪ ... ∪ Aₙ = {x | leidub i (1 ≤ i ≤ n), et x ∈ Aᵢ}

**Ühisosa** ⋂ᵢ₌₁ⁿAᵢ = A₁ ∩ A₂ ∩ ... ∩ Aₙ = {x | iga i (1 ≤ i ≤ n) korral x ∈ Aᵢ}

**Näide:**
Olgu A₁ = {1, 2, 3}, A₂ = {2, 3, 4}, A₃ = {3, 4, 5}.
- ⋃ᵢ₌₁³Aᵢ = A₁ ∪ A₂ ∪ A₃ = {1, 2, 3, 4, 5}
- ⋂ᵢ₌₁³Aᵢ = A₁ ∩ A₂ ∩ A₃ = {3}

## Lõplikud ja lõpmatud ühendid ja ühisosad

Hulkade jada A₁, A₂, A₃, ... ühendi ja ühisosa saame defineerida järgmiselt:
- ⋃∞ᵢ₌₁Aᵢ = A₁ ∪ A₂ ∪ A₃ ∪ ... = {x | ∃i ∈ ℕ nii, et x ∈ Aᵢ}
- ⋂∞ᵢ₌₁Aᵢ = A₁ ∩ A₂ ∩ A₃ ∩ ... = {x | ∀i ∈ ℕ korral x ∈ Aᵢ}

**Näide:**
Olgu iga i ∈ ℕ korral Aᵢ = {-i, 0, i}. Siis
- ⋃∞ᵢ₌₁Aᵢ = ℤ (kõigi täisarvude hulk)
- ⋂∞ᵢ₌₁Aᵢ = {0} (ainult 0 kuulub kõikidesse hulkadesse)

Olgu I = [1, 4] ja iga α ∈ I korral Aα = [0, α]. Siis
- ⋃α∈IAα = ⋃α∈[1,4]Aα = [0, 4]
- ⋂α∈IAα = ⋂α∈[1,4]Aα = [0, 1]

De Morgani seadused laienevad ka lõpmatutele ühendidele ja ühisosadele:
- (⋃ᵢAᵢ)' = ⋂ᵢAᵢ'
- (⋂ᵢAᵢ)' = ⋃ᵢAᵢ'

## Hulgatehete rakendused

Hulgatehted on põhitööriistad paljudes matemaatika ja arvutiteaduse valdkondades. Siin on mõned olulised rakendused:

### 1. Andmebaasiteooria

Relatsioonilistes andmebaasides kasutatakse hulgatehted päringute koostamiseks. SQL-keeles on olemas sellised operaatorid nagu UNION, INTERSECT ja EXCEPT (vahe).

**Näide SQL-is:**
```sql
-- Ühend
SELECT * FROM tabel1 UNION SELECT * FROM tabel2;

-- Ühisosa
SELECT * FROM tabel1 INTERSECT SELECT * FROM tabel2;

-- Vahe
SELECT * FROM tabel1 EXCEPT SELECT * FROM tabel2;
```

### 2. Tõenäosusteooria

Tõenäosusteooria kasutab hulgateooria mõisteid sündmuste kirjeldamiseks:
- Sündmuste summa (A ∪ B): Toimub vähemalt üks sündmus A või B
- Sündmuste korrutis (A ∩ B): Toimuvad mõlemad sündmused A ja B
- Vastandsündmus (A'): Sündmus A ei toimu

### 3. Programmeerimiskeeled

Paljudes programmeerimiskeeltes on sisseehitatud toed hulkadele ja hulgatehetele.

**Näide Python-is:**
```python
# Hulgad
A = {1, 2, 3, 4}
B = {3, 4, 5, 6}

# Hulgatehted
union = A | B        # Ühend: {1, 2, 3, 4, 5, 6}
intersection = A & B  # Ühisosa: {3, 4}
difference = A - B    # Vahe: {1, 2}
symm_diff = A ^ B     # Sümmeetriline vahe: {1, 2, 5, 6}
```

## Kokkuvõte

Hulgatehted on hulgateooria kesksed operatsioonid, mis võimaldavad meil kombineerida ja manipuleerida hulkadega. Peamised hulgatehted on:

1. **Ühend (∪)** - elemendid, mis kuuluvad vähemalt ühte kahest hulgast
2. **Ühisosa (∩)** - elemendid, mis kuuluvad mõlemasse hulka
3. **Vahe (\\)** - elemendid, mis kuuluvad esimesse, aga mitte teisse hulka
4. **Sümmeetriline vahe (△)** - elemendid, mis kuuluvad ühte, aga mitte mõlemasse hulka
5. **Täiend (')** - elemendid universumist, mis ei kuulu antud hulka
6. **Kartesiaanlik korrutis (×)** - kõik võimalikud järjestatud paarid hulkade elementidest

Neid tehteid saab kombineerida keerulisemate avaldiste loomiseks, kasutades distributiivususe ja De Morgani seadusi. Hulgatehted on fundamentaalsed tööriistad paljudes matemaatika ja arvutiteaduse valdkondades, kaasa arvatud tõenäosusteooria, andmebaasiteoorias, loogika ja arvutiteaduses.