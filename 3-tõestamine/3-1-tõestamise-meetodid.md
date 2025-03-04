# Tõestamise meetodid

Tõestamine on matemaatika südameks - see on protsess, mille käigus näitame, et mingi väide on tõene, kasutades loogilisi argumente ja tuginedes varem tõestatud tulemustele, definitsioonidele või aksioomidele. Tõestamise oskus ei ole kasulik mitte ainult matemaatikas, vaid ka igapäevaelus, õpetades meid loogiliselt mõtlema ja oma argumente selgelt väljendama.

Selles peatükis tutvustame peamisi tõestamismeetodeid:

## 1. Otsene tõestus

Otsene tõestus on kõige tavalisem tõestamismeetod, kus alustame eeldusest ja loogilise arutelu kaudu jõuame järelduseni. Enamik tõestusi, millega sa siiamaani kokku oled puutunud, on olnud otsesed tõestused.

### Näide 1.1: Paarisarvude summa

**Väide:** Kui m ja n on paarisarvud, siis m + n on samuti paarisarv.

**Tõestus:** Olgu m ja n paarisarvud. Paarisarvude definitsiooni kohaselt saame kirjutada m = 2k₁ ja n = 2k₂, kus k₁ ja k₂ on mingid täisarvud. Nüüd,

m + n = 2k₁ + 2k₂ = 2(k₁ + k₂)

Kuna k₁ + k₂ on täisarv, siis 2(k₁ + k₂) on paarisarv. Seega m + n on paarisarv.

## 2. Tõestus alamjuhtude põhjal

Mõnikord on kasulik jagada tõestus erinevateks alamjuhtudeks ja tõestada väide eraldi iga alamjuhu jaoks.

### Näide 2.1: Naturaalarvude ruudud ja paaritute arvude summa

**Väide:** Iga naturaalarvu n korral on n³ + n paarisarv.

**Tõestus:** Jaotame naturaalarvude hulga kaheks alamjuhuks: paarisarvud ja paaritud arvud.

**Juht 1:** Olgu n paarisarv, n = 2k, kus k on naturaalarv.
Siis n³ + n = (2k)³ + 2k = 8k³ + 2k = 2(4k³ + k).
Kuna 4k³ + k on täisarv, siis 2(4k³ + k) on paarisarv.

**Juht 2:** Olgu n paaritu arv, n = 2k + 1, kus k on naturaalarv.
Siis n³ + n = (2k+1)³ + (2k+1) = 8k³ + 12k² + 6k + 1 + 2k + 1
= 8k³ + 12k² + 8k + 2 = 2(4k³ + 6k² + 4k + 1).
Kuna 4k³ + 6k² + 4k + 1 on täisarv, siis 2(4k³ + 6k² + 4k + 1) on paarisarv.

Seega mõlemal juhul on n³ + n paarisarv, mis tõestab väite.

## 3. Kontrapositiivne tõestus

Kontrapositiivne tõestus põhineb faktil, et väide "Kui P, siis Q" on samaväärne väitega "Kui mitte Q, siis mitte P". Mõnikord on lihtsam tõestada kontrapositiivset väidet.

### Näide 3.1: Ruutjuur 2 irratsionaalsus

**Väide:** Kui n² on paaritu, siis n on paaritu.

Esmalt märgime, et seda on raske otse tõestada, alustades eeldusest "n² on paaritu". Selle asemel tõestame kontrapositiivse väite: "Kui n on paarisarv, siis n² on paarisarv".

**Kontrapositiivne tõestus:** Olgu n paarisarv, siis n = 2k mingi täisarvu k korral. Nüüd,
n² = (2k)² = 4k² = 2(2k²)
Kuna 2k² on täisarv, siis n² on paarisarv.

Seega, kontrapositiivse loogikareegli põhjal, kui n² on paaritu, siis n on paaritu.

## 4. Vastuväiteline tõestus

Vastuväiteline tõestus (absurdsusele taandamine) on tõestusmeetod, kus eeldame, et tõestatav väide ei kehti, ja näitame, et see eeldus viib vastuoluni.

### Näide 4.1: √2 on irratsionaalarv

**Väide:** √2 on irratsionaalarv.

**Tõestus:** Oletame vastuväiteliselt, et √2 on ratsionaalarv. Siis saame kirjutada √2 = a/b, kus a ja b on täisarvud, b ≠ 0, ja a/b on taandumatu murd (ehk arvudel a ja b pole ühiseid tegureid peale 1).

Ruutu võttes saame:
2 = a²/b²
Seega a² = 2b²

See tähendab, et a² on paarisarv, mis omakorda tähendab, et a on paarisarv (kasutades kontrapositiivset teadmist). Seega saame kirjutada a = 2k mõne täisarvu k jaoks.

Asendades:
a² = 2b²
(2k)² = 2b²
4k² = 2b²
2k² = b²

Nüüd näeme, et b² on paarisarv, mis tähendab, et b on paarisarv. Nii a kui ka b on paarisarvud, mis on vastuolus meie eeldusega, et a/b on taandumatu murd.

See vastuolu näitab, et meie algne eeldus oli vale, seega √2 on irratsionaalarv.

## 5. Ekvivalentsi tõestamine

Ekvivalentsi tõestamisel näitame, et kaks väidet A ja B on samaväärsed, tõestades mõlema suuna implikatsiooni: A ⇒ B ja B ⇒ A.

### Näide 5.1: Paarisarvude iseloomustus

**Väide:** Täisarv n on paarisarv parajasti siis, kui n² on paarisarv.

**Tõestus:** 
1) A ⇒ B: Kui n on paarisarv, siis n² on paarisarv.
   Olgu n = 2k mingi täisarvu k korral. Siis n² = (2k)² = 4k² = 2(2k²), mis on paarisarv.

2) B ⇒ A: Kui n² on paarisarv, siis n on paarisarv.
   Tõestame seda vastuväiteliselt. Oletame, et n ei ole paarisarv, st n on paaritu. Siis n = 2k + 1 mingi täisarvu k korral.
   Seega n² = (2k + 1)² = 4k² + 4k + 1 = 2(2k² + 2k) + 1, mis on paaritu arv.
   See on vastuolus eeldusega, et n² on paarisarv.

Kuna mõlemad implikatsioonid on tõesed, siis väited "n on paarisarv" ja "n² on paarisarv" on samaväärsed.

## 6. Olemasolu tõestus

Olemasolu tõestused näitavad, et leidub vähemalt üks objekt, mis rahuldab teatud tingimust.

### Näide 6.1: Irratsionaalarvude astendamine

**Väide:** Leiduvad irratsionaalarvud a ja b nii, et a^b on ratsionaalarv.

**Tõestus:** Vaatleme arvu (√2)^(√2). Kui see on ratsionaalarv, siis võtame a = b = √2 ja oleme näidanud, et väide kehtib.

Kui (√2)^(√2) on irratsionaalarv, siis vaatleme arvu ((√2)^(√2))^(√2) = (√2)^(√2·√2) = (√2)^2 = 2, mis on ratsionaalarv. Sel juhul võtame a = (√2)^(√2) (mis on meie eelduse kohaselt irratsionaalarv) ja b = √2, ning oleme näidanud, et a^b on ratsionaalarv.

Nii või teisiti, leiduvad irratsionaalarvud a ja b, nii et a^b on ratsionaalarv.

## Kokkuvõte

Oleme tutvunud viie peamise tõestamismeetodiga:
- Otsene tõestus
- Tõestus alamjuhtude põhjal
- Kontrapositiivne tõestus
- Vastuväiteline tõestus
- Ekvivalentsi tõestamine
- Olemasolu tõestus

Igal meetodil on oma tugevused ja kasutusvaldkonnad. Oskus valida sobiv tõestusmeetod on oluline osa matemaatilisest mõtlemisest ja probleemide lahendamisest. Piisava harjutamise järel hakkad tunnetama, milline meetod millise probleemi jaoks kõige paremini sobib.

Matemaatika õppimisel on oluline mitte ainult teada, et teatud väited on tõesed, vaid ka mõista, *miks* need on tõesed. Tõestused annavad meile sügavama arusaama matemaatilistest kontseptsioonidest ja aitavad meil näha seoseid erinevate ideede vahel.