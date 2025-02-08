---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 3.04 – Pomiar impedancji i jej składowych (przyrządy, schemat obwodu, obliczenie modułu i fazy impedancji, sposób oznaczenia charakteru impedancji – pojemnościowy, indukcyjny)/","tags":["wiedza/zettel"]}
---

* ## Pomiar impedancji – najprościej jak można
	* dany jest obwód o nieznanej impedancji $Z$
	* obwód ten badamy w układzie poprawnie mierzonego napięcia i prądu zasilając obwód źródłem napięcia stałego DC o znanej wartości i stałej wartości
	* Z tych danych (napięcia i prądu) obliczamy rezystancję $R$
	* krok 2. powtarzamy przy zasilaniu obwodu napięciem AC
	* Z tym danych obliczamy impedancję $Z$
	* Reaktancję $X$ obliczamy ze wzoru
		* $X=\sqrt{ Z^2-R^2 }$
	* Całość możemy zapisać zgodnie ze wzorem:
		* $Z=R+jX$
	* Charakter obwodu ustalamy obliczając kąt $\Phi$
		* $\Phi= \text{arc}\tan (\frac{X}{R})$
			* $\Phi$ < 0 – charakter pojemnościowy
			* $\Phi$ = 0 – charakter rezystancyjny
			* $\Phi$ > 0 – charakter indukcyjny
* ## Inne metody
	* ### Pomiar za pomocą mostków #to-do/research 
		* Pomiar polega na porównaniu nieznanej wielkości impedancji z wielkościami wzorcowymi
		* #### [[10 Notatki/Mostek Wheatstone'a\|Mostek Wheatstone'a]]
		* #### Mostek Maxwella
		* #### Mostek Wiena
		* #### Mostek Heydta
	* ### Pomiar multimetrami
		* Nie wymaga wyjaśnień – przecież wszystko da się zmierzyć multimetrem
	* ### Pomiar oscyloskopem i generatorem funkcji
		* Wrzucamy na obwód napięcie sinusoidalne
		* Wrzucamy sobie na oscyloskop przebieg napięcia i prądu na elemencie
		* Mierzymy napięcie i prąd skuteczny
		* Obliczamy z tego impedancję
		* Patrzymy na oscyloskopie, o jaki kąt $\Phi$ jest prąd przesunięty od napięcia (lub vice verca)
		* Rezystancję obliczamy ze wzoru
			* $R=Z\cos \phi$
			* $X=Z\sin\phi$
	* #### Wektorowy analizator impedancji (VIA)
		* Urządzenie generuje sygnał sinusoidalny
		* Mierzy napięcie i prąd, a nastęnie oblicza impedancję
		* Przedstawia wynik w postaci wykresów Bodego lub Smitha