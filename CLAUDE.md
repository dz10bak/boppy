# Boppy

Free AI Music Generator — landing page for boppy.me.

## Struktura projektu

- `index.html` — cała strona w jednym pliku (HTML + CSS + JS inline)

## Sekcje strony

1. **Nav** — logo, linki nawigacyjne (How it works, Features, Voice Clone, FAQ), CTA button, mobile hamburger
2. **Hero** — główny nagłówek z animowanym gradientem, floating music notes, dwa CTA buttony
3. **How it works** — 3 kroki (Describe → AI Lyrics → Generate & Share) z connectorami
4. **Features** — 6 kart (Free, No Signup, Every Genre, Up to 5 min, Share, Open Source)
5. **Community/Showcase** — 3 przykładowe tracki z waveform playerami
6. **Voice Clone (Coming Soon)** — zapowiedź funkcji klonowania głosu, animacja orb + wave, formularz waitlist
7. **Create (Generator)** — fake generator UI (textarea, mode/duration selector, fake generating flow z wynikiem)
8. **FAQ** — 7 pytań w accordionie + schema.org JSON-LD
9. **Footer** — logo, copyright, linki (Privacy, Terms, GitHub)

## Konwencje

- Projekt to single-file HTML — cały CSS i JS trzymamy inline w `index.html`
- Ciemny morski motyw (--surface: #0c1b24, --surface-light: #142935)
- Kolory: primary #ff8e48 (pomarańcz), accent #72dce5 (turkus), highlight #ff5948 (czerwony)
- Font: Inter (Google Fonts)
- Animacje: wyłącznie CSS (bez zewnętrznych bibliotek), scroll reveal przez IntersectionObserver
- Design: minimalistyczny, responsywny (3 breakpointy: 1024px, 768px, 480px)
- SEO: meta tags, OG tags, Twitter cards, schema.org FAQ
- Generator jest fake — symuluje generowanie z losowym wynikiem z predefiniowanych piosenek
