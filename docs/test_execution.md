# ✅ Egzekucja testów – Pokeshop.pl

Dokumentacja wykonania przypadków testowych przeprowadzona manualnie na stronie [pokeshop.pl](https://pokeshop.pl), zgodnie z przypadkami z pliku `test_cases.md`.

---

## 📊 Podsumowanie testów

| ID | Nazwa | Status | Uwagi |
|----|-------|--------|-------|
| POK-1 | Dodanie produktu do koszyka | ✅ Pass | — |
| POK-2 | Usuwanie produktu z koszyka | ✅ Pass | — |
| POK-22 | Pozostawienie pustego formularza do rejestracji | ✅ Pass | — |
| POK-24 | Wpisanie niepoprawnego formatu kodu pocztowego | ❌ Fail | brak komunikatu walidacyjnego |
| POK-25 | Wpisanie niepoprawnego formatu numeru telefonu | ❌ Fail | brak komunikatu walidacyjnego |
| POK-26 | Wpisanie niepoprawnego formatu e-mail | ❌ Fail | niepoprawny komunikat walidacyjny |
| POK-32 | Utworzenie konta w serwisie | ✅ Pass | — |
| POK-34 | Zalogowanie do konta poprawnymi danymi | ✅ Pass | — |
| POK-36 | Wpisanie błędnego hasła | ✅ Pass | — |
| POK-38 | Wpisanie nieistniejącego emaila | ✅ Pass | — |
| POK-40 | Ustawienie nowego hasła do logowania | ✅ Pass | — |
| POK-41 | Wpisanie frazy niespełniającej wymogu ilości znaków | ✅ Pass | — |
| POK-42 | Wyszukanie produktów po nazwie Pokemona | ✅ Pass | — |
| POK-54 | Wyszukanie aktualnych promocji | ✅ Pass | — |
| POK-67 | Przekierowanie do logowania | ✅ Pass | — |
| POK-70 | Dokonanie zakupu produktów przez system płatności Paynow | ✅ Pass | — |
| POK-78 | Wejście na stronę główną 100 użytkowników | ✅ Pass | — |

**Legenda statusów:**
- ✅ Pass – test zakończony sukcesem
- ❌ Fail – test nie przeszedł
- 🚫 Blocked – test zablokowany (np. przez inny błąd)

---

## ❌ Szczegóły błędów

### POK-24 – Wpisanie niepoprawnego formatu kodu pocztowego

**Opis błędu:**
Nie pojawia się komunikat walidacyjny po wpisaniu niepoprawnego kodu pocztowego.

**Status:** ❌ Fail  
**Krytyczność:** Średnia  
**Rekomendacja:** Do zaimplementowania przez zespół developerski właściwy komunikat walidacyjny o treści: "Podaj kod pocztowy w formacie XX-XXX".

--

### POK-25 – Wpisanie niepoprawnego formatu numeru telefonu

**Opis błędu:**
Nie pojawia się komunikat walidacyjny po wpisaniu niepoprawnego numeru telefonu.

**Status:** ❌ Fail  
**Krytyczność:** Średnia  
**Rekomendacja:** Do zaimplementowania przez zespół developerski właściwy komunikat walidacyjny o treści: "Wpisz wymaganą liczbę znaków"

--

### POK-26 – Wpisanie niepoprawnego formatu e-mail

**Opis błędu:**
Pojawia się nieprawidłowy komunikat walidacyjny przy niepoprawnym mailu. Pojawia się komunikat walidacyjny o treści: "Podany email już jest w naszej bazie".

**Status:** ❌ Fail  
**Krytyczność:** Średnia  
**Rekomendacja:** Do zaimplementowania przez zespół developerski właściwy komunikat walidacyjny o treści: "Wpisano niepoprawny adres e-mail".

---

## 🧾 Uwagi końcowe

- Testy przeprowadzono w środowisku produkcyjnym.
- Wszystkie przypadki testowe zrealizowano ręcznie.
- TestLink był używany do planowania i rejestrowania wyników.

---

## 📎 Powiązane pliki

- [`test_cases.md`](test_cases.md) – szczegółowe przypadki testowe
- [`test_report_summary.md`](test_report_summary.md) – podsumowanie ogólne wyników testów
- [`full_testlink_report.pdf`](full_testlink_report.pdf) – pełny raport eksportowany z TestLinka