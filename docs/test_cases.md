# 📄 Przypadki testowe – Pokeshop.pl

W projekcie przygotowano 78 przypadków testowych w TestLink. Poniżej przedstawiono reprezentatywny przekrój przypadków, które ilustrują strategię testowania, różne typy scenariuszy oraz pokrycie funkcjonalne kluczowych modułów aplikacji. Wszystkie przypadki testowe są opisane w raporcie końcowym z TestLinka (docs/full_testlink_report.pdf)

--

## POK-1:Dodanie produktu do koszyka

**Moduł:** Produkt
**Priorytet:** Wysoki
**Wydanie:** 1.0.2

**Kroki testowe:** 
1. Otwieramy stronę https://pokeshop.pl.
2. Klikamy w zakładkę "Wszystkie produkty".
3. Klikamy w pierwszy produkt z listy.
4. Klikamy w przycisk "Dodaj do koszyka".
5. Klikamy w przycisk "Przejdź do koszyka".

**Oczekiwany rezultat:** Produkt w koszyku

--

## POK-2:Usuwanie produktu z koszyka

**Moduł:** Produkt
**Priorytet:** Wysoki
**Wydanie:** 1.0.2
**Warunek wstępny:** Istnieje dodany produkt w koszyku

**Kroki testowe:** 
1. Otwieramy stronę https://pokeshop.pl.
2. Klikamy w ikonkę "Koszyk".
3. Klikamy w ikonę "X" w kolumnie o nazwie "Usuń".

**Oczekiwany rezultat:** Koszyk pusty

--

## POK-22:Pozostawienie pustego formularza do rejestracji

**Moduł:** Formularz do rejestracji
**Priorytet:** Wysoki
**Wydanie:** 1.0.2

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. Najeżdżamy kursorem myszki na ikonkę "Panel klienta".
3. Klikamy w przycisk "Załóż konto".
4. Nie wpisujemy żadnych danych na formularzu i klikamy w przycisk "Utwórz konto"

**Oczekiwany rezultat:** Wyświetliły się komunikaty walidacyjne przy wszystkich obowiązkowych polach o treści "Pole jest wymagane"

--

## POK-24:Wpisanie niepoprawnego formatu kodu pocztowego

**Moduł:** Formularz do rejestracji
**Priorytet:** Średni
**Wydanie:** 1.0.2
**Dane wejściowe:** Kod pocztowy: 1

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. Najeżdżamy kursorem myszki na ikonkę "Panel klienta".
3. Klikamy w przycisk "Załóż konto".
4. W polu "Kod pocztowy" wpisujemy wartość wejściową.

**Oczekiwany rezultat:** Pojawił się komunikat walidacyjny o treści "Podaj kod pocztowy w formacie XX-XXX"

--

## POK-25:Wpisanie niepoprawnego formatu numeru telefonu

**Moduł:** Formularz do rejestracji
**Priorytet:** Średni
**Wydanie:** 1.0.2
**Dane wejściowe:** Numer telefonu: 1

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. Najeżdżamy kursorem myszki na ikonkę "Panel klienta".
3. Klikamy w przycisk "Załóż konto".
4. W polu "Numer telefonu" wpisujemy wartość wejściową.

**Oczekiwany rezultat:** Pojawił się komunikat walidacyjny o treści "Wpisz wymaganą liczbę znaków"

--

## POK-26:Wpisanie niepoprawnego formatu e-mail

**Moduł:** Formularz do rejestracji
**Priorytet:** Średni
**Wydanie:** 1.0.2
**Dane wejściowe:** Adres email: a@a

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. Najeżdżamy kursorem myszki na ikonkę "Panel klienta".
3. Klikamy w przycisk "Załóż konto".
4. W polu "Adres email" wpisujemy wartość wejściową.

**Oczekiwany rezultat:** Pojawił się komunikat walidacyjny o treści "Wpisano niepoprawny adres e-mail"

--

## POK-32:Utworzenie konta w serwisie

**Moduł:** Formularz do rejestracji
**Priorytet:** Wysoki
**Wydanie:** 1.0.2
**Dane wejściowe:**
Imię: Lucaz
Nazwisko: Test
Ulica i numer domu / lokalu: Testowa 1
Kod pocztowy: 00-100
Miejscowość: Warszawa
Numer telefonu: 123456789
Adres email: lucaztest@proton.me
Hasło: qwerty
Powtórz hasło: qwerty

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. Najeżdżamy kursorem myszki na ikonkę "Panel klienta".
3. Klikamy w przycisk "Załóż konto".
4. Wypełniamy poszczególne pola formularza wartościami wejściowymi oraz zaznaczamy checkboxy przy wymaganych zgodach.
5. Klikamy w przycisk "Utwórz konto".
6. Klikamy w przycisk "Panel klienta".

**Oczekiwany rezultat:** Panel klienta wyświetlił się poprawnie. Nowy użytkownik został zalogowany

--

## POK-34:Zalogowanie do konta poprawnymi danymi

**Moduł:** Formularz do logowania
**Priorytet:** Wysoki
**Wydanie:** 1.0.2
**Warunek wstępny:** Zarejestrowane konto w sklepie internetowym
**Dane wejściowe:**
Adres email lub nick: lucaztest@proton.me
Hasło: qwerty

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. Najeżdżamy kursorem myszki na ikonkę "Panel klienta".
3. Klikamy w przycisk "Zaloguj się".
4. Wpisujemy w polach formularza wartości wejściowe, a następnie klikamy w przycisk "Zaloguj się".
5. Klikamy w przycisk "Panel klienta"

**Oczekiwany rezultat:** Użytkownik poprawnie zalogowany

--

## POK-36:Wpisanie błędnego hasła

**Moduł:** Formularz do logowania
**Priorytet:** Wysoki
**Wydanie:** 1.0.2
**Warunek wstępny:** Zarejestrowane konto w sklepie internetowym
**Dane wejściowe:**
Adres email lub nick: lucaztest@proton.me
Hasło: qwe

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. Najeżdżamy kursorem myszki na ikonkę "Panel klienta".
3. Klikamy w przycisk "Zaloguj się".
4. Wpisujemy w polach formularza wartości wejściowe, a następnie klikamy w przycisk "Zaloguj się".

**Oczekiwany rezultat:** Wyświetlił się komunikat walidacyjny o treści: "Błędny adres email / nick lub hasło użytkownika

--

## POK-38:Wpisanie nieistniejącego emaila

**Moduł:** Odzyskiwanie hasła
**Priorytet:** Średni
**Wydanie:** 1.0.2
**Warunek wstępny:** Zarejestrowane konto w sklepie internetowym
**Dane wejściowe:** Podaj adres email: lucaztest@proton.pl

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. Najeżdżamy kursorem myszki na ikonkę "Panel klienta".
3. Klikamy w przycisk "Zaloguj się".
4. W obszarze "Odzyskiwanie hasła" wpisujemy w polu "Podaj adres email" wartość wejściową, a następnie klikamy w przycisk "Wyślij".

**Oczekiwany rezultat:** Wyświetlił się komunikat walidacyjny o treści: "Podany login / email nie istnieje w naszym sklepie"

--

## POK-40:Ustawienie nowego hasła do logowania

**Moduł:** Odzyskiwanie hasła
**Priorytet:** Wysoki
**Wydanie:** 1.0.2
**Warunek wstępny:** Zarejestrowane konto w sklepie internetowym
**Dane wejściowe:**
Podaj adres email: lucaztest@proton.me
Nowe hasło: qwerty123
Powtórz hasło: qwerty123

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. Najeżdżamy kursorem myszki na ikonkę "Panel klienta".
3. Klikamy w przycisk "Zaloguj się".
4. W obszarze "Odzyskiwanie hasła" wpisujemy w polu "Podaj adres email" wartość wejściową, a następnie klikamy w przycisk "Wyślij".
5. Klikamy w przycisk "Zaloguj się".
6. Wchodzimy na skrzynkę mailową podaną w danych wejściowych.
7. Klikamy w link z treści maila.
8. W polach formularza do nadania hasła wpisujemy wartości wejściowe.

**Oczekiwany rezultat:** Pojawiło się okno z komunikatem o treści: "Twoje hasło zostało zmienione" oraz dwa przyciski: "Zaloguj się" i "Przejdź do strony głównej"

--

## POK-41:Wpisanie frazy niespełniającej wymogu ilości znaków

**Moduł:** Wyszukiwarka produktów
**Priorytet:** Średni
**Wydanie:** 1.0.2
**Dane wejściowe:** "a"

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. W polu wyszukiwarki wpisujemy wartość wejściową, a następnie klikamy w ikonkę "lupy".

**Oczekiwany rezultat:** Pojawiło się okno z komunikatem o treści: "Minimalna ilość znaków w polu wyszukiwania to: 2"

--

## POK-42:Wyszukanie produktów po nazwie Pokemona

**Moduł:** Wyszukiwarka produktów
**Priorytet:** Średni
**Wydanie:** 1.0.2
**Dane wejściowe:** Charizard

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. W polu wyszukiwarki wpisujemy wartość wejściową, a następnie klikamy w ikonkę "lupy".

**Oczekiwany rezultat:** Wyświetla się lista produktów zawierających frazę z wartości wejściowej w nazwie lub opisie produktu

--

## POK-54:Wyszukanie aktualnych promocji

**Moduł:** Strona główna
**Priorytet:** Wysoki
**Wydanie:** 1.0.2

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. Klikamy w przycisk "Promocje".

**Oczekiwany rezultat:** Wyświetliła się lista produktów będących w promocji

--

## POK-67:Przekierowanie do logowania

**Moduł:** Strona główna
**Priorytet:** Średni
**Wydanie:** 1.0.2

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. Klikamy w dolnej sekcji strony w przycisk "Logowanie".

**Oczekiwany rezultat:** Wyświetliła się strona do logowania

--

## POK-70:Dokonanie zakupu produktów przez system płatności Paynow

**Moduł:** Proces zakupu
**Priorytet:** Wysoki
**Wydanie:** 1.0.2
**Warunki wstępne:**
1. Użytkownik jest zalogowany.
2. Użytkownik dodał co najmniej jeden produkt do koszyka.
3. Użytkownik wskazał wybraną formę przesyłki.
4. Uzytkownik wybrał formę płatności jako Paynow.

**Kroki testowe:**
1. Otwieramy stronę https://pokeshop.pl.
2. Klikamy w ikonkę "Koszyk".
3. Klikamy w przycisk "Do kasy".
4. Zaznaczamy wymagane zgody.
5. Klikamy w przycisk "Zamawiam i płacę".
6. Klikamy w przycisk "Płacę".
7. Na stronie bramki płatniczej Paynow klikamy w wybraną metodę płatności, następnie w przycisk "Płacę", potwierdzamy płatność, a następnie klikamy przycisk "WRÓĆ DO SKLEPU"

**Oczekiwany rezultat:** Otworzyła się strona sklepu z komunikatem: "Płatność wykonana. Dziękujemy za dokonanie płatności". Proces zakupu został zrealizowany poprawnie.

--

## POK-78:Wejście na stronę główną 100 użytkowników

**Moduł:** Wydajność i obciążenie
**Priorytet:** Średni
**Wydanie:** 1.0.2
**Parametry przypadku testowego:**
1. Liczba użytkowników - 100
2. Czas - 10 sekund
3. Oczekiwany czas odpowiedzi serwera - 3000 ms

**Kroki testowe:**
1. Wykonanie testu zgodnie z parametrami przypadku testowego w aplikacji Jmeter.
2. Weryfikacja czasu odpowiedzi serwera

**Oczekiwany rezultat:** Serwer odpowiedział w czasie niższym niż 3000 ms przy każdym użytkowniku