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
+ strzał (góra, dół, prawo, lewo, góra-lewo, góra-prawo, dół-lewo, dół-prawo)
#### nagroda:
###### dodatnia:
+ przejście do następnej galaktyki
+ zestrzelenie wrogiego statku
+ napełnienie paliwa (odwrotnie proporcjonalna do ilości paliwa)
+ uratowanie 3 kadetów na planecie
###### ujemna:
+ utrata jednego życia
+ Zylos niszczy planetę
+ zwiększenie się czujności w hyperspace-ie (focus = (0-idealnie, 3-najgorzej))
#### cel:
+ maksymalizacja przyszłych nagród
+ dolecieć na Solaris
