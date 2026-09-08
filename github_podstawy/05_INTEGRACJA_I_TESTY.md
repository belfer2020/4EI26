# Integracja i testy końcowe

## Cel

Po scaleniu pull requestu właściciel łączy dwa niezależne zestawy plików w jedną witrynę. Partner pomaga w testowaniu i zgłasza zauważone problemy.

## 1. Sprawdź strukturę repozytorium właściciela

Po scaleniu powinny znajdować się w nim:

```text
README.md
index.html
style.css
atrakcje.html
atrakcje.css
```

Jeśli brakuje pliku, nie przechodź do integracji. Najpierw sprawdź pull request i historię commitów.

## 2. Dodaj nawigację do obu stron

W `index.html`, najlepiej wewnątrz `header`, dodaj:

```html
<nav aria-label="Główna nawigacja">
    <a href="index.html">Strona główna</a>
    <a href="atrakcje.html">Atrakcje</a>
</nav>
```

W `atrakcje.html` dodaj taką samą nawigację. Dzięki ścieżkom względnym obie strony mogą wskazywać na siebie w obrębie repozytorium.

## 3. Sprawdź arkusze CSS

W `index.html` powinno znajdować się:

```html
<link rel="stylesheet" href="style.css">
```

W `atrakcje.html` powinno znajdować się:

```html
<link rel="stylesheet" href="atrakcje.css">
```

Wielkość liter ma znaczenie. Nazwy `Atrakcje.css` i `atrakcje.css` mogą być traktowane jako różne pliki.

## 4. Zapisz integrację

Właściciel zapisuje zmiany commitem:

```text
Połączenie stron nawigacją
```

Jeśli poprawki dotyczą różnych zagadnień, można użyć kilku precyzyjnych commitów zamiast jednego ogólnego.

## 5. Wykonaj testy

### Test zawartości repozytorium

- [ ] W repozytorium właściciela są cztery pliki witryny.
- [ ] Pliki ucznia B są widoczne w historii pull requestu.
- [ ] Pull request ma status `Merged`.
- [ ] Ostatni commit właściciela opisuje integrację.

### Test HTML

- [ ] Każda strona ma `<!doctype html>`.
- [ ] Każda strona ma `lang="pl"`.
- [ ] Każda strona ma kodowanie UTF-8.
- [ ] Każda strona ma własny `title`.
- [ ] Każda strona ma dokładnie jeden `h1`.
- [ ] Znaczniki są prawidłowo zagnieżdżone i zamknięte.
- [ ] Obie strony zawierają nawigację.

### Test połączeń

- [ ] Link z `index.html` prowadzi do `atrakcje.html`.
- [ ] Link z `atrakcje.html` prowadzi do `index.html`.
- [ ] `index.html` wskazuje `style.css`.
- [ ] `atrakcje.html` wskazuje `atrakcje.css`.
- [ ] Nazwy w atrybutach `href` mają poprawną wielkość liter.

### Test jakości

- [ ] Tekst jest czytelny i napisany własnymi słowami.
- [ ] Kontrast tekstu i tła pozwala odczytać treść.
- [ ] Nawigacja jest widoczna.
- [ ] Układ nie wymaga przewijania poziomego na wąskim ekranie.
- [ ] Kod ma czytelne wcięcia.
- [ ] W repozytorium nie ma danych poufnych.

## 6. Opcjonalny podgląd

Jeżeli nauczyciel przewidział dodatkowy czas, witrynę można opublikować przez GitHub Pages zgodnie z osobną instrukcją nauczyciela. Publikacja nie jest warunkiem podstawowego zaliczenia ćwiczenia. Nawet bez GitHub Pages można ocenić strukturę plików, historię commitów, pull request i kod źródłowy.

## 7. Raport błędów

Wpisz zauważone problemy i sposób ich usunięcia:

```text
Problem 1:
..............................................................................
Rozwiązanie:
..............................................................................

Problem 2:
..............................................................................
Rozwiązanie:
..............................................................................
```
