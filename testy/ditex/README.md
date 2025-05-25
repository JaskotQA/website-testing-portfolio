# Raport testów – Ditex.com.pl

## 📍 Strona testowana
**https://ditex.com.pl**

## 📅 Okres analizy
Kwiecień 2025

## 👤 Tester
Jakub Jaskot

---

## 📦 Zakres i struktura dokumentacji

W ramach testów wykonano **cztery główne analizy**, dostępne w folderze `raporty/`:

| Nr | Nazwa pliku PDF | Opis zawartości |
|----|------------------|-----------------|
| 0 | **Wstęp.pdf** | Krótkie podsumowanie celów testu, narzędzi i zakresu prac |
| 1 | **Testy funkcjonalne (UX-UI).pdf** | Zgłoszenia błędów użyteczności, formularzy, układu i intuicyjności |
| 2 | **Audyt SEO (Screaming Frog).pdf** | Wyniki crawl’a: duplikaty tytułów, ALT, przekierowania, linki 404 |
| 3 | **Analiza wydajności i dostępności (PageSpeed).pdf** | Ocena wydajności strony (LCP, CLS, FCP), dostępności i optymalizacji kodu |

---

## 🔍 Najważniejsze problemy wykryte

### 🧩 UX/UI
- Duplikacja pola „Adres e-mail” w formularzu rejestracyjnym
- Mylnie wyglądający element „lub” – udający przycisk
- Niski kontrast niektórych tekstów

### 📈 SEO
- 20 duplikatów tytułów
- 50 obrazów bez ALT
- 81 uszkodzonych linków (404)
- Ponad 6800 przekierowań (do weryfikacji)

### 🚀 Wydajność
- Bardzo dobre wyniki PageSpeed (Performance 94, SEO 92)
- Do poprawy: CLS = 0.141, niepotrzebny CSS (111 KiB), TTFB = 610 ms
- Brak WebP i width/height w <img>

---

## 📁 Dodatkowe dane techniczne

Wszystkie pliki źródłowe z narzędzia Screaming Frog SEO Spider (np. `redirects.csv`, `broken_links.csv`, itd.) znajdują się w osobnym folderze:

➡ `screamingfrog-crawl/`  
Zawierają one surowe dane wspierające raport nr 2 (Audyt SEO).

---

## ✅ Rekomendacje końcowe

- Poprawa formularzy i elementów UI dla lepszej intuicyjności
- Uzupełnienie metaopisów, ALT i tytułów
- Optymalizacja kodu CSS i obrazów
- Wdrożenie formatów nowej generacji (WebP), poprawa CLS
- Przejrzenie przekierowań i uszkodzonych linków

---

📎 Wszystkie PDF-y są dostępne w katalogu `raporty/`  
📊 Pliki źródłowe crawl'a: `screamingfrog-crawl/`
