# Testy – AZ Ubezpieczenia

## 📅 Data testów
10 marca 2025

## 👤 Tester
Jakub Jaskot

## 🧪 Zakres testów

Przetestowano stronę: [https://nowa.az-ubezpieczenia.pl](https://nowa.az-ubezpieczenia.pl)  
Zakres testów obejmował:

- ✅ Walidację certyfikatu SSL
- ✅ Formularz kontaktowy (sekcja "Chcesz dowiedzieć się więcej?")
- ✅ Linki i przekierowania w sekcjach ofertowych

## 🛠 Użyte narzędzia

- Przeglądarki internetowe (Chrome, Firefox, Edge)
- Ręczne testy eksploracyjne
- Analiza zachowania formularzy i linków

## 🐞 Zgłoszone błędy

### 1. Nieprawidłowy certyfikat SSL
- 🔒 Podczas wejścia na [https://nowa.az-ubezpieczenia.pl](https://nowa.az-ubezpieczenia.pl) pojawia się komunikat: „Połączenie nie jest prywatne”.
- 📌 Certyfikat SSL nie obejmuje subdomeny `nowa.az-ubezpieczenia.pl`.
- ✅ Oczekiwane: Certyfikat powinien obejmować tę subdomenę.

---

### 2. Błędy w formularzu kontaktowym (dół strony)
- ⚠️ Po zmianie tematu w polu „Temat (wybierz z listy)” automatycznie podświetlają się puste pola „E-mail” i „Telefon”.
- ⚠️ Pole „Imię” nie podświetla się, mimo że prawdopodobnie jest wymagane.
- ✅ Oczekiwane: Pola powinny podświetlać się **dopiero** przy próbie wysłania formularza.

---

### 3. Błędne przekierowania w sekcjach ofertowych
- 📧 Kliknięcie w kategorię „Dzieci” (oraz inne jak „OC Przewoźnika”, „Mieszkaniowe”, itd.) otwiera... klienta poczty e-mail, zamiast strony z ofertą.
- ✅ Oczekiwane: Przekierowanie powinno prowadzić do właściwej podstrony ubezpieczenia.

---

## 📎 Załącznik
Szczegółowy raport PDF: `AZ-UBEZPIECZENIA.PL.pdf`

