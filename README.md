# atube

ATube dla Windows — wyszukiwanie, odtwarzanie i pobieranie filmów YouTube,
obsługa klawiaturą i czytnikiem ekranu oraz opcjonalna audiodeskrypcja AI.

## Pobieranie

[Pobierz instalator ATube 1.4.21 dla Windows](https://github.com/sanklip98-sys/atube-download/releases/download/v1.4.21/atube-Setup.exe)

[Najnowsze wydanie](https://github.com/sanklip98-sys/atube-download/releases/latest)

Wersja: **1.4.21**. Instalator: `atube-Setup.exe`, 161065770 bajtów.

SHA-256 instalatora:

`9EBE658F388E2B66CB4B7D3B21243BCF0FE1CC101B79057BC0DAE1B7736C3E16`

## Zmiany od publicznej wersji 1.4.16

- Po zamknięciu menu podczas odtwarzania fokus wraca do wcześniej aktywnej
  listy lub odtwarzacza. Escape i Alt w menu nie zatrzymują filmu. Poprawka
  obejmuje też powrót po zapisaniu i anulowaniu ustawień.
- `Ctrl+I` otwiera opis filmu. Program uzupełnia tytuł, kanał i opis również
  dla filmu otwartego z linku. Można włączyć ogłaszanie kanału po tytule.
- Nieudany zapis ustawień zachowuje poprzedni plik i zgłasza błąd przez
  mechanizm ogłoszeń czytnika ekranu. Poprawiono kończenie procesów
  pomocniczych po przekroczeniu czasu i przywracanie plików po błędzie instalacji.
- Wzmocniono ochronę kluczy API oraz maskowanie danych w logach i błędach.
  Importowane cookies są przechowywane w zaszyfrowanej postaci dla bieżącego
  konta Windows. Oryginalny eksport wskazany przez użytkownika pozostaje na dysku.
- Program sprawdza zatwierdzoną sumę yt-dlp przed uruchomieniem. Wersja
  2026.10.26 jest dołączona do instalatora; kolejne wersje pomocnika będą
  dostarczane z aktualizacjami ATube.
- Od wersji 1.4.21 aktualizator sprawdza podpis manifestu ATube oraz sumę
  instalatora. Przekierowania pobierania wymagają HTTPS.

## Instalacja i dokumentacja

Uruchom instalator, aby zainstalować program lub zaktualizować wcześniejszą
wersję. Do działania yt-dlp potrzebny jest Node.js lub Deno. VLC jest dołączony.
Instrukcję i pozostałe dokumenty Word znajdziesz po instalacji w folderze
`Dokumentacja` obok programu. Pomoc klawiaturowa jest dostępna przez `F1`,
a ustawienia przez `F4`.

Instalator i program nie mają jeszcze podpisu wydawcy Authenticode.
Podpis manifestu aktualizacji jest odrębnym zabezpieczeniem. Windows może
wyświetlić informację o nieznanym wydawcy.

Przeszły testy automatyczne aplikacji, zabezpieczeń, instalacji, aktualizacji,
fokusu oraz rzeczywistego pobrania MP4 z obrazem i dźwiękiem. Nie wykonywano
nowych płatnych żądań AI ani pełnego odsłuchu tej wersji z NVDA/JAWS.

## Zasady publikacji

Repozytorium zawiera tylko `README.md` i `latest.json`. Do wydania dołączany
jest instalator. Kod źródłowy, testy, skrypty budowania i dane użytkownika
pozostają poza tym repozytorium. Instalator zawiera potrzebne biblioteki,
zasoby, licencje i dokumentację.

Archiwa „Source code” tworzone automatycznie przez GitHub zawierają wyłącznie
publiczne pliki informacyjne i manifest. Pliki wykonywalne nadal mogą być
analizowane; podpisy i obfuskacja nie gwarantują niemożności dekompilacji.
