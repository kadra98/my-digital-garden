---
{"dg-publish":true,"permalink":"/10 Notatki/Tranzystor/","tags":["wiedza/zettel"]}
---

* ## Zasadniczo wykorzystywane jako
	* Działa jak przełącznik bez ruchomych elementów
	* Wzmacniacze sygnałów
* ## Budowa
	* tranzystor zbudowany jest z  3 warstw: N-P-N
	* warstwy te są skonstruowane w tak samo jak w przypadku [[10 Notatki/Dioda#^222085\|złącza P-N, jak w przypadku diody]]
		* tj. dziury i elektrony
	* składa się z
		* emitera – warstwy N, z której wypływają elektrony
		* bazy – złącza P, przez którą elektrony swobodnie przepływają
		* kolektora – złącza N, z które wypływają elektrony z tranzystora
* ## Zasada działania
	* ### Tranzystor bipolarny (BJT – ang. Bipolar junction transistor)
		* dzięki podaniu napięcia (i powstałemu w ten sposób prądowi) i zainicjowaniu ruchu między emiterem a bazą, dziury, które powstały w bazie przez ten ruch, są wykorzystywane do transmisji wolnych elektronów z emitera do kolektora
		* ![Pasted image 20250202133605.png](/img/user/80%20Zasoby/Pasted%20image%2020250202133605.png)
		* mały prąd bazy przekłada się na duży prąd kolektora
		* po zwiększeniu prądu bazy, prąd kolektora zwiększa się proporcjonalnie
			* a więc następuje wzmocnienie sygnału
* ## Rodzaje
	* ### Bipolarny BJT – ang. Bipolar junction transistor
		* #### NPN
			* ![Pasted image 20250202134604.png](/img/user/80%20Zasoby/Pasted%20image%2020250202134604.png)
			* ![Pasted image 20250202134620.png](/img/user/80%20Zasoby/Pasted%20image%2020250202134620.png)
		* #### PNP
			* ![Pasted image 20250202134640.png](/img/user/80%20Zasoby/Pasted%20image%2020250202134640.png)
			* ![Pasted image 20250202134654.png](/img/user/80%20Zasoby/Pasted%20image%2020250202134654.png)
		* sterowany prądowo
		* niewielki prąd bazy (płynący miedzy bazą a emiterem) steruje większym prądem między emiterem a kolektorem
		* #### Parametry statyczne tranzystorów
			* $P_{max}$ – moc admisyjna, hiperbola mocy
			* $I_{cMAX}$ – prąd maksymalny (kolektora)
			* $I_{c{0}}$ – prąd zerowy
			* $U_{CEmax}$ – maksymalne napięcie
			* $U_{CEsat}$ – napięcie nasycenia
			* $\beta=\frac{I_{c}}{I_{B}}$ – współczynnik wzmocnienia prądowego
* ## Układy pracy
	* ### WB – wspólna baza
		* ![WB.jpg](/img/user/80%20Zasoby/WB.jpg)
		* ![charakterystyki WB.jpg](/img/user/80%20Zasoby/charakterystyki%20WB.jpg)