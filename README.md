# ZIP to Audio

ZIP to Audio to program dla Windows, który przepakowuje archiwum RAR do ZIP
przygotowanego do odtwarzaczy książek audio.

To publiczne repozytorium zawiera dokumentację użytkownika i publiczne pliki
potrzebne do aktualizacji programu. Kod źródłowy nie jest tutaj publikowany.

## Pobieranie

Najnowszy instalator:

<https://github.com/sanklip98-sys/zip-to-audio/releases/latest/download/ZipToAudio-Setup.exe>

## Najważniejsze funkcje

1. Czyta wskazane archiwum RAR bez instalowania 7-Zip.
2. Może dodać do ZIP-a tylko pliki MP3.
3. Może nadać plikom kolejne numery, np. `1.mp3`, `2.mp3`, `10.mp3` zmieni na `01.mp3`, `02.mp3`, `03.mp3`.
4. Zapisuje ZIP w kolejności numerowanych nazw.
5. Może automatycznie wypakować utworzony ZIP do wybranego folderu.
6. Po wypakowaniu usuwa z tej operacji pliki inne niż MP3.
7. Może ponumerować istniejący ZIP bez wypakowywania go do folderu.
8. Pokazuje status, pasek postępu i prędkość pracy.

Oryginalny plik RAR nie jest modyfikowany.

## Podstawowe użycie

1. Uruchom `ZipToAudio.exe`.
2. Wybierz plik RAR.
3. Sprawdź lub zmień miejsce zapisu ZIP.
4. Sprawdź folder wypakowania. Domyślnie program proponuje `Dokumenty\Z t a konwersje\nazwa-archiwum`.
5. Zostaw zaznaczone opcje, jeśli chcesz typową konwersję audiobooka:
   - `Wypakuj ZIP po konwersji`
   - `Do ZIP-a dodawaj tylko pliki MP3`
   - `Nadaj kolejne numery plikom`
6. Naciśnij `Konwertuj`.

## Opcje dodatkowe

Menu `Opcje dodatkowe` otworzysz klawiaturą przez `Alt+O`.

Dostępne opcje:

- `Konwertuj RAR na ZIP` - przepakowuje całe archiwum RAR do ZIP bez filtrowania MP3 i bez zmiany nazw.
- `Konwertuj ZIP na RAR` - przepakowuje ZIP do RAR. Ta opcja wymaga programu `Rar.exe` albo `WinRAR.exe`.
- `Dodaj numerację do ZIP` - tworzy w folderze konwersji programu nowy ZIP z samymi plikami audio i numeracją `01`, `02`, `03` itd.; od `10` program nie dodaje zera z przodu.

## Sterowanie klawiaturą

- `Alt+O` otwiera menu `Opcje dodatkowe`.
- `Alt+N` od razu uruchamia opcję `Dodaj numerację do ZIP`.
- `F1` pokazuje pomoc z opisem działania klawiszy.
- `Enter` zatwierdza wybraną opcję w menu i dialogach.
- `Escape` lub zamknięcie okna pyta, czy zamknąć program.
- W pytaniu o zamknięcie wybór `Tak`/`Nie` zmienia się strzałkami lewo/prawo.

## Aktualizacje

Program sprawdza, czy jest dostępna nowsza wersja.
Jeśli aktualizacja istnieje, pojawi się okno dialogowe z przyciskami:

- `Aktualizuj teraz`
- `Odłóż na później`

`Enter` zatwierdza aktualnie wybraną opcję.

## Logi

Program zapisuje log działania w katalogu:

```text
%LOCALAPPDATA%\ZipToAudio\Logs
```

Log pomaga sprawdzić, co program robił i jaki błąd wystąpił.

## Wymagania

- Windows.
- Do podstawowej konwersji RAR na ZIP nie trzeba instalować 7-Zip.
- Do podstawowej konwersji nie trzeba instalować dodatkowych bibliotek.
- Tylko opcja dodatkowa ZIP na RAR wymaga programu `Rar.exe` albo `WinRAR.exe`, ponieważ format RAR nie jest zapisywany przez 7-Zip ani SharpCompress.

## Licencje

Do obsługi archiwów program używa biblioteki SharpCompress zaszytej w pliku EXE.
Informacje o licencjach bibliotek są dołączone do paczki programu.
