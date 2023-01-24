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
## Subtask 3
** Po co piszemy test case’y?**
* Pomaga w zapewnieniu dobrego pokrycia testów (coverage).
* Pomaga w mierzeniu postępów testowania.
* Pomaga potwierdzić, że software spełnia wymagania (np. biznesu, czy użytkownika).
* Każdy może ich użyć (np. jeśli w przyszłości zmieni się tester).
* Są pomocne w testach regresyjnych i retestach.
* Pomaga znaleźć niejasności i potencjalne problemy, które mogą pomóc w usprawnieniu kodu.

<video src="https://www.youtube.com/watch?v=iZaAN7WmUuc"></video>
