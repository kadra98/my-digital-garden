---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 1.02 – Moce w obwodach z przebiegami okresowymi odkształconymi/","tags":["wiedza/zettel"]}
---

* ## Przebieg odkształcony
	* każdy okresowy, niesinusoidalny
* ## Plan działania
	* ### 1. Rozkładamy przebieg w [[10 Notatki/Szereg Fouriera\|Szereg Fouriera]]
		* w szereg możemy rozłożyć w zasadzie każdy okresowy przebieg, w przyrodzie nie występują takie przebiegi okresowe, których się nie da rozłożyć (nie ma drzew rosnących do nieba)
			* czysto teoretycznie nie można rozłożyć np. [[Delta Diracca\|Delta Diracca]] – pionowej szpilki do nieskończoności w górę w nieskończenie krótkim okresie czasu
		* nawet jeśli uważamy, że nie jest odkształcony, to nic się nie zepsuje, jeśli go rozłożymy
		* to wykonujemy za pomocą [[Algorytm FTT\|Algorytm FTT]]
		* na wyjściu mamy przebieg rozłożony na składniki (są to [[Wyższe harmoniczne\|Wyższe harmoniczne]]), które po zsumowaniu, dadzą nam sygnał (przebieg) wejściowy
			* te składniki to sinusoidy o różnej wartości amplitudy, okresie i przesunięciu
	* ### 2. Obliczamy to, czego nie mamy
		* no bo rozkładamy albo przebieg prądu, albo przebieg napięcia
			* (przynajmniej tak było w zadaniach)
		* więc to drugie (prąd albo napięcie) musimy dla określonych harmonicznych policzyć\
			* **UWAGA** jeżeli w obwodzie występują elementy reaktancyjne, to należy zwrócić uwagę, jak zachowują się przy innych częstotliwościach, bo jak wiadomo – reaktancje kondensatorów i cewek zależą od częstotliwości
				* może się zdarzyć, że przy pewnych częstotliwościach występują zjawiska [[Rezonans elektromagnetyczny\|Rezonans elektromagnetyczny]]
			* nie zapominać, że algorytm może wyrzucić np. składową stałą
			* nie wykonujemy obliczeń dla parzystych harmonicznych, bo nie wnoszą nic do rachunków
	* ### 3. Obliczamy moce P czynne dla harmonicznych
		* $P_{h}=|U_{h}|*|I_{h}|*\cos(\psi_{h}-\theta_{_{h}})$
			* $\psi$ – kąt przesunięcia napięcia
			* $\theta$ – kąt przesunięcia prądu
			* $h$ – numer harmonicznej
		* sumujemy otrzymane moce
			* $P=P_{0}+P_{1}+P_{3}+P_{5}+\dots$
	* ### 4. Obliczamy [[10 Notatki/Moc bierna\|moce bierne]] Q dla harmonicznych oraz moc bierną Budeanu (sumę mocy biernych harmonicznych)
		* analogicznie jak wyżej, z tą różnicą, że
			* $Q_{h}=|U_{h}|*|I_{h}|*\sin(\psi_{h}-\theta_{h})$
		* $Q_{B}=Q_{1}+Q_{3}+Q_{5}+\dots$
	* ### 5. Obliczamy moce pozorne S, bierną Fryzego i deformacji
		* $S=|U|*|I|$
		* $Q_{F}=\sqrt{ |S|^2 -P^2}$
		* $D=\sqrt{ Q_{F}^2-Q_{B}^2 }$
		* ![Pasted image 20250208215710.png](/img/user/80%20Zasoby/Pasted%20image%2020250208215710.png)
* ## Inne zagadnienia
	* ### [[10 Notatki/THD  - Współczynnik odkształcenia napięcia w SEE\|THD  - Współczynnik odkształcenia napięcia w SEE]]
		* $$\text{THD}=\sqrt{ \frac{\Sigma |A_{h}|^2}{|A_{1}|^2} }*100 \%$$
		* $A_{h}$ – amplituda h-tej harmonicznej
		* $A_{1}$ – amplituda 1. harmonicznej
		* czysta sinusoida – THD = 0%
	* ### Wymagania odnośnie THD
		* <8% ogólnej zawartości harmonicznych – dostawcy energii elektrycznej na [[Sieć n\|Sieć n]]
		* <5% maksymalnej wartości pojedynczej harmonicznej – dostawcy energii na [[Sieć n\|Sieć n]]
		* <1% – w sprzęcie audio
	* ### Wymagania odnośnie urządzeń
		* oprócz wymagań dla dostawców energii elektrycznej, istnieją także wymagania odnośnie urządzeń, takich jak np. AGD (klasa A), urządzenia przenośne <75W (klasa B), oświetlenie (C), urządzenia o mocy <600W i PF <0.95
			* wymagania zapisuje się na różne sposoby dla 3., 5., i 7. harmonicznej
				* albo w wielkościach bezwzględnych prądu (np. <2,3 A dla 3. harmonicznej)
				* albo w procentowej zawartości danej harmonicznej prądu (np. 3. harmoniczna <87% prądu)
				* albo w wartościach bezwzględnych uwzględniających moc urządzenia (np. 3,4 mA/W dla 3. harmonicznej)