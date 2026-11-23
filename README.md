# Notatnik spotkań

Aplikacja na telefon (PWA) do transkrypcji wewnętrznych spotkań. Rozpoznaje mówców, oznacza miejsca, w których kilka osób mówi naraz, robi podsumowanie i eksportuje je do PDF.

**Adres:** https://mikislaga-a11y.github.io/notatnik-spotkan/

## Instalacja na telefonie
- **iPhone (Safari):** Udostępnij → „Do ekranu początkowego”
- **Android (Chrome):** menu ⋮ → „Zainstaluj aplikację”

Przy pierwszym uruchomieniu wklej klucz API OpenAI (https://platform.openai.com/api-keys).

## Prywatność
- To repozytorium zawiera wyłącznie kod aplikacji, bez kluczy i danych.
- Klucz API zapisuje się tylko w pamięci telefonu.
- Nagrania, transkrypcje i podsumowania istnieją tylko w pamięci otwartej aplikacji i znikają po jej zamknięciu.
- Audio jest wysyłane do OpenAI (`gpt-4o-transcribe-diarize`), które robi transkrypcję.

## Do zapamiętania
- Model `gpt-4o-transcribe-diarize` ma zapowiedziane wyłączenie na 26.02.2027. Przed tą datą trzeba zmienić stałą `TRANSCRIBE_MODEL` w `index.html`.
- Model do podsumowań zmienia się w ustawieniach aplikacji (⚙).
