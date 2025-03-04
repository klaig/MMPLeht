# Hulgateooria põhimõisted

## Mis on hulk?

**Definitsioon:** Hulga all mõistetakse üksteisest erinevate objektide kogumit, mida vaadeldakse ühe tervikuna ja kus iga objekti korral on võimalik üheselt kindlaks määrata, kas ta kuulub antud hulka või mitte.

Hulgateooria rajaja Georg Cantor sõnastas hulga kui sellise omavahel erinevate objektide kogu, millest saab mõelda kui tervikust. See definitsioon tähendab, et hulka kuuluvad objektid peavad olema omavahel erinevad ja iga objekti puhul peab olema selge, kas see kuulub hulka või mitte.

Objekte, mis moodustavad hulga (kuuluvad hulka), nimetatakse **hulga elementideks**. Oluline on märkida, et hulk ja element on erinevad objektid – hulk koosneb elementidest, kuid ei ole ise element (välja arvatud teistes hulkades, mis on ise hulkade hulgad).

Hulga elemendid võivad olla mistahes objektid: arvud, punktid, funktsioonid, või isegi teised hulgad. Ainuke tingimus on, et peab olema selge, kas objekt kuulub hulka või mitte.

Võrreldes igapäevaeluga võib hulka kujutleda kui karpi, kuhu on pandud kokku kuuluvad asjad – karp on hulk ja asjad karbi sees on hulga elemendid.

## Hulkade tähistamine

Hulki tähistatakse tavaliselt suurte ladina tähtedega (A, B, C, X, Y, Z jne), hulkade elemente aga väikeste ladina tähtedega (a, b, c, x, y, z jne).

### Elemendi kuuluvus hulka

Fakti, et element a kuulub hulka A, tähistatakse sümboliga "∈":

a ∈ A

Kui element a ei kuulu hulka A, tähistatakse seda sümboliga "∉":

a ∉ A

**Näide:**  
Kui A = {1, 2, 3, 4, 5}, siis 3 ∈ A, aga 9 ∉ A.

## Hulga esitamise viisid

Hulka saab esitada peamiselt kolmel viisil:

### 1. Loendamise teel

Kui hulk koosneb väikesest arvust elementidest, siis võib need elemendid looksulgude vahel komadega eraldatult üles loetleda.

**Näited:**
- A = {1, 2, 3}
- B = {a, e, i, o, u}
- C = {punane, sinine, kollane, roheline}

Elementide järjekord hulgas ei ole oluline. Seega:
- {1, 2, 3} = {3, 2, 1} = {2, 1, 3}
- {a, b, c} = {c, b, a}

Kui element esineb loetelus korduvalt, siis arvestatakse teda vaid üks kord. Näiteks:
- {1, 2, 3, 1} = {1, 2, 3}

### 2. Omaduste või tingimuste abil

Hulga saab määrata ka hulka kuulumise tingimuse abil. Selleks kasutatakse looksulgude sees toonitust, kus vertikaaljoonega (|) või kooloniga (:) eraldatakse muutuja ja tingimus.

S = {x | x rahuldab tingimust P(x)}

või

S = {x : P(x)}

kus P(x) tähistab tingimust või tingimuste loetelu, mida hulka S kuuluvad elemendid x peavad rahuldama.

**Näited:**
- A = {x | x on naturaalarv ja x < 6} = {1, 2, 3, 4, 5}
- B = {x | x on täisarv ja -2 ≤ x ≤ 2} = {-2, -1, 0, 1, 2}
- C = {x | x on täht sõnas "matemaatika"} = {m, a, t, e, i, k}

### 3. Rekursiivselt

Mõnikord defineeritakse hulk rekursiivselt, määrates mõned algelemendid ja seejärel reeglid, kuidas hulga elemente moodustada.

**Näide:** Fibonacci arvude hulk F saab defineerida rekursiivselt:
- F₀ = 0 ja F₁ = 1 on hulgas F
- Kui F_{n-2} ja F_{n-1} on hulgas F, siis ka F_n = F_{n-2} + F_{n-1} on hulgas F

## Hulkade võrdsus

**Definitsioon:** Kaks hulka A ja B on võrdsed (tähistatakse A = B) parajasti siis, kui need hulgad koosnevad täpselt samadest elementidest.

Formaalselt:
A = B parajasti siis, kui ∀x (x ∈ A ⟺ x ∈ B)

Ehk hulk A on võrdne hulgaga B ainult siis, kui iga element, mis kuulub A-sse, kuulub ka B-sse, ja vastupidi, iga element, mis kuulub B-sse, kuulub ka A-sse.

**Näide:**  
Hulgad {1, 2, 3} ja {3, 2, 1} on võrdsed, sest elementide järjekord hulgas ei ole oluline.
Hulgad {a, b, c} ja {a, b, c, a} on samuti võrdsed, sest element a esineb mõlemas hulgas (korduvalt loetlemine ei lisa hulka uusi elemente).
Hulgad {1, 2, 3} ja {1, 2, 3, 4} ei ole võrdsed, sest hulgas {1, 2, 3, 4} on element, mida ei leidu hulgas {1, 2, 3}.

## Tühi hulk

**Definitsioon:** Tühi hulk on hulk, mis ei sisalda ühtegi elementi. Tühja hulka tähistatakse sümboliga ∅ või {}.

Tühi hulk on üheselt määratud, mis tähendab, et on ainult üks tühi hulk. Kõik tühjad hulgad on omavahel võrdsed. 

**Omadused:**
- Iga hulga alamhulk on tühi hulk: ∅ ⊆ A iga hulga A korral
- Tühi hulk on alamhulk iseendale: ∅ ⊆ ∅
- Tühi hulk ei sisalda ühtegi elementi: ∀x (x ∉ ∅)
- Tühi hulk ei ole sama, mis {∅} (hulk, mille ainus element on tühi hulk)

**Näide:**
- ∅ on tühi hulk (ei sisalda ühtegi elementi)
- {∅} on hulk, mis sisaldab ühte elementi – tühja hulka

**NB! {∅} ≠ ∅**
- ∅ on tühi hulk, mis ei sisalda ühtegi elementi (tühi karp).
- {∅} on hulk, mis sisaldab ühte elementi - tühja hulka (karp, milles on tühi karp).

## Universaalhulk

**Definitsioon:** Universaalhulk (või universumhulk), mida tähistatakse tavaliselt tähega U, on hulk, mis sisaldab kõiki vaatluse all olevaid elemente.

Universaalhulk sõltub kontekstist ja vaadeldavast valdkonnast. See määratleb "universumi", milles kõik teised hulgad on vaadeldavad.

**Näited:**
- Geomeetria ülesandes võib universaalhulk olla kõigi vaadeldavate punktide hulk.
- Tõenäosusteooria ülesandes võib universaalhulk olla kõigi võimalike sündmuste hulk.
- Aritmeetika ülesandes võib universaalhulk olla näiteks reaalarvude hulk ℝ või täisarvude hulk ℤ.

## Osahulk

**Definitsioon:** Hulka A nimetatakse hulga B osahulgaks ehk alamhulgaks (tähistatakse A ⊆ B), kui iga hulga A element kuulub ka hulka B.

Formaalselt:
A ⊆ B parajasti siis, kui ∀x (x ∈ A ⟹ x ∈ B)

**Näide:**  
Kui A = {1, 2, 3} ja B = {1, 2, 3, 4, 5}, siis A ⊆ B, sest iga element, mis kuulub hulka A, kuulub ka hulka B.

Osahulgaks olemist võib kujutleda nii, et karbi A sisu on täielikult karbi B sees.

### Pärisosahulk

**Definitsioon:** Hulka A nimetatakse hulga B pärisosahulgaks (tähistatakse A ⊂ B), kui A on B osahulk ja A ≠ B (ehk hulgas B on vähemalt üks element, mida pole hulgas A).

**Näide:**  
Kui A = {1, 2, 3} ja B = {1, 2, 3, 4, 5}, siis A ⊂ B, sest A ⊆ B ja A ≠ B.

Seoste A ⊆ B ja A ⊂ B vahekord on analoogiline arvude vahelise mitterange ja range võrratusega.

### Osahulga omadused

1. **Refleksiivsus**: Iga hulk on iseenda osahulk: A ⊆ A.
2. **Antisümmeetrilisus**: Kui A ⊆ B ja B ⊆ A, siis A = B.
3. **Transitiivsus**: Kui A ⊆ B ja B ⊆ C, siis A ⊆ C.

Antisümmeetrilisuse omadust kasutatakse sageli just siis, kui on vaja tõestada, et kaks hulka on võrdsed. Võrduse tõestamiseks näidatakse sel juhul, et kumbki hulkadest on teise hulga osahulk. Ehk siis võrdsuse A = B tõestamiseks näidatakse, et A ⊆ B ja B ⊆ A.

### Alamhulkade arv

Kui hulgas A on n elementi, siis sellel hulgal on täpselt 2ⁿ erinevat alamhulka (sealhulgas tühi hulk ja hulk A ise).

**Näide:**  
Kui A = {1, 2, 3}, siis hulgal A on 2³ = 8 erinevat alamhulka:
∅, {1}, {2}, {3}, {1, 2}, {1, 3}, {2, 3}, {1, 2, 3}

## Hulga kõigi osahulkade hulk (astmehulk)

**Definitsioon:** 
Olgu A hulk. Hulga A kõigi osahulkade hulka nimetatakse astmehulgaks (või potentshulgaks) ja tähistatakse P(A) = {X | X ⊆ A}.

Astmehulka võib kujutleda kui suurt karpi, milles on kõik võimalikud väiksemad karbid, mida saab moodustada algse karbi elementidest.

**Näide:**
Kui A = {a, b, c}, siis P(A) = {∅, {a}, {b}, {c}, {a, b}, {a, c}, {b, c}, {a, b, c}}

**NB! Väga oluline on mõista, et kui X on hulga A alamhulk, siis X ∈ P(A).**

See tähendab, et alamhulga ja astmehulga vaheline seos on kuuluvusseos (∈), mitte alamhulga seos (⊆).

**Näiteks:**
- {a, c} ⊂ {a, b, c} (alamhulga seos originaalhulgaga)
- {a, c} ∈ P({a, b, c}) (kuuluvusseos astmehulgaga)

## Hulga võimsus (kardiaalarv)

**Definitsioon:** Hulga võimsus ehk kardiaalarv on hulga elementide arv. Hulga A võimsust tähistatakse sümboliga |A| või #(A).

**Näited:**
- Kui A = {1, 2, 3, 4, 5}, siis |A| = 5
- Kui B = ∅ (tühi hulk), siis |B| = 0
- Kui C = {a, {a}, {{a}}}, siis |C| = 3 (siin on kolm erinevat elementi: a, {a} ja {{a}})

### Lõplikud ja lõpmatud hulgad

Hulk on **lõplik**, kui selle võimsus on lõplik (saab väljendada naturaalarvuna). Vastasel juhul on hulk **lõpmatu**.

**Näited lõplikest hulkadest:**
- A = {1, 2, 3} on lõplik hulk võimsusega 3
- B = ∅ on lõplik hulk võimsusega 0

**Näited lõpmatutest hulkadest:**
- Naturaalarvude hulk ℕ = {1, 2, 3, ...}
- Reaalarvude hulk ℝ
- Ratsionaalarvude hulk ℚ

## Tähtsamad arvuhulgad

Matemaatikas on mitmeid olulisi arvuhulki, mida tähistatakse eriliste sümbolitega:

- **Naturaalarvude hulk** ℕ = {1, 2, 3, ...}
  - Mõnikord loetakse ka 0 naturaalarvuks ja siis tähistatakse hulka kui ℕ₀
  - **Selles kursusel naturaalarvud on hulk ℕ = {1, 2, 3, ...} ehk 0 ei ole naturaalarv!**

- **Täisarvude hulk** ℤ = {..., -3, -2, -1, 0, 1, 2, 3, ...}

- **Ratsionaalarvude hulk** ℚ = {p/q | p, q ∈ ℤ, q ≠ 0}
  - Ratsionaalarvud on kõik arvud, mida saab väljendada kahe täisarvu jagatisena

- **Irratsionaalarvude hulk** I = {x ∈ ℝ | x ∉ ℚ}
  - Irratsionaalarvud on reaalarvud, mida ei saa väljendada kahe täisarvu jagatisena
  - Näiteks π, e, √2 on irratsionaalarvud

- **Reaalarvude hulk** ℝ
  - Reaalarvud sisaldavad kõiki ratsionaalarve ja irratsionaalarve (nagu π, e, √2)

- **Kompleksarvude hulk** ℂ = {a + bi | a, b ∈ ℝ, i² = -1}
  - Kompleksarvud laiendavad reaalarvude hulka imaginaararvude lisamisega

Nende hulkade vahel kehtivad järgmised sisalduvussuhted:
ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ ⊂ ℂ

## Arvude intervallid

Arvuintervallid on reaalarvude hulga alamhulgad, mida saab defineerida alg- ja lõpp-punkti järgi.

- **Suletud intervall** [a,b] = {x ∈ ℝ | a ≤ x ≤ b}
  - Sisaldab nii alg- kui ka lõpp-punkti
  - Näide: [2, 5] = {x ∈ ℝ | 2 ≤ x ≤ 5}

- **Avatud intervall** (a,b) = {x ∈ ℝ | a < x < b}
  - Ei sisalda ei alg- ega lõpp-punkti
  - Näide: (2, 5) = {x ∈ ℝ | 2 < x < 5}

- **Poolavatud intervallid**
  - [a,b) = {x ∈ ℝ | a ≤ x < b} (sisaldab algpunkti, aga mitte lõpp-punkti)
  - (a,b] = {x ∈ ℝ | a < x ≤ b} (ei sisalda algpunkti, aga sisaldab lõpp-punkti)

- **Lõpmatud intervallid**
  - [a, ∞) = {x ∈ ℝ | x ≥ a} (sisaldab kõiki reaalarve alates a-st)
  - (a, ∞) = {x ∈ ℝ | x > a} (sisaldab kõiki reaalarve, mis on suuremad kui a)
  - (-∞, b] = {x ∈ ℝ | x ≤ b} (sisaldab kõiki reaalarve kuni b-ni)
  - (-∞, b) = {x ∈ ℝ | x < b} (sisaldab kõiki reaalarve, mis on väiksemad kui b)
  - (-∞, ∞) = ℝ (kõikide reaalarvude hulk)

## Hulga element ja alamhulk (oluline erinevus)

On väga oluline mõista erinevust hulga elemendi ja alamhulga vahel. See on üks sagedasemaid segaduse allikaid hulgateooria õppimisel.

- Kui x on element, siis kirjutame x ∈ A, mis näitab, et x on üks objektidest hulgas A.
- Kui X on hulk, siis kirjutame X ⊆ A, mis näitab, et X on hulga A alamhulk (kõik X-i elemendid on ka A elemendid).

Kujuta ette kooli: õpilased on elemendid ja klassid on alamhulgad. Kui Mari on õpilane, siis Mari ∈ Kool. Kui 5.A on üks klassidest, siis 5.A ⊆ Kool.

**Näide:**
Olgu A = {1, 2, 3}
- 1 ∈ A (1 on hulga A element)
- {1} ⊆ A ({1} on hulga A alamhulk)
- {1} ∉ A ({1} ei ole hulga A element, sest A elemendid on 1, 2 ja 3, mitte {1})
- 1 ≠ {1} (number 1 ja hulk {1} on täiesti erinevad objektid)

**NB! Erinevus hulga elemendi ja alamhulga vahel on üks tähtsamaid asju, mida hulgateooria õppimisel meeles pidada.**

## Hulk kui andmestruktuur

Hulgad on olulised mitte ainult teoreetilises matemaatikas, vaid ka arvutiteaduses, kus neid kasutatakse andmestruktuuridena. Erinevalt massiividest või loeteludest ei ole hulkades elementide järjekord oluline ja iga element saab esineda ainult ühe korra.

Paljudes programmeerimiskeeltes on olemas spetsiaalsed hulga andmestruktuurid:
- Python: `set`
- Java: `HashSet`, `TreeSet`
- JavaScript: `Set`
- C++: `std::set`, `std::unordered_set`

**Näide Python-is:**
```python
# Hulga loomine
A = {1, 2, 3, 4}
B = {3, 4, 5, 6}

# Elementide lisamine ja eemaldamine
A.add(5)      # A = {1, 2, 3, 4, 5}
A.remove(1)   # A = {2, 3, 4, 5}

# Alamhulga kontrollimine
is_subset = {1, 2}.issubset({1, 2, 3})  # True

# Võrdsuse kontrollimine
are_equal = {1, 2, 3} == {3, 2, 1}  # True
```

## Paradoksid hulgateooria kontekstis

Hulgateooria arengus on avastatud mitmeid paradokse, mis viitavad võimalikele probleemidele naiivsetes hulgateooria formulatsioonides.

### Russelli paradoks

Russelli paradoks (Bertrand Russell, 1901) tekib, kui vaatleme hulka R = {X | X ∉ X}, ehk kõigi selliste hulkade hulka, mis ei sisalda iseennast elemendina.

Küsimus: kas R ∈ R?
- Kui R ∈ R, siis definitsiooni järgi R ∉ R.
- Kui R ∉ R, siis definitsiooni järgi R ∈ R.

See on vastuolu, mis näitab, et naiivsetes hulgateooria raamides ei ole võimalik sellist hulka R konstrueerida.

Russelli paradoksi ja teiste sarnaste probleemide lahendamiseks arendati välja aksiomaatilised hulgateooria süsteemid, nagu Zermelo-Fraenkeli hulgateooria.

## Kokkuvõte

Hulgateooria põhimõisteid mõistes ja neid rakendades saame:
1. Formaliseerida matemaatilisi kontseptsioone täpselt ja selgelt
2. Käsitleda erinevaid matemaatilisi objekte ühtses raamistikus
3. Analüüsida objektide kogumite vahelisi seoseid

Olulisimad terminid ja kontseptsioonid hulgateooria põhimõistetes on:
- **Hulk** - objektide kogum, mida vaadeldakse ühe tervikuna
- **Element** ja **kuuluvus** (∈) - suhe elemendi ja hulga vahel
- **Alamhulk** (⊆) ja **pärisalamhulk** (⊂) - suhted hulkade vahel
- **Tühi hulk** (∅) - hulk, mis ei sisalda ühtegi elementi
- **Universaalhulk** (U) - kõiki vaadeldavaid elemente sisaldav hulk
- **Võimsus** (kardiaalarv) - hulga elementide arv
- **Astmehulk** (P(A)) - hulga kõigi alamhulkade hulk
- **Arvuhulgad** - ℕ, ℤ, ℚ, ℝ, ℂ - matemaatikas kasutatavad standardsed arvuhulgad
- **Intervallid** - [a,b], (a,b), [a,b), (a,b] - teatud tüüpi reaalarvude hulkade tähistused

Nende põhimõistete mõistmine loob aluse hulgateooria edasistele teemadele, mille hulka kuuluvad hulgatehted, hulkade visualiseerimine ja hulgateooria rakendused.