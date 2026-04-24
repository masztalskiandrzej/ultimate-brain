# Drugi Mózg - Narrated Explainer (do użycia w klasie)

> Skrypt narracji dla instruktora. Użyj podczas lekcji, mając vault otwarty w Obsidian na współdzielonym ekranie. Czas: ~15-20 minut.

---

## BLOK 1: Koncept (3-4 min)

**[Ekran: otwarty vault w Obsidian, widok drzewa folderów po lewej]**

Widzicie te 8 folderów? To jest Wasz drugi mózg. Nie kurs. Nie materiały do pobrania. Narzędzie, które zabieracie ze sobą po Demo Day - do pracy, do następnego projektu, do nowej firmy za pół roku.

Idea pochodzi od Andreja Karpathy'ego - byłego szefa AI w Tesli. Jego metoda: wrzucasz surowe materiały do jednego folderu, AI je czyta i kompiluje do wiki - jednej strony na koncept, z linkami między nimi, cytatami ze źródeł. Po 20-30 źródłach masz prawdziwą bazę wiedzy, która odpowiada na pytania szybciej i mądrzej niż gdybyś szukał po osobnych plikach.

My wzięliśmy tę metodę i zaadaptowaliśmy ją dla product builderów. Dodaliśmy projekty, szablony, skille i profil osobisty - żeby AI wiedziało nie tylko CO wiesz, ale JAK z Tobą pracować.

---

## BLOK 2: Struktura (4-5 min)

**[Ekran: klikaj po folderach w miarę omawiania]**

Osiem folderów, w logicznej kolejności:

**[Kliknij 1-Daily]**
**Daily** - notatki dzienne. Jak w Obsidian, jak w jakimkolwiek systemie notatek. Używacie jak chcecie.

**[Kliknij 2-Inbox]**
**Inbox** - tu lądują nowe rzeczy. Artykuł z webu? Inbox. Transkrypt lekcji? Inbox. PDF z konferencji? Inbox. Jeśli zainstalujecie Obsidian Web Clipper - klipy z przeglądarki lądują automatycznie tutaj.

**[Kliknij 3-Projects]**
**Projects** - tu faktycznie pracujecie. FashionHero jest już tu przygotowany - z briefem, z folderami na discovery, decyzje, prototypy. Jeśli macie własny projekt, założycie tu drugi folder.

**[Kliknij 4-Knowledge]**
**Knowledge** - to jest serce metody Karpathy'ego. **Tego folderu nie wypełniacie sami - robi to AI.** Wrzucacie coś do Inbox, mówicie AI "przetwórz to", i AI tworzy tu stronę wiki. Jedna strona na koncept, nie jedno źródło. Po 5 tygodniach macie tu swoją skompilowaną wiedzę produktową z linkami i cytatami.

**[Kliknij 5-Raw]**
**Raw** - archiwum przetworzonych źródeł. Gdy AI przetworzy plik z Inbox, przenosi go tutaj. Inbox pusty = nic nowego do przetworzenia. Proste.

**[Kliknij 6-Templates]**
**Templates** - szablony dokumentów. PRD, OST, RICE, roadmapa. Na start puste - będą rosły z każdą lekcją.

**[Kliknij 7-Skills]**
**Skills** - ustrukturyzowane rozmowy, które AI prowadzi krok po kroku. Na start jest jeden: `second-brain-setup`. Kolejne dojdą w trakcie programu.

**[Kliknij 8-System]**
**System** - dwa pliki. `brain.md` - instrukcje dla AI, jak operować tym vaultem. Nie ruszacie, chyba że wiecie co robicie. `about.md` - Wasz profil osobisty. Kim jesteście, jak z Wami pracować, co jest Waszym celem. Wypełniacie go raz, AI potem honoruje to w każdej odpowiedzi.

---

## BLOK 3: Jak to działa - trzy operacje (4-5 min)

**[Ekran: otwórz brain.md, przewiń do sekcji Workflowy]**

Cały vault opiera się na trzech operacjach. Nie ma magicznych komend - mówicie AI po ludzku.

### Operacja 1: Ingest

Dodajecie plik do Inbox. Mówicie AI: "przetwórz to" albo "zrób ingest". AI czyta plik, tworzy lub aktualizuje stronę w Knowledge, przenosi plik do Raw. Inbox pusty = wszystko przetworzone.

**[Jeśli czas: pokaż live - wrzuć plik do Inbox, powiedz AI "przetwórz to", pokaż jak powstaje strona w Knowledge]**

### Operacja 2: Query

Zadajecie pytanie. "Co wiem o discovery?" "Jakie mam dane o zwrotach w e-commerce?" AI czyta Knowledge, odpowiada z cytatami. Nie szuka po surowych plikach - czyta skompilowaną wiki.

### Operacja 3: Work

Pracujecie w projekcie. "Pomóż mi z OSTem dla FashionHero." AI czyta brief projektu, korzysta z Knowledge i Templates, pisze output do folderu projektu.

To wszystko. Trzy operacje. Ingest, Query, Work.

---

## BLOK 4: Profil osobisty (2-3 min)

**[Ekran: otwórz about.md]**

Ten plik mówi AI kim jesteście. Trzy sekcje:

- **Context** - rola, firma, produkt, użytkownicy
- **How to work with me** - jak AI ma się z Wami komunikować, gdzie Was popychać
- **Current goal** - Wasz cel na 6 miesięcy

Macie dwie drogi do wypełnienia:

**Droga szybka:** Jeśli macie wyniki Gallup CliftonStrengths, DISC, MBTI, 16Personalities - wklejcie je do rozmowy z AI. AI wyciągnie z nich to, co faktycznie zmienia sposób współpracy - nie przepisuje raportu, wyciąga 5-8 konkretnych bullet pointów typu "wypychaj mnie poza strefę komfortu gdy dryfuję" albo "framuj rekomendacje przez dane, nie story".

**Droga pełna:** AI przeprowadzi z Wami krótki wywiad - 5-7 minut. Pytania o kontekst, styl komunikacji (multiple choice), obszary rozwoju, cel.

Skill `second-brain-setup` obsługuje oba warianty. Uruchomicie go po lekcji.

---

## BLOK 5: Co robicie po lekcji (2-3 min)

**[Ekran: wróć do widoku drzewa folderów]**

Trzy rzeczy do zrobienia do następnej lekcji:

1. **Pobierzcie vault** - link na Circle. Rozpakujcie w dowolnym miejscu. Otwórzcie w Obsidian.

2. **Podłączcie AI** - instrukcja w PDF, który dostaniecie. Trzy ścieżki:
   - Claude Code albo Cowork (jeśli macie Claude Pro)
   - Open Code z darmowym modelem albo GPT (jeśli nie chcecie płacić za Claude)
   - Cursor, Windsurf, Antigravity (jeśli już macie IDE z AI)
   Wszystkie działają na tym samym folderze.

3. **Uruchomcie skill `second-brain-setup`** - wypełni Wasz profil. Od tego momentu AI zna Was i wie jak z Wami pracować.

Po tych trzech krokach - otwórzcie `3-Projects/fashion-hero/brief.md`. Na dole jest gotowy prompt na start. Użyjcie go.

**[Ekran: otwórz brief.md, przewiń do sekcji z promptem]**

Ten prompt mówi AI: "przeczytaj brief, pomóż mi wygenerować 12 hipotez o przychodach FashionHero." To jest Wasze pierwsze zadanie - Stream B, strona przychodowa. Konrad bierze koszty, Wy bierzecie przychody.

---

## BLOK 6: Dlaczego to działa (1 min, opcjonalny)

Za 5 tygodni ten vault będzie miał:
- Waszą skompilowaną wiedzę z 10 lekcji
- Szablony dokumentów, których faktycznie użyliście
- Skille, które prowadzą Was przez konkretne procesy
- Pełen projekt FashionHero - od hipotez po prototyp
- Opcjonalnie - Wasz własny projekt

To nie jest folder z materiałami kursowymi. To jest narzędzie, które rośnie z Wami. Po Demo Day zabieracie je do pracy i używacie dalej.

Zaczynamy.
