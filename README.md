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
