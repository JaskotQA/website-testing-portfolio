# Testy – Inwood.pl

## 📅 Data testów
27.04–03.05.2025

## 👤 Tester
Jakub Jaskot

## 🧪 Zakres testów

Testy zostały przeprowadzone dla strony **https://inwood.pl** i obejmowały:

- ✅ Sanity check (2 etapy)
- ✅ Testy funkcjonalności i UX
- ✅ Testy techniczno-SEO
- ✅ Testy bezpieczeństwa (nagłówki, CMS, brute-force)
- ✅ Testy wydajności (PageSpeed + JMeter)

## 🛠 Użyte narzędzia

- Screaming Frog SEO Spider
- OWASP ZAP
- Apache JMeter
- Google PageSpeed Insights
- Qualys SSL Labs, SecurityHeaders, UpGuard
- Ręczne testy eksploracyjne

## 📄 Raporty (PDF)

| Nr | Nazwa pliku | Zakres |
|----|-------------|--------|
| 1 | Test wstępny – etap 1 | Sanity check, działanie strony, błędy UX |
| 2 | Test wstępny – etap 2 | Formularze, responsywność, kontrast, menu |
| 3 | Kompleksowy raport bezpieczeństwa i wydajności | SSL, DNS, nagłówki, CMS, PageSpeed |
| 4 | Kompleksowy raport techniczno-SEO | SEO crawl, H1/H2, meta, błędy 404/500, obrazy |
| 5 | Bezpieczeństwo i nagłówki | Braki HSTS, CSP, X-Frame, nosniff, CORS |
| 6 | Testy logowania i ochrona brute-force | OWASP ZAP Fuzzer, odporność logowania |
| 7 | Podsumowanie testu wydajnościowego | Apache JMeter – testy pod obciążeniem |

## 🐞 Najważniejsze problemy

### 🔐 Bezpieczeństwo:
- Brak nagłówków: HSTS, CSP, X-Content-Type-Options, X-Frame-Options
- Brak DNS CAA i DNSSEC
- Przestarzałe wtyczki WordPress (Elementor Pro, Contact Form 7)
- Brak polityk DMARC i słabe szyfry

### 📊 Wydajność:
- Mobile PageSpeed = 71 (FCP: 3.3s, LCP: 5.3s)
- Czas odpowiedzi w JMeter: średnio 8.5s (max: 13.3s)
- Obrazy nie w WebP/AVIF, brak lazy loadingu, render-blocking JS/CSS

### 🧩 SEO:
- Duplikaty tytułów i meta opisów
- Brak H1 i ALT dla obrazów
- Błędy 404, długie adresy URL, brak danych strukturalnych

### ⚙ UX & funkcjonalność:
- Menu „Inwood Shutters” nie rozwija się poprawnie
- Brak walidacji pól w konfiguratorze
- Link telefoniczny otwiera pustą stronę (about:blank)
- Niski kontrast tekstu w sekcji „Pytania”
- Hamburger menu znika na iPhone 12

## ✅ Rekomendacje
- Wdrożenie pełnego zestawu nagłówków bezpieczeństwa
- Poprawa wydajności mobilnej (lazy-load, cache, optymalizacja zasobów)
- Poprawki SEO i danych strukturalnych
- Usprawnienia UX: formularze, menu, kontrast
- Retest po optymalizacji (JMeter + PageSpeed)

---

📎 Wszystkie raporty znajdują się w folderze `raporty/`
