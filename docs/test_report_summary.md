# 📋 Podsumowanie testów – Pokeshop.pl

## 🧪 Cel testów

Celem testów było zweryfikowanie podstawowej funkcjonalności sklepu internetowego [pokeshop.pl](https://pokeshop.pl) z perspektywy użytkownika końcowego, obejmując procesy rejestracji, logowania, dodawania produktów do koszyka oraz składania zamówień.

---

## 📊 Wyniki testów

| Wskaźnik | Wartość |
|----------|---------|
| Liczba przypadków testowych | 78 |
| Przypadki zakończone sukcesem | 75 |
| Przypadki zakończone niepowodzeniem | 3 |
| Blokery krytyczne | 0 |
| Pokrycie funkcjonalne (szacunkowe) | 80% |

---

## ❌ Błędy wykryte podczas testów

### 🔴 POK-24 – Wpisanie niepoprawnego formatu kodu pocztowego
- **Opis:** Nie pojawia się komunikat walidacyjny po wpisaniu niepoprawnego kodu pocztowego.
- **Krytyczność:** Średnia
- **Status:** ❌ Fail
- **Rekomendacja:** Do zaimplementowania przez zespół developerski właściwy komunikat walidacyjny o treści: "Podaj kod pocztowy w formacie XX-XXX".

--

### 🔴 POK-25 – Wpisanie niepoprawnego formatu numeru telefonu
- **Opis:** Nie pojawia się komunikat walidacyjny po wpisaniu niepoprawnego numeru telefonu.
- **Krytyczność:** Średnia
- **Status:** ❌ Fail
- **Rekomendacja:** Do zaimplementowania przez zespół developerski właściwy komunikat walidacyjny o treści: "Wpisz wymaganą liczbę znaków"

--

### 🔴 POK-26 – Wpisanie niepoprawnego formatu e-mail
- **Opis:** Pojawia się nieprawidłowy komunikat walidacyjny przy niepoprawnym mailu.
- **Krytyczność:** Średnia
- **Status:** ❌ Fail
- **Rekomendacja:** Do zaimplementowania przez zespół developerski właściwy komunikat walidacyjny o treści: "Wpisano niepoprawny adres e-mail".

---

## ✅ Wnioski

- Strona działa stabilnie.
- Wykryto trzy średniej istotności błędy przy formularzu do rejestracji nowego użytkownika. Nieprawidłowe dane kontaktowe mogłyby w przyszłości utrudnić skuteczne dostarczanie zamówień.
- Testy objęły najważniejsze funkcje sklepu z punktu widzenia użytkownika.
- Wskazane jest przeprowadzenie kolejnych testów po poprawkach, szczególnie w obszarze funkcjonowania formularza do rejestracji.

---

## 📎 Powiązane materiały

- [`test_plan.md`](test_plan.md) – plan testów
- [`test_cases.md`](test_cases.md) – przypadki testowe
- [`test_execution.md`](test_execution.md) – wykonanie testów
- [`full_testlink_report.pdf`](full_testlink_report.pdf) – oryginalny raport PDF z TestLinka
- [`summary_report.png`](summary_report.png) – raport z testów wydajnościowych z Apache JMeter

---

**Autor:** Łukasz  
📅 Data wykonania testów: *[02-06-2025]*  