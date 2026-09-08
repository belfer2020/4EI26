# Wymagania projektu

## Temat witryny

**Przewodnik po ciekawych miejscach w regionie**

Para wybiera miejscowość lub region. Treści powinny być krótkie, napisane własnymi słowami i bez danych osobowych. Zdjęcia są opcjonalne. Jeżeli uczniowie używają materiałów zewnętrznych, muszą sprawdzić prawo do ich wykorzystania i podać źródło.

## Podział treści

### Strona główna ucznia A

Pliki:

```text
index.html
style.css
```

Strona powinna zawierać:

- tytuł przewodnika,
- krótkie wprowadzenie do miejscowości lub regionu,
- sekcję „Dlaczego warto odwiedzić?”,
- co najmniej trzy krótkie informacje,
- stopkę z oznaczeniem klasy lub zespołu, bez pełnych danych osobowych,
- po integracji link do `atrakcje.html`.

### Podstrona ucznia B

Pliki:

```text
atrakcje.html
atrakcje.css
```

Strona powinna zawierać:

- nagłówek „Atrakcje”,
- opis co najmniej trzech ciekawych miejsc,
- listę uporządkowaną lub nieuporządkowaną,
- jedną sekcję wyróżnioną klasą CSS,
- stopkę,
- po integracji link powrotny do `index.html`.

## Wspólne wymagania HTML

Każdy dokument HTML powinien:

- używać deklaracji `<!doctype html>`,
- mieć ustawiony język polski,
- zawierać elementy `html`, `head` i `body`,
- zawierać kodowanie UTF-8,
- mieć unikalny i sensowny tytuł w elemencie `title`,
- korzystać z semantycznych elementów, na przykład `header`, `nav`, `main`, `section`, `article`, `footer`,
- mieć dokładnie jeden nagłówek `h1`,
- mieć prawidłowo zamknięte znaczniki,
- podłączać właściwy arkusz CSS przez element `link`.

Przykładowy szkielet:

```html
<!doctype html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tytuł strony</title>
    <link rel="stylesheet" href="nazwa-pliku.css">
</head>
<body>
    <header>
        <h1>Tytuł strony</h1>
    </header>

    <main>
        <section>
            <h2>Nagłówek sekcji</h2>
            <p>Treść napisana własnymi słowami.</p>
        </section>
    </main>

    <footer>
        <p>Projekt edukacyjny</p>
    </footer>
</body>
</html>
```

## Wspólne wymagania CSS

Każdy arkusz CSS powinien zawierać co najmniej:

- styl dla `body`,
- styl nagłówka lub elementu `header`,
- styl nawigacji i odnośników,
- klasę używaną w HTML,
- ustawienia odstępów, na przykład `margin` i `padding`,
- co najmniej jeden kolor tła i jeden kolor tekstu,
- prostą regułę responsywną `@media`.

Przykład reguły responsywnej:

```css
@media (max-width: 600px) {
    main {
        padding: 1rem;
    }

    nav a {
        display: block;
        margin: 0.5rem 0;
    }
}
```

## Wymagania dotyczące GitHuba

Para musi udokumentować:

- publiczne repozytorium ucznia A,
- fork na koncie ucznia B,
- co najmniej jeden sensowny commit każdego ucznia,
- pull request od ucznia B do ucznia A,
- komentarz właściciela odnoszący się do kodu lub jakości rozwiązania,
- ewentualną poprawkę ucznia B jako kolejny commit,
- scalenie pull requestu,
- końcową zawartość repozytorium ucznia A.

## Ograniczenia

- Nie dodawaj ucznia B jako collaboratora.
- Nie przesyłaj plików przez komunikator lub pocztę.
- Nie kopiuj kodu partnera ręcznie do repozytorium właściciela.
- Nie używaj terminala ani GitHub Desktop.
- Nie umieszczaj danych poufnych ani pełnych danych osobowych.
- Nie zmieniaj ustalonych nazw czterech głównych plików.

## Warunek ukończenia

Projekt jest ukończony, gdy repozytorium ucznia A zawiera cztery działające pliki witryny, historia potwierdza pracę obu uczniów, pull request został scalony, a nawigacja pozwala przechodzić między obiema stronami.
