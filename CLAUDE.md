# Boppy

Free AI Music Generator — landing page and subpages for boppy.me.

## Struktura projektu

Projekt to multi-page static site — każda strona to osobny plik HTML z inline CSS i JS (zero zależności).

- `index.html` — strona główna (landing page)
- `generate.html` — pełna strona generatora muzyki (fake UI)
- `share.html` — strona udostępniania/odtwarzania tracka
- `privacy.html` — polityka prywatności
- `terms.html` — warunki użytkowania

## Sekcje strony głównej (index.html)

1. **Nav** — logo, linki (How it works, Features, Community, Voice Clone, FAQ), CTA → generate.html, mobile hamburger
2. **Hero** — nagłówek z animowanym gradientem, floating music notes, CTA → generate.html
3. **How it works** — 3 kroki (Describe → AI Lyrics → Generate & Share)
4. **Features** — 6 kart (Free, No Signup, Every Genre, Up to 5 min, Share, Open Source)
5. **Community/Showcase** — 3 przykładowe tracki z waveform playerami
6. **Stats** — 4 liczniki z animacją (50K+ tracks, 12K+ creators, 30+ genres, 100% free)
7. **Testimonials** — 3 opinie użytkowników
8. **Voice Clone (Coming Soon)** — zapowiedź voice cloning, animacja orb + wave, formularz waitlist
9. **FAQ** — 7 pytań w accordionie + schema.org JSON-LD
10. **CTA Bottom** — final call to action → generate.html
11. **Footer** — logo, copyright, linki do privacy.html, terms.html, GitHub

## Podstrony

### generate.html
- Pełny UI generatora: prompt textarea, "Boost with AI", mode selector (Turbo/Base), duration selector
- Krok lyrics: edytowalny textarea z AI-generated lyrics + music description
- Fake generowanie z progress stepsami i spinnerem
- Wynik: tytuł, genre badge, waveform player, lyrics, share button
- 5 presetów piosenek losowo wybieranych

### share.html
- Strona odtwarzania tracka "Starlight Serenade"
- Duży player z waveformem, play/pause, progress bar, timer
- Pełne lyrics z oznaczeniami [Verse], [Chorus], [Bridge]
- Copy Link + Remix this track buttons
- CTA "Want to create your own?"

### privacy.html & terms.html
- Spójny design z resztą serwisu
- Treść prawna (GDPR, cookies, data handling)
- Effective Date: March 7, 2026

## Design system

- **Motyw**: ciemny morski (ocean dark)
- **Tło**: `#0a1620` (body), `#0c1b24` (surface), `#142935` (surface-light), `#1e3a4a` (surface-lighter)
- **Primary**: `#ff8e48` (pomarańcz) — CTA, akcenty, gradienty
- **Accent**: `#72dce5` (turkus/cyan) — podświetlenia, linki, Voice Clone sekcja
- **Highlight**: `#ff5948` (czerwony) — wyróżnienia
- **Muted**: `#64748b`, `#94a3b8` — tekst drugorzędny
- **Font**: Inter (Google Fonts), wagi: 300–900
- **Border radius**: 12px (karty), 16px (większe), 50px (buttony/badge)

## Konwencje

- Każda strona to standalone HTML — inline CSS + JS, zero frameworków
- Animacje: wyłącznie CSS (gradientShift, pulse, wave, float, spin) + JS scroll reveal (IntersectionObserver)
- Responsywność: 3 breakpointy (1024px, 768px, 480px)
- SEO: meta tags, OG tags, Twitter cards, schema.org FAQ (na index.html)
- Nawigacja: wspólny nav i footer na wszystkich stronach, linki między stronami
- Generator i player są fake — symulują działanie z predefiniowanymi danymi
