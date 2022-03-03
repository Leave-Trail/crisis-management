## Zarządzanie kryzysowe Iteracje.

### Iteracja 0. MVP
Grupa na fb połączona z mapą google. W modelu Concierge. Uczestnicy grupy uzupełniają informacje na temat dostępnych lokalizacji pomocy humanitarnej. Administrator uzupełnia te dane raz dziennie w mapie google.

### Iteracja 1. Mapa lokalizacji pomocy humanitarnej.
Celem tej iteracji jest dodanie możliwości dodawania lokalizacji pomocy humanitarnej do mapy oraz wyszukiwanie tych lokalizacji po kategoriach. Rozwiązanie składa się z aplikacji mobilnej oraz aplikacji web. Aktorami uczestniczącymi w tej iteracji jest Wolontariusz i Uciekinier.

* Jako Wolontariusz chcę mieć możliwość dodawania nowych lokalizacji pomocy humanitarnej z wykorzystaniem aplikacji mobilnej.

* Jako Wolontariusz chcę mieć możliwość dodawania nowych lokalizacji pomocy humanitarnej z poziomu aplikacji web.

* Jako Uciekinier chcę mieć możliwość sprawdzenia gdzie znajdują się najbliższe punkty pomocy oraz jakiego rodzaju pomoc może zostać mi tam udzielona. Chcę przeglądać punkty na mapie oznaczone odpowiedniem symbolem i kolorem a także na liście.

* Jako Uciekinier chcę dostać wskazówki dotarcia do wybranego przez siebie miejsca w aplikacji mobilnej  (Przekierowanie do map google)

### Iteracja 2. Dodanie zasobów.
Celem tej iteracji jest dodanie potrzeb, zasobów, aktualnej liczby osób przebywających w miejscu.
Wolontariusz lub osoba postronna która jest na miejscu może użyć aplikacji mobilnej aby poinformować inne organizacje o aktualnej sytuacji w danym miejscu.
Chcem publikować informacje na temat:
Ilość osób potrzebujących pomocy w danym miejscu.
Informacje bierzące Krótkie wiadomości z możliwością dodania kategorii jak informacja, zapotrzebowanie.
Dodawanie zasobów w danym miejscu oraz statusu zapotrzebowania. (Nadmiar, Braki)
Dla niektórych zasobów dodanie konkretnej ilości.

* Jako wolontariusz chcę mieć możliwość określenia liczby osób potrzbujących w danej lokalizacji w danym czasie.

* Jako wolontariusz chcę mieć możliwość definiowania zapotrzebowania na zasoby w danej lokalizacji a także sygnalizowania nadmiaru zasobu.
Określenie liczby sztuk danego zasobu w lokalizacji.



### Iteracja 3. Stany magazynowe
 W poprzedniej Iteracji zidentyfikowaliśmy obiekt zasobu lecz zdefiniowaliśmy tylko podstawowy mało precyzyjny współczynnik zapotrzebowania lub nadmiaru danego zasobu w lokalizacji. W obecnej iteracji dodamy stany magazynowe które określają ilość danego zasobu w lokalizacji. Na potrzeby raportowania utworzymy także tabelę historyczną która będzie pokazywała zmiany stanu magazynowego w czasie. Zdefiniujemy także obiekty Dodania na magazyn i zdjęcia z magazynu wraz z różnymi statusami jak wydanie produktu transport do innej lokalizacji, dodanie produktu.

* Jako Operator chcę mieć możliwość obsługi przyjęcia zasobów na stan. To znaczy w danej lokalizacji określony jest stan danego zasobu. Mamy obiekt dostawa lub wydanie w której określamy ile sztuk danego zasobu doszło lub ubyło. Dodatkowo określone są metadane. Kto dostarczył lub odebrał produkt

### Iteracja 4. Zlecenie transportu.
Poprzednie etapy przyniosły dużo wartości dodanej. Jednym rzutem oka na mapę można stwierdzić gdzie potrzebna jest pomoc, gdzie są nadmiary jakiegoś rodzaju rzeczy. Dzięki temu Uciekinierzy mogą łatwo dotrzeć do punktów pomocy a Wolontariusze w bardziej uporządkowany sposób mogą kierować swoją pomoc. Jednak nie jest jeszcze rozwiązany problem konkurowania o pewne miejsca. Co jeżeli w jednym momencie wielu kierowców spojrzy na mapę i sprawdzi, że na przejściu granicznym A oczekuje duża liczba uciekinierów. Może okazać się, że wszyscy pojadą w jedno miejsce i spowodują korek.
Drugi problem polega na tym, że osoby oczekujące na pomoc muszą zostać przetransportowana w zupełnie inne miejsca.
Odpowiedzią na te problemy jest zlecenie transportu zasobu z jednej lokalizacji w inną.
Kto miałby tworzyć takie zlecenia transportu. W obecnej iteracji nie mamy jeszcze odpowiedniej struktury. Nie możemy dopuścić wszystkich użytkowników do tworzenia zleceń transportu gdyż mogłoby spowodować to zamęt. W kolejnym etapie tworzymy odpowiednią strukturę organizacyjną która będzie mogła tworzyć role operatorów. Obecnie ograniczymy się do roli operatora która jest zdefiniowana na poziomie całej aplikacji.

* Jako Operator chcę mieć możliwość zdefiniowania zlecenia transportu przez wybranie zasobów wraz z określeniem ich ilości z danej lokalizacji pomocy humanitarnej a następnie w aplikacji web przeciągnięcia strzałki z jednego punktu do drugiego na mapie a, w aplikacji mobilnej wybranie punktu docelowego z mapy.
* Jako Operator chcę mieć możliwość zdefiniowania jaki typ transportu jest potrzebny do wykonania danego zlecenia transportu. Czy ma być to samochód osobowy autobus bus, tir, samolot pociąg czy inne.
* Zlecenia transportu trafiają do kolejki zleceń transportu .
* Jako Wolontariusz chcę mieć możliwość przeglądania zleceń transportu w postaci listy z możliwością filtrowania lokalizacji tak by móc wybrać transport najbardziej dogodny dla mnie.
* Do przedyskutowania kwestie wiarygodności. (Kiedy zdejmować zlecenie transportu z kolejki) Czy kiedy zostanie zrealizowane czy pobrane. 
* Do przemyślenia także kwestie weryfikacji kierowców. Prestiż, Wiarygodność, Ocena kierowcy. 
* Co w przypadku gdy transport nie dotrze.
* Pojawiały się już kwestie uprowadzeń lub wymuszeń i kradzieży.


### Iteracja 5. Organizacje
Organizacje zrzeszają ludzi wokół świadczenia jakiejś formy działania. Potrzebujemy wprowadzenia obiektu organizacji przed kolejnymi etapami aby umożliwić pewną ustrukturalizowaną formę zarządzania. Niektóre czynności mogą być wykonywane spontanicznie przez wolontariuszy lecz inne wymagają planowania i koordynacji. Definiowanie dyżurów, organizacja transportu. Do pomocy mogą włączać się już istniejące organizacje z własną strukturą. Musimy dać możliwość rejestracji tych organizacji w aplikacji udostępnienie swojego profilu działania a także powiązania ich z istniejącymi stronami www. Telefonami i innymi informacjami teleadresowymi.


### Iteracja 6. Kalendarze dyżurów podpięte pod lokalizację.

### Iteracja 7. Baza wiedzy.
