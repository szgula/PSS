# PSS

Projekt końcowy z przedmiotu Przemysłowe Systemy Sterowania

### Cel:

Celem projektu była realizacja miernika mocy rowerowego przy użyciu sterownika PLC oraz środowiska programistycznego TiaPortal. 

### Opis:

Wejściem układu jest miernik mocy który zwraca dyskretny sygnał o znanym zakresie (za układem ADC) - taki czujnik mógłby być reprezentowany przez potencjometr na sterownikach używanych w czasie zajęć. Następnie sygnał mocy (chwilowej) jest mnożony przez czas cyklu programu, a następnie sumowany w celu obliczenia całkowitej energii włożonej w czasie treningu (całkowanie metodą trapezów).

Dodatkowo użytkownik ma możliwość wprwadzenia maksymalnej energii którą chce włożyć w czasie treningu. Ta informacja jest używana w 2 celach:
  - porównania do włożonej energii i wskazania czy trening został już wykonany
  - estymacji czasu w jakim ukończymy trening (przy zachowaniu obecnej mocy)
  
  
### Kod programu:
![Alt text](zdjecia/kod.jpg?raw=true "kod_programu")

### Blok main
![Alt text](zdjecia/main.jpg?raw=true "main_programu")

### Print-Screen prezentujące działania
  
### Możliwości przyszłego rozwinięcia projektu:
1. Implementacja wykresu mocy
2. Wyznaczanie mocy średniej
3. Filtracja sygnału mocy
4. Estymowanie pozostałego czasu treningu na podstawie filtrowanego sygnału
