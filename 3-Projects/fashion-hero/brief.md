# FashionHero - Brief projektu

> To jest Twój case'owy projekt w AI Product Heroes. Pracujesz nad nim przez całe 5 tygodni programu, równolegle z lekcjami. Fabuła rozwija się w trakcie - nowe informacje pojawiają się z każdą lekcją. Ten brief zawiera tylko to, co wiesz na START programu, po lekcji L1.1.

---

## Firma

**FashionHero** to marketplace modowy w Polsce - think Allegro Moda, tylko mniejsze i skupione wyłącznie na modzie. Platforma łączy sprzedawców (od małych butików po streetwearowych brandów indie) z kupującymi.

- Założona 2020, rośnie szybko
- 2.4 mln aktywnych kupujących, 4,200 niezależnych sprzedawców
- ~300 tys. zamówień miesięcznie, średnie zamówienie ~200 PLN, ~60 mln PLN obrotu miesięcznie
- Model: marketplace, 100% przychodu z prowizji od transakcji (standardowo 22%, negocjowane niżej dla dużych sprzedawców) - czyli ~44 PLN od przeciętnego zamówienia
- Obrót rośnie (+28% YoY), ale marża na pojedynczym zamówieniu spada
- Dwie rundy finansowania zamknięte, trzecia w planach

---

## Problem widoczny na Day 1

Dwa twarde fakty, od których wszystko się zaczyna:

### 1. Return rate = 38%

Prawie 4 na 10 zamówień wraca. Każdy zwrot to stracona prowizja - ~44 PLN (200 PLN x 22%) które nigdy nie trafiają do kasy. A do tego FashionHero dopłaca do darmowych zwrotów (~15 PLN za przesyłkę zwrotną) żeby konkurować z Zalando i Forte. Łącznie zwroty kosztują FashionHero ~6.7 mln PLN miesięcznie. Przy skali platformy to są prawdziwe pieniądze wyciekające co dzień.

Dashboard FashionHero pokazuje dane. Formularze zwrotów są analizowane. Support tickety są kategoryzowane. FashionHero MA analitykę - to nie jest firma, która leci bez danych. Mimo to problem nie został rozwiązany przez dwa lata.

### 2. Marża topnieje

Mimo że obrót rośnie, FashionHero zarabia coraz mniej na każdym zamówieniu. Inwestorzy nie patrzą na obrót - patrzą na to ile firma zarabia per transakcja. Przy obecnym trendzie za rok FashionHero nie będzie miało argumentu na kolejną rundę finansowania.

---

## Zespół

Cztery osoby, z którymi będziesz pracować. Każda ma swój głos i swoje zdanie - co nie zawsze się zgadza.

### Maja - CEO

Pragmatyczna, data-driven. Lubi hasło "pokaż mi liczby". Nie toleruje opinii bez uzasadnienia. Widzi problem zwrotów w prosty sposób: **"Zdjęcia nie oddają produktu. Zróbcie lepsze zdjęcia - profesjonalne studio, modele, oświetlenie. To rozwiąże problem."**

Jej intuicja jest oparta na wieloletnim doświadczeniu w retailu. Brzmi rozsądnie.

### Konrad - Product Manager

Twój partner w zbrodni przez najbliższe 5 tygodni.

Chętny, szybki, uczący się. Nie czeka. Gdy dostaje problem - rzuca się do analizy. Czasami jego szybkość jest jego mocą, czasem jego słabością (wyprzedza dane, wyciąga wnioski przed researchem).

Zdanie Konrada: **"Problem to rozmiarówka. Ludzie zamawiają, dostają, rozmiar nie pasuje, zwracają. 62% zwracanych zamówień ma w formularzu 'zły rozmiar' jako powód. Benchmarki z Zalando i ASOS potwierdzają - to najczęstsza przyczyna zwrotów w branży. Nawet support tickety to potwierdzają. Buduję lepszy system rozmiarów."**

Jego rozumowanie brzmi sensownie. Jest oparte na danych, benchmarkach, ticketach. Każdy rozsądny PM zrobiłby to samo.

### Ela - Data Scientist

Kobieta, która zadaje niewygodne pytania. Cicha, ale gdy się odzywa - słuchasz.

Ela ma przeczucie. **"Nie ufam formularzom zwrotów. Coś mi tu nie gra. Daj mi tydzień - chcę przekopać surowe dane, nie tylko agregaty, które wyciąga Konrad. Mam hipotezę, ale bez danych jej nie pokażę."**

Konrad nie ma tygodnia. Ma AI i działa szybko. Ela wraca do swojego laptopa i zaczyna kopać.

### Ola - Growth Marketing

Skupiona na kliencie. Ciągle rozmawia z użytkownikami, prowadzi wywiady, czyta recenzje. Zna jej czytelników głębiej niż ktokolwiek w firmie.

### Tomek - Customer Support

Widzi wzorce z pierwszej linii. Gdy coś jest nie tak z produktem, Tomek wie pierwszy - bo tickety mu mówią. Powtarza od miesięcy: **"To nie jest błąd. To jest zachowanie. Ludzie tak zamawiają - na zapas, żeby zwrócić. To część modelu, nie defekt."**

Nikt go do końca nie słucha. Ma swoją teorię, która brzmi zbyt prosto.

---

## Twoja rola: Stream A + Stream B

Program ma dwa równoległe strumienie pracy. Pracujesz na obu jednocześnie.

### Stream A - Koszty (Konrad prowadzi, Ty obserwujesz)

W klasie, podczas każdej lekcji, obserwujesz jak Konrad radzi sobie z problemem zwrotów. Konrad buduje, testuje, uczy się, adaptuje. Ty widzisz jego ścieżkę z boku - jako sparing partner, osoba zadająca pytania, obserwator uczący się na jego sukcesach i pomyłkach.

Stream A to ten, w którym narracja się rozwija. Niektóre rzeczy które wygląda na prawdziwe teraz - nie są. Niektóre rozwiązania, które brzmią sensownie - nie działają. To jest nauka przez obserwację.

### Stream B - Przychody (Ty prowadzisz)

Równolegle, TY pracujesz na drugiej stronie problemu: **marża topnieje**. Konrad bierze koszty (zwroty). Ty bierzesz **przychody**.

FashionHero ma 100% przychodu z prowizji. Zero dywersyfikacji. Czy to jedyny sposób, żeby zarabiać na marketplace modowym? Co mógłby zrobić FashionHero, żeby marża przestała topnieć - bez kanibalizacji istniejącego biznesu?

To jest Twoje pole. Tu wypracowujesz hipotezy, robisz wywiady (syntetyczne i prawdziwe, w zależności od zasobów), budujesz prototypy, testujesz, decydujesz. Nie masz gotowej odpowiedzi. Musisz ją znaleźć.

---

## Co się dzieje po L1.1

Lekcja 1.1 pokazuje Ci FashionHero. Poznajesz ekipę, widzisz problem, rozumiesz kontekst. Konrad w klasie pokazuje, jak **uruchomił Claude'a i w ciągu kilku minut wygenerował 12 hipotez** o przyczynach wysokich zwrotów. Po analizie wybrał jedną: rozmiarówkę. W czwartek zacznie budować.

**Twoje zadanie (homework):**

1. Skonfiguruj swój vault (uruchom skill `second-brain-setup` z folderu `7-Skills/`)
2. Napisz własne 12+ hipotez - ale NIE o zwrotach (to Konrada teren). O **przychodach**. Co FashionHero mógłby zrobić, żeby marża przestała topnieć z innej strony niż koszty zwrotów?
3. Wybierz 3 najciekawsze
4. Dla każdej zapisz predykcję: *"Główna przyczyna to ____ bo ____"*
5. Zapisz swoje hipotezy w `3-Projects/fashion-hero/discovery/pierwsze-hipotezy.md`

---

## Przydatne pliki

- `brief.md` (ten plik) - podstawowy kontekst
- `margin-brief.md` - jednostronicowy briefing od Mai z liczbami i trzema głosami o przychodach
- `discovery/` - tu idą Twoje wywiady, hipotezy, dane, research
- `decisions/` - tu idą OSTy, RICE, PRD, strategiczne wybory
- `prototypes/` - tu linki do Lovable, zrzuty, specs
- `analyses/` - tu wyniki A/B, analizy, learningi
- `artifacts/` - tu to, co oddajesz na certyfikacji (końcowy prototyp, video pitch)

## Twój pierwszy prompt do AI po konfiguracji vaulta

```
Przeczytaj 3-Projects/fashion-hero/brief.md. Oto mój kontekst jako Product Buildera
na start programu AI Product Heroes. Moje zadanie na pierwszy tydzień: wygenerować
12+ hipotez o tym, jak FashionHero mógłby zwiększyć przychody (NIE o zwrotach -
to teren Konrada, ja pracuję nad stroną przychodową). Pomóż mi przejść ten proces.
Zacznij od zadania mi jednego konkretnego pytania, które uruchomi moje myślenie.
```
