# Karta pracy ucznia A: właściciel repozytorium

**Imię lub identyfikator:** ........................................................  
**Partner:** ........................................................  
**Klasa:** ........................  **Data:** ........................

## Cel roli

Utworzysz repozytorium źródłowe i stronę główną. Następnie przeprowadzisz przegląd pull requestu partnera, scalisz zaakceptowane zmiany i połączysz dwie strony w witrynę.

## Etap 1. Załóż publiczne repozytorium

1. Zaloguj się do GitHuba.
2. Utwórz nowe repozytorium.
3. Ustaw nazwę:

```text
przewodnik-region
```

4. Wpisz krótki opis, na przykład:

```text
Dwustronicowy przewodnik przygotowany w ramach nauki fork i pull request.
```

5. Ustaw widoczność `Public`.
6. Zaznacz inicjalizację plikiem `README.md`.
7. Kliknij `Create repository`.
8. **Nie dodawaj partnera jako collaboratora.**
9. Przekaż partnerowi adres URL repozytorium.

### Kontrola

- [ ] Repozytorium jest publiczne.
- [ ] Repozytorium zawiera `README.md`.
- [ ] Partner nie ma bezpośredniego prawa zapisu.
- [ ] Partner otrzymał poprawny adres repozytorium.

Adres repozytorium:

```text
..............................................................................
```

## Etap 2. Utwórz `index.html`

1. Otwórz repozytorium.
2. Wybierz `Add file`, a następnie `Create new file`.
3. Wpisz nazwę `index.html`.
4. Przygotuj stronę zgodnie z wymaganiami projektu.
5. Wybierz `Commit changes`.
6. Użyj komunikatu:

```text
Dodanie strony głównej przewodnika
```

7. Zapisz commit w swoim repozytorium.

### Kontrola HTML

- [ ] Ustawiono `lang="pl"` i kodowanie UTF-8.
- [ ] Strona ma unikalny `title`.
- [ ] Strona ma dokładnie jeden `h1`.
- [ ] Użyto elementów semantycznych.
- [ ] Podłączono `style.css`.
- [ ] Treść jest zgodna z tematem.

## Etap 3. Utwórz `style.css`

1. Utwórz nowy plik `style.css`.
2. Dodaj style zgodne z wymaganiami.
3. Zapisz commit z komunikatem:

```text
Dodanie stylów strony głównej
```

### Kontrola CSS

- [ ] Styl obejmuje `body`.
- [ ] Ostylowano nagłówek, nawigację i odnośniki.
- [ ] Użyto co najmniej jednej klasy.
- [ ] Ustawiono odstępy i kolory.
- [ ] Dodano regułę `@media`.

## Etap 4. Odbierz pull request

Poczekaj, aż partner prześle adres pull requestu.

1. Otwórz zakładkę `Pull requests` w swoim repozytorium.
2. Otwórz pull request partnera.
3. Sprawdź tytuł i opis.
4. Otwórz `Files changed`.
5. Potwierdź, że dodawane są pliki:

```text
atrakcje.html
atrakcje.css
```

6. Przeczytaj kod obu plików.
7. Sprawdź zgodność z wymaganiami.
8. Dodaj merytoryczny komentarz. Nie wystarczy komentarz „OK”.

Przykładowe komentarze:

```text
Proszę dodać atrybut lang="pl" w elemencie html.
```

```text
Kod jest czytelny. Podoba mi się wykorzystanie elementów article. Proszę jeszcze dodać regułę responsywną dla ekranów do 600 px.
```

### Kontrola przeglądu

- [ ] Sprawdzono dokładnie dwa oczekiwane pliki.
- [ ] Sprawdzono strukturę HTML.
- [ ] Sprawdzono połączenie HTML z CSS.
- [ ] Sprawdzono nazwy plików i ścieżki.
- [ ] Dodano merytoryczną informację zwrotną.

## Etap 5. Podejmij decyzję

Jeśli kod wymaga poprawy, poproś partnera o wykonanie poprawki w jego forku. Po dodaniu kolejnego commitu pull request powinien zaktualizować się automatycznie. Sprawdź go ponownie.

Jeżeli rozwiązanie jest gotowe:

1. kliknij `Merge pull request`,
2. sprawdź komunikat scalenia,
3. kliknij `Confirm merge`.

Nie usuwaj forka partnera. Nie jest to potrzebne do ukończenia zadania.

### Kontrola scalenia

- [ ] Pull request ma poprawny kierunek.
- [ ] Nie ma nierozwiązanych problemów.
- [ ] Zmiany zostały scalone do `main` repozytorium właściciela.
- [ ] W repozytorium widoczne są pliki partnera.

Adres pull requestu:

```text
..............................................................................
```

## Etap 6. Połącz strony

Wykonaj integrację według pliku `05_INTEGRACJA_I_TESTY.md`.

Dodaj w `index.html` nawigację do podstrony:

```html
<nav aria-label="Główna nawigacja">
    <a href="index.html">Strona główna</a>
    <a href="atrakcje.html">Atrakcje</a>
</nav>
```

Następnie edytuj `atrakcje.html` i dodaj analogiczną nawigację. Zapisz integrację sensownym commitem, na przykład:

```text
Połączenie stron nawigacją
```

## Etap 7. Podsumowanie

Odpowiedz krótko:

1. Co sprawdziłeś przed scaleniem pull requestu?

```text
..............................................................................
..............................................................................
```

2. Dlaczego partner nie został dodany jako collaborator?

```text
..............................................................................
..............................................................................
```

3. Jaka jest różnica między forkiem a repozytorium źródłowym?

```text
..............................................................................
..............................................................................
```
