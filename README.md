# TASK 1
## Subtask 1
Punkty: 10
## Subtask 3
Cześć!

Nazywam się Beata i niedawno zaczęłam nową pracę na stanowisku testera manualnego w aplikacjach mobilnych.

Wprawdzie jakąś wiedzę już posiadam to chciałam poszerzyć zakres tej wiedzy i uważam, że ten challenge jest dobrym sposobem na osiągnięcie tego celu.
Spodziewam się, że dowiem się wielu nowych rzeczy, które pomogą mi rozwijać swoje umiejętności w pracy.

*Beata*


## Subtask 4
**Na czym polega ta aplikacja? Do czego służy?**
* Aplikacja służy do zarządzania graczami, meczami i do tworzenia raportów.


**Jakie funkcjonalności znajdują się w aplikacji? Do czego służą. Czy są intuicyjne, czy może byś coś zmienił_a? (Nie bój się wyrażać opinię!)**
* W aplikacji można dodawać graczy, mecze i generować raporty. Można też wyszukiwać graczy z listy, filtrować etc. Aplikacja jest całkiem intuicyjna, ale na pewno można by było ją usprawnić.
* To co jest ok to, że można filtrować i sortować kolumnami. 
* Z tego co widzę to ktokolwiek ma konto (wszystkie testowe konta) może edytować graczy. Nie widziałam natomiast opcji usuwania gracza. Przycisk „Clear” po utworzeniu zawodnika przestaje działać. 


**Oceń interfejs aplikacji (wygląd) – czy Ci się podoba, czy nie?**
* Niestety interface jest mało atrakcyjny. Wygląda bardzo prosto, czarno na białym niemalże. Strona główna nie jest w żaden sposób ułożona, w sensie „Scouts Panel”, Linki pomocnicze” i „aktywność” mogły być wyrównane do kafelków ilość graczy, mecy, raportów, akcji.


**Czy aplikacja jest intuicyjna? (Intuicyjna, czyli np. nie masz problemu ze zrozumieniem, co należy kliknąć, żeby wejść do formularza dodawania nowego zawodnika piłki nożnej do systemu).**
* Tak, myślę, że generalnie jest w miare intuicyjna, chociaż było dla mnie mylące to, że przy dodawaniu np. Gracza, wciśnięcie „sumbit” nie przenosiło mnie na ekran z profilem gracza tylko zostawało na tej samej stronie. Wprawdzie status dodawania pojawił się w prawym górnym rogu, ale nadal myślę, że powiniene być ekran, gdzie wszystko jest podsumowane i trzeba wcisnąc osobno przycisk edycji, by wrócić do ekranu i móc edytować.
To co było mniej intuicyjne to „Start meczu”, nie do końca wiedziałam w co kliknąć, żeby coś się zadziało na boisku, czy brakuje mi jakichś informacji etc. Dopiero po pewnym czasie odkryłam jak dodać różne czynności co szczerze mówiąc też nie wiele pomogą bo nie znam się na piłce nożnej. 
Nie jestem pewna, czy symulacja meczu i wypełnianie danych w ten sposób jest bardo intuicyjne. 


**Czy zauważasz jakieś błędy? Albo coś wydaje Ci się błędem? Zapisz swoje przemyślenia w pliku. Tutaj masz na to miejsce, czas i przestrzeń! ;)**
* Lokalizacja:
  * W wersji angielskiej niektóre pola zostają po polsku i vice versa.
  * „Please fill out this field” , „View column”, „show columns”, “download csv”, “filter table”,”print” “web match”, “submit”, “clear” “sorry, no matching records found” wyświetla się w polskiej wersji językowej.
* Pola edycji:
  * Przy tworzeniu lub edytowaniu pól nie ma żadnych ograniczeń
  * W prawie każdym polu można w używać samych cyfer, specjalnych znaków, jednego znaku, nieskończenie długiego łancucha znaków, emotikonów.  
  * Przy dodaniu bardzo długiego łańcucha znaków można zaobserwować clipping w głównym panelu (lewa strona) oraz aktywności na głównej stronie, overflowing w wygenerowanym raporcie, overlapping w tabeli, imię może wejść na kolumnę nazwisko etc.
  * Data urodzenia może być każda, nawet dzień dzisiejszy.
  * Edytowanie gracza imienia i nzawiska, nie zmienia się w lewym panelu po wciśnięciu „Submit”. Dopiero po kliknięciu w lewym panelu na gracza nazwa się uaktualnia.
  * Przy dodawaniu meczu, nie można wygenerowaćraportu bez „district” w profilu gracza, która nie jest wartością obowiązkową. Może powinna być, jeśli w kolejnych krokach bez niej się nie obejdzie.
* Przycisk „Clear” przestaje funkcjonować po zapisaniu gracza/meczu. Formularz nie czyści się.
* Nie widziałam też opcji usunięcia gracza.
* Przycisk Reset w filtrowaniu Players nie wyświetla z powrotem wszystkich wyników, tabela zostaje pusta.
* Wygląda na to, że ładowanie strony jest dosyć wolne, kliknięcie na „Players” ładuję stronę dosyć długo, nawet przy throttling na fast 3G. Na slow 3g jest bardzo wolne (ok. 80sec) 
* Raport z Lighthouse zwraca ok informacje dla desktop ale dla mobilnego urządzenia performance jest bardzo niski (12).
* Przy dodawaniu meczu, nie można wygenerowaćraportu bez „district” w profilu gracza, która nie jest wartością obowiązkową. Może powinna być, jeśli w kolejnych krokach bez niej się nie obejdzie.
* Po edycji imienia nie zmieniło się ono w raporcie. (może to zamierzone, ale będzie mylące szczególnie, że możmy edytować raport pod względzem innych danych.
* Przy symulacji używania aplikacji na telefonie, nie widziałam opcji sortowania graczy, przy 1800 graczach może to nie być najwygodniejsze. Filtrowanie pewnie pomoże, ale czasem sortowanie też może być przydatne.
* W wersji mobilnej raport w ogóle się nie przystosowuje do urządzenia, użytkownik musi scrollować przez cały raport, żeby zobaczyć poszczególne sekcje.



# TASK 2


## Subtask 1 & 2
* https://drive.google.com/drive/folders/1sjA2cRyHlKYrPIE4AQM9KvDTL_hQKIYe?usp=share_link


## Subtask 3
**Po co piszemy test case’y?**
* Pomaga w zapewnieniu dobrego pokrycia testów (coverage).
* Pomaga w mierzeniu postępów testowania.
* Pomaga potwierdzić, że software spełnia wymagania (np. biznesu, czy użytkownika).
* Każdy może ich użyć (np. jeśli w przyszłości zmieni się tester).
* Są pomocne w testach regresyjnych i retestach.
* Pomaga znaleźć niejasności i potencjalne problemy, które mogą pomóc w usprawnieniu kodu.


https://user-images.githubusercontent.com/122435818/214252671-bbe75001-9b40-494b-a9c2-61667d184304.mp4


[<img src="https://images.template.net/wp-content/uploads/2016/04/27133811/Youtube-Thumbnail1.jpg" width="50%">](https://youtu.be/OO3FANjwKHY "A komu to potrzebne?")



# TASK 3
https://drive.google.com/drive/folders/1WwsZ9x_z9TrZRcxVIKABR9hDqLPPrOdr?usp=share_link


# TASK 4
## Subtask 1 & 2
https://drive.google.com/drive/folders/1XBilWNgHLWhiAj9lDJyn97cPkUikKxyV?usp=share_link

## Subtask 3

**Do czego służy ta aplikacja? Jaki jest cel tej aplikacji?**
* Aplikacja służy do wyszukiwania ofert, kupowania i sprzedawania rzeczy, usług, etc. Aplikacja ma na celu ułatwienie korzystania z portalu olx.pl na telefonach komórkowych.


**Kto ma być użytkownikiem końcowym aplikacji?**
* Użytkownicy portalu olx.pl, wszyscu, którzy chcą coś sprzedać, kupić, a nawet znaleźć ofertę pracy.


**Czy według Ciebie aplikacja jest user friendly? (Przyjazna dla użytkownika- np. wchodzisz do aplikacji i szybko łapiesz do czego służą przyciski. Poczytaj na ten temat w internecie- co to znaczy, że aplikacja jest przyjazna dla użytkownika)**
* Na pewno dałoby się udoskonalić te aplikację, ale wydaję mi się, że jest w miare przyjazna użytkownikowi. Przynajmniej na pierwszy rzut oka. Nawigacja jest intuicyjna, łatwo się zorientować w ofertach i kategoriach, jak obserwować. Interfejs jest prosty. Na pozwolenie, aplikacja może wysyłać notyfikacje.Ikony kategorii wyglądaja czytelnie i przyspieszają wyszukianie.


**Jak byś usprawnił aplikację? Co byś w niej poprawił. Czy masz jakiś pomysł na dodatkową funkcjonalność? (Żeby nie było: nie jest to aplikacja przy której pracuję, takie pytania pojawiają się na rozmowach rekrutacyjnych dlatego dobrze jest to przećwiczyć :D )**
* Nie jestem pewna czy wiele bym usprawniła w aplikacji. To co na pewno bym zmieniła (ale to w każdej aplikacji) to reklamy, które się pojawiają pomiedzy wyszukiwaniem i opisem ofert. Wiem, że to pewnie nie możliwe, ale ogólnie reklamy w aplikacjach są frustrujące.
* Osobiście też lubię jak aplikacje są wielojęzykowe, a chociaż w języku angielskim, a nie tylko po polsku. Uważam, że w Polsce mieszka wielu obcokrajowców, którzy nie znają polskiego i fajnie by było jakby też mogli korzystać z aplikacji przynajmniej po angielksu.


**Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej?**
* Testowanie aplikacji internetowej polega na testowaniu jak strona/aplikacja wyświetla się w przeglądarce. Zakładam, że do używania aplikacji internetowej wymagane jest stałe połączenie z internetem, dla aplikacji natywnej zazwyczaj nie jest to potrzebne do wszystkiego. (zależy od aplikacji)
* Testowanie aplikacji natywnej skupia się na testowaniu jak aplikacja działa i wygląda na różnych urządzeniach i ekranach. Dla aplikacji internetowej skupiamy się zazwyczaj bardziej na kompatybilności na wielu przeglądarkach.
* Testowanie aplikacji internetowej nie wymaga testów takich jak usability, performance, czy testowania battery drainage, storage.

**Subtask 4

https://dare-it-2023-man-test.atlassian.net/jira/software/projects/CPP2/boards/1

* Bug template
![Bug template](https://user-images.githubusercontent.com/122435818/217286582-ccf7d2c3-34a5-4ba6-ac02-e5a5df4e4c70.jpg)

* Start of the Sprint
*![Start of sprint](https://user-images.githubusercontent.com/122435818/217287251-e46dc928-5eca-4d71-b40b-b6a2f67bc87d.jpg)


# TASK 4

## Subtask 1
SELECT
FROM
WHERE
AND/OR
IN
NOT LIKE
BETWEEN



## Subtask 2

![Task5_subtask2](https://user-images.githubusercontent.com/122435818/218429346-6b3be633-8caf-4f85-a37e-dab09d9de0db.jpg)



## Subtask 3
1. **Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.**

SELECT * FROM actors ORDER BY surname ASC;

![Task5_subtask3_pyt1_!](https://user-images.githubusercontent.com/122435818/218433330-faf2aeef-c2ed-47f5-8794-f44b18e83986.jpg)


2. **Wyświetl film, który powstał w 2019 roku.**

SELECT * FROM movies WHERE movies.year_of_production=2019;

![Task5_subtask3_pyt2](https://user-images.githubusercontent.com/122435818/218434471-ddfb278b-39c5-4e0a-abf7-de03c0bf7c2e.jpg)


3. **Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.**

SELECT * FROM movies WHERE movies.year_of_production BETWEEN 1990 AND 1999;

SELECT * FROM movies WHERE movies.year_of_production >=1990 AND movies.year_of_production<=1999;

![Task5_subtask3_pyt3](https://user-images.githubusercontent.com/122435818/218435264-655383f1-478d-4143-9912-5eb74adbecdb.jpg)


4. **Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$**

SELECT title, price FROM movies WHERE price<=7;

![Task5_subtask3_pyt4](https://user-images.githubusercontent.com/122435818/218436358-126e2b4f-d4b5-4b8e-9f65-45e95190caf7.jpg)


5. **Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.**

SELECT * FROM actors WHERE actor_id >=4 AND actor_id<=7;

![Task5_subtask3_pyt5](https://user-images.githubusercontent.com/122435818/218436864-68e58734-5802-4a5c-8a58-60067c431cf5.jpg)


6. **Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.**

SELECT * FROM customers WHERE customers.customer_id=2 OR customers.customer_id=4 OR customers.customer_id=6;

![Task5_subtask3_pyt6](https://user-images.githubusercontent.com/122435818/218438474-c1891c15-e82c-4f79-8912-79fc726c502b.jpg)


7. **Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.**

SELECT * FROM customers WHERE customers.customer_id IN (1,3,5);

![Task5_subtask3_pyt7](https://user-images.githubusercontent.com/122435818/218439108-8ac4ad72-bd51-4962-8b41-5f4d6fd7004b.jpg)


8. **Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.**

SELECT * FROM actors WHERE actors.name NOT LIKE 'An%';

![Task5_subtask3_pyt8](https://user-images.githubusercontent.com/122435818/218439696-e77ffc50-bb88-4301-aad0-59213403865d.jpg)


9. **Wyświetl dane klienta, który nie ma podanego adresu email.**

SELECT * FROM customers WHERE email IS NULL;

![Task5_subtask3_pyt9](https://user-images.githubusercontent.com/122435818/218439990-5ddd1f33-82d1-43a1-8fbf-061dc5db3ec3.jpg)


10. **Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.**

SELECT * FROM movies WHERE movies.price>=9 AND movies.movie_id BETWEEN 2 AND 8;

![Task5_subtask3_pyt10](https://user-images.githubusercontent.com/122435818/218440585-e2cd02d5-c26c-452d-9737-e2d69eb886d0.jpg)


