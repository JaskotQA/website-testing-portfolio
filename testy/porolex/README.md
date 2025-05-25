# Testy – Porolex

## 🧪 Zakres testów

Dla strony **Porolex** wykonano następujące testy:

- ✅ Testy SEO
- ✅ Testy bezpieczeństwa (nagłówki HTTPS)
- ✅ Testy wydajności (Google PageSpeed – mobile i desktop)
- ✅ Testy funkcjonalne (formularz kontaktowy, panel administratora)
- ✅ Zestawienie wszystkich zgłoszeń i plików

## 🛠 Użyte narzędzia

- Google PageSpeed Insights
- Lighthouse
- DevTools
- Ręczne testy eksploracyjne
- Validator nagłówków HTTPS
- Formularze testowane ręcznie (manual testing)

## 📄 Raporty

Wszystkie raporty znajdują się w folderze `raporty/` i obejmują:

| Plik PDF | Zawartość |
|----------|-----------|
| 0. Zestawienie załączników | Podsumowanie wszystkich plików |
| 1. Raport SEO | Wyniki testów SEO |
| 2. Raport Bezpieczeństwa | Analiza nagłówków bezpieczeństwa |
| 3. Zgłoszenia błędów | Formularz kontaktowy, błędy panelu admina |
| 4. PageSpeed – Mobile | Wydajność na urządzeniach mobilnych |
| 5. PageSpeed – Desktop | Wydajność na komputerach |

## 🐞 Główne znalezione problemy

- Brak nagłówków bezpieczeństwa (np. `Content-Security-Policy`)
- Formularz kontaktowy nie waliduje wszystkich pól
- Niska wydajność strony mobilnej (PageSpeed poniżej 50)
- Brak favicon
