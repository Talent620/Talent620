# JARVIS / asystent AI

[← Portfolio](../README.md) · [Kod źródłowy](https://github.com/Talent620/Jarvis)

## Problem

Rozmowa z AI, pamięć kontekstu i wykonywanie zadań często są rozdzielone między różne narzędzia. JARVIS łączy je w jednym interfejsie głosowym i tekstowym, z możliwością korzystania z różnych dostawców modeli.

## Zakres projektu

- Interfejs React/TypeScript oraz konfiguracje Electron i Capacitor.
- Adaptery dostawców AI, obsługa przełączania i błędów połączenia.
- Narzędzia agentowe i kontrola uprawnień do akcji.
- Funkcje pamięci, głosu i produktywności.
- Backend Cloudflare Worker oraz testy i konfiguracje GitHub Actions.

## Mapa do przeglądu technicznego

| Obszar | Kod lub dokumentacja | Co warto sprawdzić |
| :--- | :--- | :--- |
| Orkiestracja | [brain.ts](https://github.com/Talent620/Jarvis/blob/main/src/lib/brain.ts) | Łączenie kontekstu, wybór dostawcy i obsługa awarii |
| Dostawcy AI | [providers/](https://github.com/Talent620/Jarvis/tree/main/src/lib/providers) | Oddzielenie integracji od interfejsu aplikacji |
| Narzędzia | [tools.ts](https://github.com/Talent620/Jarvis/blob/main/src/lib/tools.ts) | Definicje i wykonywanie akcji |
| Testowanie zachowania | [actionOutcome.test.ts](https://github.com/Talent620/Jarvis/blob/main/tests/actionOutcome.test.ts) | Symulacja, próba i potwierdzone wykonanie |
| Automatyczna weryfikacja | [test.yml](https://github.com/Talent620/Jarvis/blob/main/.github/workflows/test.yml) | Instalacja zależności, skan sekretów, testy, typy i build |
| Architektura | [ARCHITECTURE.md](https://github.com/Talent620/Jarvis/blob/main/ARCHITECTURE.md) | Przepływy i opis długu technicznego; dokument może odstawać od bieżącego kodu |

## Uruchomienie do przeglądu

Wymagane są Node.js i npm zgodne z konfiguracją projektu. CI testów korzysta z Node.js 20.

```bash
git clone https://github.com/Talent620/Jarvis.git
cd Jarvis
npm ci
npm run dev
```

Interfejs uruchamia Vite; adres zostanie podany w terminalu. Funkcje AI wymagają własnej konfiguracji dostawcy lub backendu. Dane dostępowe należy przechowywać poza repozytorium.

Komendy do samodzielnej weryfikacji:

```bash
npm test
npm run build
npm run scan:secrets
```

Są to instrukcje przeglądu, a nie deklaracja wykonania nowych testów przy publikacji portfolio. Historię uruchomień można sprawdzić w [GitHub Actions](https://github.com/Talent620/Jarvis/actions).

## Status i tematy do rozmowy

Repozytorium jest projektem rozwijanym iteracyjnie. Dokument [SECURITY.md](https://github.com/Talent620/Jarvis/blob/main/SECURITY.md) opisuje historyczne problemy i działania po stronie infrastruktury; ich zamknięcia nie należy zakładać na podstawie samej obecności dokumentu.

Tematy do rozmowy technicznej: obsługa awarii dostawców, uprawnienia do narzędzi, testowanie potwierdzeń akcji oraz dalszy podział rozbudowanych modułów. To pozwala ocenić zarówno zakres aplikacji, jak i decyzje dotyczące jej utrzymania.
