# Sterownik Studio / zdjęcia produktowe

[← Portfolio](../README.md) · [Publiczny projekt](https://github.com/Talent620/Sterownik-Studio)

## Problem

Obróbka zdjęcia produktowego powinna poprawiać prezentację bez zmiany tożsamości i widocznych cech produktu. Szczególnie ważne są numery, naklejki, kody, złącza, piny i rzeczywiste uszkodzenia.

## Rozwiązanie

Aplikacja Windows łączy dodawanie zdjęć, retusz z AI, kontrolę wyniku i porównanie ze źródłem. Zgodnie z instrukcją wydania 1.9.4 niepewny wynik kontroli blokuje automatyczny eksport.

```text
Zdjęcie źródłowe → obróbka AI → kontrola wyniku
                                     ↓
                    porównanie z oryginałem → eksport
```

**Istotna decyzja produktowa:** wygenerowanie zdjęcia i dopuszczenie go do eksportu to osobne kroki.

## Co można zobaczyć

[Wydanie Windows 1.9.4](https://github.com/Talent620/Sterownik-Studio/releases/tag/v1.9.4) udostępnia:

- instalator Windows x64;
- instrukcję instalacji, konfiguracji i sprawdzenia programu;
- sumy SHA-256 oraz opis zakresu weryfikacji wydania.

Publiczne repozytorium udostępnia wydania i dokumentację. Kod źródłowy jest utrzymywany oddzielnie.

## Zakres weryfikacji

Opis wydania 1.9.4 odnotowuje kontrolę budowania, instalacji i uruchamiania na Windows CI. Logowanie na rzeczywistym koncie i płatne generowanie obrazu wymagają konfiguracji użytkownika. Testy z atrapami integracji nie potwierdzają jakości płatnego retuszu.

Wydanie nie ma podpisu Authenticode. Suma kontrolna służy porównaniu pobranego pliku z opublikowanym artefaktem; nie zastępuje podpisu wydawcy.

## Tematy do rozmowy

Zachowanie cech produktu przy edycji obrazu, niezależna kontrola wyniku, obsługa niepewności, porównanie przed/po i pakowanie aplikacji dla użytkownika bez środowiska programistycznego.
