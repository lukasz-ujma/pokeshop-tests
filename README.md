# 🧪 Testy manualne sklepu internetowego Pokeshop.pl

## 📌 Opis projektu

Ten projekt przedstawia manualne testy funkcjonalne przeprowadzone dla sklepu internetowego [Pokeshop.pl](https://pokeshop.pl), wykonane z wykorzystaniem narzędzia **TestLink**. Celem było zweryfikowanie kluczowych funkcji systemu e-commerce, takich jak rejestracja, logowanie, koszyk, zamówienia i płatności. Testy wydajnościowe, wykonane z wykorzystaniem narzędzia **Apache JMeter**, miały na celu zbadanie obciążenia serwera przy liczbie 100 użytkowników. Wykryte błędy zostały zgłoszone w systemie **Jira**.

Dokumentacja zawiera:
- plan testów
- przypadki testowe
- wykonanie testów
- zgłoszenie błędów
- raport końcowy

## 📂 Struktura projektu

pokeshop-tests/
├── README.md
├── docs/
│   ├── test_plan.md
│   ├── test_cases.md
│   ├── test_execution.md
│   ├── test_report_summary.md
│   ├── full_testlink_report.pdf
│   ├── performance_tests/
│   │    ├── pokeshop_performance_test.jmx
│   │    ├── test_results.csv
│   │    └── summary_report.png
│   ├── jira_issues/
│   │    ├── bug_001_zip_code.png
│   │    ├── bug_002_phone_number.png
│   │    └── bug_003_email.png

## 🛠️ Narzędzia i technologie

- ✅ **TestLink** – dokumentacja i zarządzanie testami
- 🖥️ Google Chrome – testy manualne na desktopie
- 🚀 **Apache JMeter** – testy wydajnościowe
- 📈 **Jira** – zgłoszenie błędów
- 📂 Git + GitHub – wersjonowanie i publikacja projektu

## 📊 Podsumowanie testów

- Liczba przypadków testowych: **78**
- Przypadki zakończone sukcesem: **75**
- Przypadki z błędami: **3**
- Ogólny wynik: ✅ (strona działa stabilnie, brak błędów krytycznych, wykryto średniej istotności błędy przy formularzu do rejestracji nowego użytkownika)

## ❌ Zgłoszone błędy

W trakcie testów manualnych zostały zidentyfikowane i zgłoszone trzy błędy do systemu **Jira**. Każdy z błędów został udokumentowany zrzutem ekranu i przypisany do odpowiedniego komponentu. Zrzuty z Jiry znajdują się w katalogu [`jira_issues`](docs/jira_issues).

Błędy:
1. **BUG-001**: Nie pojawia się komunikat walidacyjny po wpisaniu niepoprawnego kodu pocztowego 
2. **BUG-002**: Nie pojawia się komunikat walidacyjny po wpisaniu niepoprawnego numeru telefonu  
3. **BUG-003**: Pojawia się nieprawidłowy komunikat walidacyjny przy niepoprawnym mailu

## 📎 Dodatkowe pliki

- [`docs/full_testlink_report.pdf`](docs/full_testlink_report.pdf) – pełny raport z TestLinka
- [`docs/test_cases.md`](docs/test_cases.md) – przypadki testowe w formacie Markdown
- [`docs/test_execution.md`](docs/test_execution.md) – wyniki wykonania testów
- [`docs/performance_tests/pokeshop_performance_test.jmx`](docs/performance_tests/pokeshop_performance_test.jmx) – scenariusz testowy testów wydajnościowych
- [`docs/performance_tests/test_results.csv](docs/performance_tests/test_results.csv) – surowe dane z testów wydajnościowych
- [`docs/performance_tests/summary_report.png](docs/performance_tests/summary_report.png) – raport z testów wydajnościowych z Apache JMeter

## 🙋‍♂️ Autor

**Łukasz**  
🔗 [LinkedIn – Łukasz Ujma](https://www.linkedin.com/in/ujma-lukasz)  
📧 ujma.lukasz@gmail.com