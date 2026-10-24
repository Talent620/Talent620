<p align="center">
  <img src="https://raw.githubusercontent.com/Talent620/Talent620/main/assets/portfolio-banner.svg" alt="Artur Józefczak — aplikacje AI, automatyzacja, desktop i web" width="100%" />
</p>

<p align="center">
  <a href="#wybrane-projekty">Wybrane projekty</a> ·
  <a href="#warsztat-techniczny">Technologie</a> ·
  <a href="https://github.com/Talent620/Talent620/blob/main/README.en.md">English</a>
</p>

# Cześć, jestem Artur

Rozwijam aplikacje, które łączą AI z codzienną pracą: obsługą dokumentów, komunikacją i przygotowaniem zdjęć produktowych. Interesuje mnie cały przepływ — od interfejsu i integracji usług po testy oraz dostarczenie programu użytkownikowi.

**Trzy projekty, od których warto zacząć:**

| Projekt | Problem i rozwiązanie | Zobacz |
| :--- | :--- | :--- |
| **JARVIS** | Asystent głosowy i tekstowy łączący różnych dostawców AI, narzędzia i funkcje produktywności. | [Kod](https://github.com/Talent620/Jarvis) · [Opis techniczny](https://github.com/Talent620/Talent620/blob/main/projects/jarvis.md) |
| **IMPULS · MARTA** | Praca z dokumentami i przygotowanie dokumentacji dotacyjnej z przeglądem propozycji przez człowieka. | [Projekt i wydania](https://github.com/Talent620/IMPULS_MARTA_INSTALLER) · [Opis](https://github.com/Talent620/Talent620/blob/main/projects/marta.md) |
| **Sterownik Studio** | Obróbka zdjęć produktowych z AI, porównaniem z oryginałem i kontrolą wyniku przed eksportem. | [Wydanie Windows](https://github.com/Talent620/Sterownik-Studio/releases/tag/v1.9.4) · [Opis](https://github.com/Talent620/Talent620/blob/main/projects/sterownik-studio.md) |

## Wybrane projekty

### 01 / JARVIS — AI w jednym interfejsie

Aplikacja łącząca rozmowę tekstową i głosową, pamięć kontekstu oraz wykonywanie narzędzi. W repozytorium znajdują się klient React/TypeScript, integracje dostawców AI, backend Cloudflare Worker i konfiguracje aplikacji desktopowej oraz mobilnej.

- **Wyzwanie:** połączyć wielu dostawców i narzędzia w spójny przepływ rozmowy.
- **W kodzie:** adaptery dostawców, obsługa błędów i przełączania, uprawnienia do akcji oraz rozróżnienie symulacji od potwierdzonego wykonania.
- **Do oceny:** [testy zachowania akcji](https://github.com/Talent620/Jarvis/blob/main/tests/actionOutcome.test.ts), [automatyczne testy i build](https://github.com/Talent620/Jarvis/blob/main/.github/workflows/test.yml), [architektura](https://github.com/Talent620/Jarvis/blob/main/ARCHITECTURE.md).

**React · TypeScript · Vite · Electron · Capacitor · Cloudflare Workers · Vitest**

### 02 / IMPULS · MARTA — od dokumentów do materiału do przeglądu

Aplikacja do odczytu materiałów i wspomagania przygotowania dokumentacji dotacyjnej. Łączy pracę na źródłach, propozycje uzupełnień i kontrolę człowieka przed wykorzystaniem wyników.

- **Wyzwanie:** zachować związek propozycji z dokumentami i jasno pokazać braki.
- **Przepływ:** materiały → odczyt → propozycje → wspólny przegląd → pliki do kontroli.
- **Do oceny:** [wydanie testowe RC8, instrukcja i raport](https://github.com/Talent620/IMPULS_MARTA_INSTALLER/releases/tag/test-v5.0.0-rc.8).

**Wersja testowa.** Opublikowany raport rozdziela testy kontrolowane od niepotwierdzonego pełnego przebiegu LIVE AI. Program nie podpisuje ani nie wysyła wniosków. Publiczne repozytorium służy dystrybucji; kod źródłowy jest utrzymywany oddzielnie.

### 03 / Sterownik Studio — zdjęcia produktowe pod kontrolą

Aplikacja Windows do obróbki zdjęć z użyciem AI. Użytkownik dodaje materiał, otrzymuje wynik i porównuje go ze źródłem; niepewna kontrola blokuje automatyczny eksport.

- **Wyzwanie:** poprawić prezentację zdjęcia, zachowując numery, etykiety i widoczne cechy produktu.
- **Przepływ:** dodanie zdjęć → obróbka → kontrola → porównanie → eksport zaakceptowanych wyników.
- **Do oceny:** [instalator, instrukcja i sumy kontrolne 1.9.4](https://github.com/Talent620/Sterownik-Studio/releases/tag/v1.9.4).

**Windows x64 · przetwarzanie obrazów · integracje AI · kontrola jakości**

## Warsztat techniczny

Technologie obecne w prezentowanych projektach:

| Obszar | Narzędzia i zagadnienia |
| :--- | :--- |
| Interfejsy | React, TypeScript, Vite, Tailwind CSS |
| Desktop i mobile | Electron, Capacitor, pakowanie aplikacji Windows i Linux |
| Integracje | API dostawców AI, Cloudflare Workers, narzędzia agentowe, głos |
| Weryfikacja | Vitest, GitHub Actions, kontrola typów, automatyczny build, skan sekretów |

## Podejście do pracy

W rozwoju projektów korzystam z narzędzi AI do programowania. Portfolio pokazuje zakres aplikacji i udostępnia materiały pozwalające ocenić implementację: kod, testy, instrukcje oraz status wydań.

Przy pracy nad integracjami zwracam uwagę na obsługę błędów, kontrolę użytkownika i czytelne rozróżnienie wyniku testowego od potwierdzonego działania. Poszczególne projekty mają różny stopień dojrzałości; szczegóły są opisane przy wydaniach.

**Najlepszy punkt do rozmowy technicznej:** [JARVIS — kod, testy i mapa projektu](https://github.com/Talent620/Talent620/blob/main/projects/jarvis.md).
