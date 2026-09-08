# Teoria: fork, commit i pull request

## 1. Repozytorium

Repozytorium to miejsce przechowywania plików projektu i historii ich zmian. W tym ćwiczeniu repozytorium znajduje się na GitHubie i jest obsługiwane w przeglądarce.

Repozytorium **publiczne** może być dostępne dla wszystkich użytkowników Internetu. Nie umieszczaj w nim danych osobowych, haseł, kluczy dostępu ani innych informacji poufnych.

## 2. Właściciel i zewnętrzny współpracownik

Właściciel kontroluje swoje repozytorium. Może między innymi dodawać pliki, scalać pull requesty i zarządzać ustawieniami.

Zewnętrzny współpracownik w tym ćwiczeniu nie otrzymuje prawa zapisu do repozytorium właściciela. Tworzy własną kopię repozytorium, czyli fork, i za jej pomocą proponuje zmiany.

## 3. Fork

Fork to osobne repozytorium utworzone na podstawie innego repozytorium. Ma własnego właściciela, pliki, commity i gałęzie, ale GitHub zachowuje informację o związku z repozytorium źródłowym, nazywanym także `upstream`.

```text
repozytorium źródłowe ucznia A
              ↓ fork
repozytorium ucznia B
```

Zmiany wykonane w forku nie zmieniają automatycznie repozytorium źródłowego.

## 4. Commit

Commit jest zapisanym punktem w historii projektu. Powinien zawierać krótki i konkretny komunikat opisujący zmianę.

Dobre komunikaty:

```text
Dodanie strony głównej przewodnika
Dodanie podstrony z atrakcjami
Uzupełnienie nawigacji między stronami
Poprawa ścieżki do arkusza CSS
```

Słabe komunikaty:

```text
zmiany
plik
gotowe
asdf
```

## 5. Gałąź

Gałąź, czyli branch, jest niezależną linią pracy w repozytorium. Główna gałąź projektu najczęściej nazywa się `main`.

W podstawowej wersji ćwiczenia uczniowie mogą zapisywać zmiany na `main` we własnych repozytoriach. Jeżeli GitHub proponuje utworzenie nowej gałęzi podczas zapisu pliku, można ją utworzyć, ale trzeba później wskazać ją jako gałąź źródłową pull requestu.

## 6. Pull request

Pull request, w skrócie PR, to propozycja scalenia zmian. Nie jest jeszcze scaleniem. Pozwala właścicielowi:

- przeczytać opis zmian,
- obejrzeć listę commitów,
- sprawdzić różnice w zakładce `Files changed`,
- zadać pytanie lub dodać komentarz,
- poprosić o poprawkę,
- zaakceptować i scalić zmiany,
- zamknąć propozycję bez scalania.

W tym ćwiczeniu kierunek pull requestu powinien wyglądać tak:

```text
base repository: repozytorium ucznia A
base branch: main

head fork: fork ucznia B
compare branch: main lub gałąź ucznia B
```

Najczęstszy błąd to odwrócenie tego kierunku.

## 7. Przegląd kodu

Przegląd kodu nie polega wyłącznie na kliknięciu przycisku `Merge`. Właściciel powinien sprawdzić:

- czy dodano wyłącznie oczekiwane pliki,
- czy HTML ma poprawną strukturę,
- czy arkusz CSS jest prawidłowo podłączony,
- czy treści są zgodne z tematem,
- czy nazwy plików i ścieżki są poprawne,
- czy kod nie zawiera danych poufnych,
- czy pull request ma zrozumiały tytuł i opis.

## 8. Merge

Merge oznacza scalenie zaakceptowanych zmian z gałęzi źródłowej do bazowej. W tym ćwiczeniu właściciel używa standardowej opcji `Merge pull request`, a następnie potwierdza operację.

Po scaleniu pliki ucznia B powinny znaleźć się w repozytorium ucznia A.

## 9. Schemat pracy

```text
Uczeń A tworzy publiczne repozytorium
                 ↓
Uczeń B tworzy fork
                 ↓
A tworzy index.html i style.css
B tworzy atrakcje.html i atrakcje.css
                 ↓
Uczeń B otwiera pull request
                 ↓
Uczeń A sprawdza zmiany i przekazuje informację zwrotną
                 ↓
Uczeń B w razie potrzeby poprawia pliki w swoim forku
                 ↓
Pull request aktualizuje się o nowe commity
                 ↓
Uczeń A scala zmiany
                 ↓
Uczeń A dodaje nawigację i testuje całą witrynę
```

## 10. Pytania kontrolne

1. Dlaczego uczeń B może zmieniać pliki w swoim forku, ale nie w repozytorium ucznia A?
2. Czym różni się commit od pull requestu?
3. Co oznaczają `base` i `compare` podczas tworzenia pull requestu?
4. Dlaczego należy obejrzeć `Files changed` przed scaleniem?
5. Co stanie się z pull requestem, gdy uczeń B doda kolejny commit do tej samej gałęzi?
6. Dlaczego publiczne repozytorium nie jest miejscem na hasła i dane poufne?

## Źródła do dalszej nauki

- GitHub Docs, Fork a repository: https://docs.github.com/en/pull-requests/how-tos/work-with-forks/fork-a-repo
- GitHub Docs, Editing files: https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files
- GitHub Docs, Creating a pull request from a fork: https://docs.github.com/en/pull-requests/how-tos/create-pull-requests/creating-a-pull-request-from-a-fork
- GitHub Docs, Merging a pull request: https://docs.github.com/en/pull-requests/how-tos/merge-and-close-pull-requests/merging-a-pull-request
