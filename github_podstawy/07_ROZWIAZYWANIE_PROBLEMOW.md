# Rozwiązywanie typowych problemów

## Nie widzę przycisku `Fork`

1. Sprawdź, czy jesteś zalogowany.
2. Upewnij się, że oglądasz repozytorium partnera, a nie własny fork.
3. Sprawdź, czy repozytorium jest publiczne.
4. Odśwież stronę.
5. Jeśli fork tego repozytorium już istnieje na Twoim koncie, otwórz utworzony wcześniej fork.

## Edytuję nie to repozytorium

Sprawdź nazwę właściciela wyświetlaną nad listą plików. Uczeń B powinien tworzyć pliki w repozytorium na swoim koncie. Uczeń A pracuje w repozytorium źródłowym.

## Nie widzę `Compare & pull request`

1. Otwórz własny fork.
2. Wybierz `Contribute` i `Open pull request`.
3. Alternatywnie otwórz zakładkę `Pull requests` i wybierz `New pull request`.
4. Użyj `compare across forks`, jeśli GitHub nie pokazuje właściwych repozytoriów.

## Pull request ma zły kierunek

Przed utworzeniem sprawdź:

```text
base repository = repozytorium ucznia A
base = main
head fork = fork ucznia B
compare = gałąź ze zmianami ucznia B
```

Jeśli kierunek jest odwrotny, nie scalaj zmian. Wróć do porównania i ustaw repozytoria prawidłowo.

## Pull request nie pokazuje zmian

Możliwe przyczyny:

- pliki nie zostały zapisane commitem,
- wybrano niewłaściwą gałąź `compare`,
- pull request porównuje repozytorium z nim samym,
- zmiany już wcześniej zostały scalone,
- pliki utworzono w innym repozytorium.

Sprawdź historię commitów forka i wybraną gałąź.

## Pull request pokazuje za dużo plików

Nie scalaj go automatycznie. Sprawdź, czy uczeń B wykonał zmiany wyłącznie w swoim zakresie. Niepożądane pliki należy usunąć lub przywrócić ich poprzednią zawartość w forku, a poprawkę zapisać kolejnym commitem.

## Właściciel nie może scalić pull requestu

Sprawdź:

- czy pull request nie jest szkicem `Draft`,
- czy występuje konflikt,
- czy wybrano właściwe repozytorium bazowe,
- czy zmiany nie zostały już scalone lub pull request nie został zamknięty,
- czy konto zalogowane w przeglądarce jest właścicielem repozytorium.

Jeśli wystąpi konflikt, przeczytaj komunikat GitHuba. W wersji podstawowej najlepiej zapobiegać konfliktom przez tworzenie różnych plików przez uczniów.

## Po poprawce pull request nadal wygląda tak samo

1. Sprawdź, czy poprawkę zapisano jako commit.
2. Sprawdź, czy commit znajduje się w tej samej gałęzi, z której otwarto pull request.
3. Odśwież stronę pull requestu.
4. Otwórz zakładki `Commits` i `Files changed`.

## Arkusz CSS nie działa

Sprawdź:

- nazwę pliku,
- wielkość liter,
- rozszerzenie `.css`,
- wartość atrybutu `href`,
- czy HTML i CSS znajdują się w tym samym katalogu,
- czy w CSS nie brakuje nawiasu klamrowego.

Poprawne połączenia:

```html
<link rel="stylesheet" href="style.css">
```

```html
<link rel="stylesheet" href="atrakcje.css">
```

## Link między stronami nie działa

Jeśli oba dokumenty znajdują się w tym samym katalogu, użyj:

```html
<a href="index.html">Strona główna</a>
<a href="atrakcje.html">Atrakcje</a>
```

Nie używaj ścieżki do pliku na dysku komputera, na przykład `C:\...`.

## Przypadkowo ujawniono informację poufną

Natychmiast zgłoś to nauczycielowi. Samo usunięcie pliku w kolejnym commicie może nie usunąć treści z historii repozytorium. Hasło, klucz lub token należy traktować jako ujawniony i unieważnić zgodnie z instrukcją nauczyciela lub administratora.

## Reguła bezpieczeństwa

Jeżeli nie rozumiesz skutków operacji, szczególnie usuwania repozytorium, zmiany widoczności lub scalania nieoczekiwanych plików, zatrzymaj się i poproś nauczyciela o pomoc.
