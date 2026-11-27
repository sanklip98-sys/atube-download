# atube

ATube dla Windows — wyszukiwanie, odtwarzanie i pobieranie filmów YouTube,
obsługa klawiaturą i czytnikiem ekranu oraz opcjonalna audiodeskrypcja AI.

## Pobieranie

[Pobierz instalator ATube 1.4.31 dla Windows](https://github.com/sanklip98-sys/atube-download/releases/download/v1.4.31/atube-Setup.exe)

[Najnowsze wydanie](https://github.com/sanklip98-sys/atube-download/releases/latest)

Wersja: **1.4.31**. Instalator: `atube-Setup.exe`, 161210877 bajtów.

SHA-256 instalatora:

`1DA737E5B59B28D116B57834E82515D2B49F7BEFE0C69168BA722DE3A74EA157`

## Zmiany w 1.4.31

- W `F4 → Dźwięk` dodano opcjonalne **Wzmocnienie głośności do 400%**.
  Jest domyślnie wyłączone, więc po aktualizacji zakres pozostaje 0–100%.
  Po świadomym włączeniu działa ze strzałkami, menu, własnymi skrótami i
  przełącznikami; powyżej 100% czytnik otrzymuje komunikat „Wzmocnienie
  aktywne”. Wyłączenie opcji od razu ogranicza poziom do 100%.
- Wzmocnienie działa tylko wewnątrz odtwarzania VLC w ATube. Nie zmienia
  głośności systemu, miksera, urządzenia ani NVDA. Poziomy powyżej 100% mogą
  być bardzo głośne, zniekształcić dźwięk oraz uszkodzić słuch lub sprzęt.
  Zacznij od niskiego poziomu i zwiększaj go stopniowo.
- Z wersji 1.4.30 uwzględniono poprawkę oznajmiania liczby zwykłych wyników
  wyszukiwania przed autoodtwarzaniem. Zaktualizowano także przypięty
  `yt-dlp` do 2026.11.23 oraz zależności budowania.
- Gotowy instalator przeszedł 34/34 zwykłe zestawy testów, 10/10 po
  obfuskacji i 11/11 na dokładnym EXE z instalatora. Sprawdzono czystą
  instalację, aktualizację z 1.4.30, podpis manifestu i rzeczywiste pobranie
  MP4 z obrazem i dźwiękiem. Nie wykonywano głośnego odsłuchu ani odsłuchu
  tej wersji z NVDA.

## Ważniejsze wcześniejsze zmiany

- Dodano sterowanie jednym lub dwoma przełącznikami klawiaturowymi.
  Zakładka `F4 → Przełączniki` udostępnia profile urządzeń, rozpoznawanie
  klawiszy, regulowane skanowanie i panel obsługi programu. Funkcja jest
  domyślnie wyłączona; `Ctrl+Shift+F12` otwiera panel.
- Audiodeskrypcja może korzystać z własnego serwera zgodnego z OpenAI.
  Obsługiwane są Chat Completions i Responses, osobny klucz chroniony DPAPI
  oraz test połączenia i rozpoznawania obrazu. Model musi obsługiwać obrazy.
- Dodano własne skróty klawiaturowe i opcjonalny układ jednej ręki,
  numerowanie 89 opcji w 15 zakładkach, kontrast, powiększenie i dodatkowe
  poprawki fokusu oraz komunikatów czytnika ekranu.
- Instalator przeszedł czystą instalację przenośną i aktualizację z 1.4.28.
  Testy fizycznych przełączników, rzeczywistego własnego serwera AI i odsłuch
  tej wersji z NVDA pozostają do wykonania przez użytkownika.

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
