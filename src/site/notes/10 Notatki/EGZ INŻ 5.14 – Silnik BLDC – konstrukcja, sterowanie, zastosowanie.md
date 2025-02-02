---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 5.14 – Silnik BLDC – konstrukcja, sterowanie, zastosowanie/","tags":["wiedza/zettel"]}
---

* ## Budowa
	* ![Pasted image 20250201213647.png](/img/user/80%20Zasoby/Pasted%20image%2020250201213647.png)
	* typ: zasadniczo outrunner, ale są tez z ruchomym wirnikiem w środku stojana
	* zasadniczo zewnętrzna, ruchoma część jest magnesem trwałym
		* niekeidy nie jest to lita, jedna część, lecz np cekcja magnesów trwałych
	* Uzwojenie stojana jest wewnątrz i składa się z kilku par cewek
		* uzwojenie to nawinięte jest na ferromagnetyk, żeby zwiększyć siłę pola
	* do uzwojenia doprowadzone jest zasilanie (DC)
		* zazwyczaj są albo 3 uzwojenia, albo 6 z uzwojeń
		* okablowane są w taki sposób, że z uzwojeń do układu sterującego wychodzą zawsze 3 końce
* ## Zasada działania
	* Za pomocą [[Czujnik Halla\|Czujnik Halla]] (czujnik położenia wału) sterownik przełącza (zamyka) 2 łączniki
		* ![Pasted image 20250201220938.png](/img/user/80%20Zasoby/Pasted%20image%2020250201220938.png)
	* Bardziej złożone układy (np. w przypadku 6ściu cewek) załączają naraz 2 pary uzwojeń, by jedno przyciągało wirnik, a drugie je odpychało
		* ![Pasted image 20250201221400.png](/img/user/80%20Zasoby/Pasted%20image%2020250201221400.png)
		* Powyższy sposób sterowania to tzw. square wave drive
			* napięcia mają (przynajmniej teoretycznie) kształt prostokątny i są względem siebie przesunięte o 120 stopni
			* Istniej także metoda tzw. *sine wave driving*, która polega na taki sterowaniu zaworami, by wartość napięcia nie przyjmowała wartości dyskretnych, tylko działa się płynnie, a napięcie na uzwojeniach miało kształt sinusoidy
				* Kształt napięcia zmienia się po prostu sinusoidalnie
* ## Zastosowanie
	* napędy dysków optycznych i twardych
		* ze względu na generację niskiej wartości pola magnetycznego i brak wprowadzanych zakłóceń do elektroniki komputera
		* ze względu na małe rozmiary
	* gramofony
	* pojazdy o napędzie elektrycznym
		* raczej mniejsze pojazdy
	* maszyny pracujące w warunkach zagrożonych wybuchem
		* ze względu na brak iskrzenia szczotek komutatora
	* wentylatory
	* elektronarzędzia
	* modelarstwo