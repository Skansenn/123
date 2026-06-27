# Skład Budowlany Kowalczyk — strona / apka webowa

Gotowa, samodzielna strona (jeden plik `index.html`) skierowana do **klientów indywidualnych**.
Motyw kolorystyczny: **niebieski + biały + czarny** (pod logo i stronę sklad-budowlany.pl).

## Jak uruchomić
Otwórz `index.html` w przeglądarce — nic nie trzeba instalować.
Aby opublikować: wgraj plik na dowolny hosting (np. przez FTP) albo darmowy serwis typu
GitHub Pages / Netlify. To zwykła strona statyczna.

## Co zawiera
- Sekcja hero z hasłem i **kalkulatorem materiału** (kostka, klej, pustaki, płytki)
- Kafelki oferty (kategorie produktów)
- Sekcja promocji dla klienta indywidualnego
- „Dlaczego my”, „Jak kupić w 3 krokach”, opinie klientów
- Formularz zapytania / wyceny (wersja demo — patrz niżej)
- Pływające przyciski: telefon + WhatsApp
- W pełni responsywna (telefon, tablet, komputer)

## Jak edytować treści (bez programowania)
Większość treści jest w **jednym miejscu** — w pliku `index.html` znajdź sekcję:

```html
<script id="site-data" type="application/json">
```

To zwykły **JSON**. Zmieniaj tylko tekst w cudzysłowach: kategorie, promocje, opinie itd.

### Dane do podmiany (placeholdery)
W kodzie wpisane są placeholdery w nawiasach `[...]` oraz numer `+48 000 000 000`.
Podmień je na prawdziwe:
- **telefon** — szukaj `+48000000000` (linki `tel:` i WhatsApp `wa.me/48...`) oraz `[+48 000 000 000]`
- **adres** — `[ulica i numer, ...]`
- **e-mail** — `kontakt@sklad-budowlany.pl`
- **godziny otwarcia** — `Pn–Pt 7:00–17:00 · Sob 8:00–14:00`

### Formularz kontaktowy
Obecnie formularz działa w trybie demo (pokazuje potwierdzenie, nie wysyła maila).
Aby odbierać zgłoszenia, podłącz go np. do Formspree / własnego skryptu PHP
albo poproś o dodanie wysyłki na e-mail.

### Logo
Logo to prosty znak „K” w niebieskim kwadracie + napis. Jeśli masz plik logo
(PNG/SVG), można je podmienić w sekcji `.logo` — chętnie pomogę.
