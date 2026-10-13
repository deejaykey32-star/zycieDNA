# Laboratorium Życia

Edukacyjno-logiczna gra o DNA: od nukleotydu, przez replikację, transkrypcję i translację, bioinformatykę (mutacja w genie HBB) i biotechnologię (EcoRI, plazmid, CRISPR-Cas9) do żywej komórki i organizmu. Przewodniczką jest dr Ada Helisa z animowanym avatarem i nagranym głosem lektorki.

## Struktura
- `index.html` – cała gra (HTML, CSS, JS w jednym pliku, bez zależności)
- `audio/` – 110 nagrań kwestii lektorki (MP3), nazwy to hash FNV-1a czytanego tekstu
- `_headers`, `wrangler.toml` – konfiguracja Cloudflare Pages

## Live / Wdrożenie
Aplikacja jest dostępna pod adresem: **[https://zycie.pages.dev](https://zycie.pages.dev)**

## Uruchomienie lokalne
```bash
npx wrangler pages dev .
```

## Wdrożenie w Cloudflare Pages
```bash
npx wrangler pages deploy . --project-name zycie
```
Albo podłącz repozytorium GitHub `zycieDNA` w panelu Cloudflare Pages (bez polecenia budowania, katalog wyjściowy `/`).

Nagrania wygenerowano otwartym modelem VITS `mai_female` (Coqui TTS, CC BY 4.0 dla danych M-AILABS) w tempie 1,1×.
