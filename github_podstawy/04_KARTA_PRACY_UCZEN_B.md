# Karta pracy ucznia B: autor forka i pull requestu

**Imię lub identyfikator:** ........................................................  
**Partner:** ........................................................  
**Klasa:** ........................  **Data:** ........................

## Cel roli

Utworzysz fork publicznego repozytorium partnera, przygotujesz w nim podstronę atrakcji i zaproponujesz jej dołączenie za pomocą pull requestu. Nie będziesz collaboratorem repozytorium źródłowego.

## Etap 1. Znajdź repozytorium partnera

1. Zaloguj się do GitHuba.
2. Otwórz adres przekazany przez partnera albo wyszukaj repozytorium.
3. Sprawdź właściciela i nazwę repozytorium.
4. Potwierdź, że repozytorium jest publiczne.

Adres repozytorium źródłowego:

```text
..............................................................................
```

## Etap 2. Utwórz fork

1. W repozytorium partnera kliknij `Fork`.
2. Jako właściciela forka wybierz swoje konto.
3. Zachowaj nazwę `przewodnik-region`.
4. Kliknij `Create fork`.
5. Po utworzeniu sprawdź informację wskazującą repozytorium źródłowe.

### Kontrola

- [ ] Fork znajduje się na moim koncie.
- [ ] Fork wskazuje repozytorium ucznia A jako źródło.
- [ ] Edytuję swój fork, a nie repozytorium partnera.

Adres forka:

```text
..............................................................................
```

## Etap 3. Utwórz `atrakcje.html`

1. Upewnij się, że jesteś w repozytorium na swoim koncie.
2. Wybierz `Add file`, a następnie `Create new file`.
3. Wpisz nazwę:

```text
atrakcje.html
```

4. Dodaj kod zgodny z wymaganiami projektu.
5. Podłącz arkusz:

```html
<link rel="stylesheet" href="atrakcje.css">
```

6. Wybierz `Commit changes`.
7. Użyj komunikatu:

```text
Dodanie podstrony z atrakcjami
```

### Kontrola HTML

- [ ] Plik nazywa się dokładnie `atrakcje.html`.
- [ ] Ustawiono język polski oraz UTF-8.
- [ ] Strona ma jeden `h1`.
- [ ] Opisano co najmniej trzy miejsca.
- [ ] Dodano listę.
- [ ] Użyto elementów semantycznych.
- [ ] Podłączono `atrakcje.css`.

## Etap 4. Utwórz `atrakcje.css`

1. Utwórz w swoim forku plik:

```text
atrakcje.css
```

2. Dodaj wymagane style.
3. Zapisz commit z komunikatem:

```text
Dodanie stylów podstrony atrakcji
```

### Kontrola CSS

- [ ] Plik nazywa się dokładnie `atrakcje.css`.
- [ ] Ostylowano `body`, nagłówek, nawigację i odnośniki.
- [ ] Zdefiniowano i użyto co najmniej jednej klasy.
- [ ] Użyto odstępów i kolorów.
- [ ] Dodano regułę `@media`.

## Etap 5. Otwórz pull request

1. Przejdź do strony głównej swojego forka.
2. Użyj `Contribute`, a następnie `Open pull request`, albo wybierz `Compare & pull request`.
3. Jeśli trzeba, wybierz `compare across forks`.
4. Sprawdź kierunek:

```text
base repository: repozytorium ucznia A
base: main
head fork: repozytorium ucznia B
compare: main lub gałąź z Twoimi zmianami
```

5. Sprawdź podgląd zmian. Powinny pojawić się tylko oczekiwane pliki i commity.
6. Wpisz tytuł:

```text
Dodanie podstrony z atrakcjami
```

7. Wpisz opis, korzystając ze wzoru:

```text
## Cel zmian
Dodałem podstronę prezentującą atrakcje regionu.

## Dodane pliki
- atrakcje.html
- atrakcje.css

## Zawartość
- opis trzech ciekawych miejsc,
- lista atrakcji,
- semantyczna struktura HTML,
- osobny arkusz CSS,
- reguła responsywna.

## Prośba do osoby przeglądającej
Proszę o sprawdzenie struktury HTML, ścieżki do CSS i czytelności strony.
```

8. Kliknij `Create pull request`.
9. Przekaż partnerowi adres pull requestu.

### Kontrola pull requestu

- [ ] Repozytorium bazowe należy do ucznia A.
- [ ] Repozytorium źródłowe jest moim forkiem.
- [ ] Pull request prowadzi do gałęzi `main` właściciela.
- [ ] Tytuł opisuje zmianę.
- [ ] Opis wymienia pliki i zakres pracy.
- [ ] Pull request nie jest szkicem, czyli `Draft`, jeśli ma być od razu scalony.

Adres pull requestu:

```text
..............................................................................
```

## Etap 6. Odpowiedz na przegląd

1. Przeczytaj komentarz partnera.
2. Jeśli trzeba, wróć do pliku w swoim forku.
3. Wprowadź poprawkę.
4. Zapisz ją jako kolejny commit, na przykład:

```text
Dodanie reguły responsywnej po przeglądzie
```

5. Wróć do pull requestu i sprawdź, czy nowy commit się pojawił.
6. Odpowiedz komentarzem, co zostało poprawione.
7. Nie twórz drugiego pull requestu do tej samej poprawki.

## Etap 7. Obserwuj scalenie

Po zatwierdzeniu przez ucznia A sprawdź, czy pull request ma status `Merged`. Następnie otwórz repozytorium źródłowe i znajdź swoje pliki.

### Podsumowanie

1. Dlaczego Twoje zmiany nie pojawiły się automatycznie w repozytorium partnera?

```text
..............................................................................
..............................................................................
```

2. Co wskazuje gałąź `base`, a co `compare`?

```text
..............................................................................
..............................................................................
```

3. Jak pull request zmienił się po dodaniu kolejnego commitu?

```text
..............................................................................
..............................................................................
```
