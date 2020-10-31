# solaris-usd
## Język programowania
+ Python
## Algorytmy
+ Q-learning
+ SARSA
## Biblioteki
+ GYM
+ Pandas - obróbka wyników
+ Seaborn - wizualizacja wyników
## Ujęcie problemu w postaci problemu decyzyjnego Markowa
#### Statek kosmiczny
#### stan:
+ w kosmosie
+ na planecie
+ skanuje galaktykę
+ w hyperspace
#### akcja:
+ nic nie rób
+ rusz się (góra, dół, prawo, lewo, góra-lewo, góra-prawo, dół-lewo, dół-prawo)
+ strzał
+ wybór sektora
#### nagroda:
###### dodatnia:
+ przejście do następnej galaktyki
+ zestrzelenie wrogiego statku
+ napełnienie paliwa (odwrotnie proporcjonalna do ilości paliwa)
+ uratowanie wszystkich kadetów na planecie (odwrotnie proporcjonalna do ilości żyć)
###### ujemna:
+ utrata jednego życia
+ Zylos niszczy planetę
+ zwiększenie się czujności w hyperspace-ie (focus = (0-idealnie, 3-najgorzej))
#### cel:
+ maksymalizacja przyszłych nagród
+ dolecieć na Solaris
## Interakcje
+ Stan: SCANNER
+ Cel: Maksymalizacja przyszłych nagród 
+ Akcje: Wybór sektora
<br><br>
+ Stan: Federation Planet
+ Cel: Znalezienie stancji dokującej w celu uzupełnienia paliwa, obrona planety jeśli znajdują się na niej jednostki wroga
+ Akcje: Poruszanie się statku, strzał
<br><br>
+ Stan: Zylon Planet
+ Cel: Znalezienie wszystkich kadetów (uzyskanie dodatkowego życia)
+ Akcje: Poruszanie się statku, strzał
<br><br>
+ Stan: Hyperspace
+ Cel: Utrzymanie jak najniższej wartości focus (oszczędzanie paliwa)
+ Akcje: Poruszanie się statku
<br><br>
+ Stan: Space (walka z flotą wroga)
+ Cel: Zniszczenie floty wroga, utrzymanie jak największej liczby żyć
+ Akcje: Poruszanie się statku, strzał
<br><br>
+ Stan: Corridor 
+ Cel: Zniszczenie planety (znalezienie stacji dokującej -> znalezienie kluczy)
+ Akcje: Poruszanie się statku, strzał
<br><br>
+ Stan: Space (walka z flotą wroga)
+ Cel: Zniszczenie floty wroga, utrzymanie jak największej liczby żyć
+ Akcje: Poruszanie się statku, strzał
<br><br>
+ Stan: Red zone (walka z flotą wroga)
+ Cel: Zniszczenie floty wroga, utrzymanie jak największej liczby żyć
+ Akcje: Poruszanie się statku (sterowanie jest na odwrót), strzał



