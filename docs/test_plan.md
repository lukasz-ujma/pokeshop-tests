# 🧾 Plan testów – Pokeshop.pl

## 🎯 Cel testów
Celem testów jest sprawdzenie poprawności działania podstawowych funkcjonalności sklepu internetowego Pokeshop.pl.

## 📌 Zakres testów
1. Testy funkcjonalne:
- Rejestracja nowego użytkownika
- Logowanie i wylogowanie
- Przeglądanie katalogu produktów
- Dodawanie produktu do koszyka
- Składanie zamówienia
- Proces płatności
- Obsługa błędów (np. błędne dane logowania)

2. Testy integracyjne:
- komunikacja z systemem modułu płatności
- komunikacja API z serwisami typu social media

3. Testy wydajnościowe:
- szybkość działania serwera
- zdolności obciążeniowe serwera

## ❌ Zakres wyłączony
- Testy automatyczne, bezpieczeństwa

## ⚙️ Środowisko
- Strona produkcyjna: [https://pokeshop.pl](https://pokeshop.pl)
- Przeglądarka: Google Chrome (wersja 136.0.7103.114)
- System operacyjny: macOS Sonoma 14.3.1

## 🧪 Metodyka
Testy wykonane ręcznie na podstawie przypadków testowych w TestLinku. Wyniki dokumentowane były bezpośrednio w systemie TestLink oraz wyeksportowane do pliku PDF.

## 🧰 Narzędzia
- TestLink 1.9.20 [DEV]
- Jmeter (testy wydajnościowe)
- GitHub (publikacja projektu)
