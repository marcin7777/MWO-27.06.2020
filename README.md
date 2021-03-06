Projekt końcowy Metody Wytwarzania Oprogramowania

## Szczegolowa specyfikacja programu

Program pobiera dane z plików Excel (rozszerzenie XLS) umieszczonych w strukturze katalogów rok-> miesiąc-> imię i nazwisko 


```
+---2012
|   +---01
|   |       Jan_Iksinski.xls
|   |       Jan_Kowalski.xls
|   |       Katarzyna_Nowak.xls
|   |       Piotr_Nowak.xls
|   |       Tomasz_jakistam.xls
|   |
|   +---02
|   |       Jan_Kowalski.xls
|   |
|   \---03
|           Jan_Kowalski.xls
|           Katarzyna_Nowak.xls
|           Piotr_Nowak.xls
|           Tomasz_jakistam.xls
|
\---2013
    +---01
    |       Jan_Iksinski.xls
    |       Katarzyna_Nowak.xls
    |       Kowalski_Jan.xls
    |       Nowak_Piotr.xls
    |       Tomasz_jakistam.xls
    |
    +---02
    |       Kowalski_Jan.xls
    |
    \---03
            Katarzyna_Nowak.xls
            Kowalski_Jan.xls
            Nowak_Piotr.xls
            Tomasz_jakistam.xls
```

## Interfejs programu (menu)
Po wczytaniu danych program wyświetla menu pozwalające na generowanie wybranego raportu.

		0: Pokaż wszystkie zaimportowane dane
		1: Alfabetyczne zestawienie listy pracowników <-> liczby godzin
		2: Alfabetyczne zestawienie projektów <-> liczba godzin
		3: Szczegółowy wykaz pracy kazdego pracownika
		4: Procentowe zaangazowanie danego pracownika w projektach w danym roku
		5: Szczegółowy wykaz pracy w danym projekcie
		6: Tworzenie wykresu słupkowego
		7: Tworzenie wykresu kołowego
		8. Exit

Przykład: Po naciśnięciu [1] i [Enter] zostanie wygenerowany raport pierwszy.

## Funkcjonalnosci programu
Program umożliwia tworzenie raportów opisujących aktywności poszczególnych pracowników.

* RAPORT 1

Program generuje alfabetyczną listę pracowników w danym roku kalendarzowym, wraz z ilością przepracowanych godzin.
Dane wyświetlane są w postaci czytelnej tabeli:

Imie i nazwisko -> ilość godzin 

* RAPORT 2 

Program generuje alfabetyczną listę projektów za dany rok kalendarzowy, wraz z ilością godzin, które zostały przepracowane w danym projekcie

1/Projekt_X -> ilość godzin

* RAPORT 3

Program generuje wykaz pracy każdego pracownika w danym projekcie, wraz z ilością przepracowanych godzin, oraz projektem któego dotyczy. 
System umożliwia wybór konkretnego pracownika poprzez wybranie jego imienia i nazwiska.

rok XXXX, Imie i nazwisko

Lp/Miesiac/Projekt/Liczba godzin 

* RAPORT 4

Program generuje wykaz procentowego zaangażowania danego pracownika w projektach w danym roku kalendarzowym. System umożliwia wybór żądanego roku.

Imię i nazwisko/Projekt_X / Projekt_Y

Imie i nazwisko/ a% / b%

* RAPORT 5

Pragram generuje szczegółowy wykaz pracy w danym projekcie, który pokazuje liczbe godzin wypracowanych przez poszczególnych pracowników w danym projekcie. 

Lp/Imie i nazwisko/ Liczba godzin

Lp/Imie i nazwisko/ Liczba godzin 

Lp/Imie i nazwisko/ Liczba godzin 

Suma: XXX [h]


* RAPORT 6 

Program rysuje wykres słupkowy do RAPORTU 2. 

gdzie:

x -> projekty

y -> liczba godzin, która wypracowana w danym projekcie


* RAPORT 7

Program zestawia wyniki procentowego zaangażowania danego pracownika w formie wykresu kołowego. 

Po naciśnięciu [7] i [Enter] zostanie wygenerowany wykres kołowy.


## Ograniczenia / known issues
Program przyjmuje dane w formacie excel (rozszerzenie XLS).
