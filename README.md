# SQL Playground

## Jak otworzyć to repozytorium w GitHub Codespaces

1. Zaloguj się na swoje konto GitHub.
2. Przejdź do tego repozytorium na GitHub.
3. Kliknij przycisk **Code**.
4. Wybierz zakładkę **Codespaces**.
5. Kliknij **Create codespace on main**.
6. Poczekaj, aż środowisko się uruchomi – możesz już pracować w chmurze!

## Praca z bazami danych SQLite

### Używanie sqlite3 w terminalu

**Aby otworzyć bazę danych w terminalu:**

1. Otwórz terminal w VS Code (Terminal → New Terminal)
2. Wpisz komendę: `sqlite3 races.db`
3. Teraz możesz wykonywać zapytania SQL bezpośrednio w terminalu

**Podstawowe komendy w terminalu sqlite3:**

- `.help` - wyświetla listę dostępnych komend
- `.tables` - wyświetla listę tabel w bazie danych
- `.schema nazwa_tabeli` - wyświetla strukturę konkretnej tabeli
- `.quit` - wychodzi z sqlite3

**Przykład użycia w terminalu:**

```sql
sqlite3 races.db
.tables
SELECT * FROM students;
.quit
```

### Używanie rozszerzenia SQLite w VS Code

**Aby korzystać z rozszerzenia SQLite:**

1. Naciśnij **Ctrl+Shift+P** (lub **Cmd+Shift+P** na Mac)
2. Wpisz `SQLite` i wybierz odpowiednią komendę:
   - `SQLite: Open Database` - otwiera bazę danych
   - `SQLite: New Query` - tworzy nowy plik z zapytaniem SQL
   - `SQLite: Run Query` - wykonuje zapytanie SQL

**Aby otworzyć bazę danych races.db:**

1. Naciśnij **Ctrl+Shift+P**
2. Wpisz `SQLite: Open Database`
3. Wybierz plik `races.db`
4. Baza pojawi się w panelu bocznym SQLITE EXPLORER

**Aby wykonać zapytanie SQL:**

1. Utwórz nowy plik z rozszerzeniem `.sql`
2. Napisz swoje zapytanie SQL
3. Naciśnij **Ctrl+Shift+P**
4. Wpisz `SQLite: Run Query`
5. Wybierz bazę danych do wykonania zapytania

## Pisanie własnego kodu SQL

**Aby napisać własne zapytania SQL:**

- Utwórz nowy plik z rozszerzeniem `.sql` w folderze głównym repozytorium
- Możesz tworzyć podfoldery, aby lepiej organizować swoje zapytania
- Używaj rozszerzenia SQLite lub terminala do wykonywania zapytań

**Aby utworzyć nową bazę danych:**

- W terminalu wpisz: `sqlite3 nazwa_bazy.db`
- Automatycznie zostanie utworzona nowa baza danych

> **Uwaga:** Plików konfiguracyjnych (np. `.gitignore`, `.devcontainer`, `.vscode/settings.json`) nie należy edytować

## Jak zapisać plik na lokalnym urządzeniu?

1. Otwórz plik, który chcesz zapisać, w edytorze w Codespaces.
2. Kliknij prawym przyciskiem myszy na plik w panelu bocznym i wybierz **Download**.
3. Plik zostanie pobrany na Twoje lokalne urządzenie.

## Przydatne zapytania SQL

**Podstawowe operacje:**

```sql
-- Wyświetlenie wszystkich rekordów z tabeli
SELECT * FROM nazwa_tabeli;

-- Dodanie nowego rekordu
INSERT INTO nazwa_tabeli (kolumna1, kolumna2) VALUES ('wartość1', 'wartość2');

-- Aktualizacja rekordu
UPDATE nazwa_tabeli SET kolumna1 = 'nowa_wartość' WHERE warunek;

-- Usunięcie rekordu
DELETE FROM nazwa_tabeli WHERE warunek;
```
