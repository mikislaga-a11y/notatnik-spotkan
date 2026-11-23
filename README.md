# Notatnik spotkań

Aplikacja na telefon (PWA) do transkrypcji wewnętrznych spotkań. Rozpoznaje mówców, robi podsumowanie i eksportuje je do PDF.

**Adres:** https://mikislaga-a11y.github.io/notatnik-spotkan/

## Instalacja na telefonie
- **iPhone (Safari):** Udostępnij → „Do ekranu początkowego”
- **Android (Chrome):** menu ⋮ → „Zainstaluj aplikację”

## Klucze (oba darmowe, bez karty)
1. **AssemblyAI** do transkrypcji: https://www.assemblyai.com/dashboard/signup. Klucz jest w zakładce API Keys. Aplikacja używa serwerów w UE (`api.eu.assemblyai.com`).
2. **Groq** do podsumowań: https://console.groq.com/keys → Create API Key.

## Prywatność
- Repozytorium zawiera wyłącznie kod aplikacji, bez kluczy i danych.
- Klucze zapisują się tylko w pamięci telefonu.
- Transkrypcje i podsumowania są zapisane tylko na telefonie i usuwają się automatycznie po 24 h. Nagranie jest kasowane z telefonu zaraz po transkrypcji.
- AssemblyAI (serwery UE) nie używa nagrań do trenowania modeli. W panelu AssemblyAI (Settings → Data Controls) warto ustawić TTL na 1 dzień, żeby transkrypcje znikały też z ich serwerów.
- Groq nie trenuje na danych z API. W panelu Groq (Settings → Data Controls) można włączyć Zero Data Retention.
