---
{"dg-publish":true,"permalink":"/10 Notatki/Prawa Maxwella (prawa Gaussa, Ampere'a)/","tags":["wiedza/zettel"]}
---

* $\nabla$
	* wektor pochodnych zmiennych dotyczących położenia
	* ![Pasted image 20250210145550.png|100](/img/user/80%20Zasoby/Pasted%20image%2020250210145550.png)
	* pomnożony iloczynem skalarnym ($\cdot$) daje konkretną wartość (skalar)
		* to jest tak jakby pochodna wektora, jego zmian
	* pomnożony iloczynem wektorowym ($\times$) daje wektor prostopadły do płaszczyzny,, na którym znajdują się dwa mnożone wektory
		* to jest wirujący wektor
* ## 1. równanie (prawo Coulomba)
	* inaczej: prawo Gaussa dla elektryczności
	* $\nabla \cdot E=\frac{\rho}{\epsilon_{0}}$
		* po lewej – strumień magnetyczny (konkretna wartość, skalar)
		* $\rho$ – gęstość ładunku
			* $\rho=\frac{Q}{V}$
				* $V$  – objętość
	* czyli w skrócie
		* mówi to tym, że natężenie pola elektrycznego w jakiejś przestrzeni równe jest gęstości ładunku (jego wielkości w stosunku do przestrzeni, o której mowa), lecz zależnie od tego, jaka to jest przestrzeń (bazowo przenikalność elektromagnetyczna próżni)
	* prawo Coulomba jest specjalnym przypadkiem tego równania, złożonego do rzeczywistości 2D
* ## 2. równanie (zasada dwuimienności dipoli magnetycznych)
	* inaczej: prawo Gaussa dla magnetyzmu
	* $\nabla \cdot B=0$
		* po lewej – strumień magnetyczny
	* mówi o tym, że każda cząstka naładowana magnetycznie ma zawsze 2 bieguny: dodatni i ujemny (w efekcie indukcja wytworzona przez taką jedną cząstkę równa jest 0, bo one może nie tyle, że się odejmują, ale zapętlają – wszystkie linie wytworzonego pola biegną od N do S)
* ## 3. równanie ([[10 Notatki/SEM (Prawo Faradaya)\|SEM (Prawo Faradaya)]])
	* $\nabla \times E=-\frac{dB}{dt}$
		* po lewej – napięcie wytworzone przez pole elektryczne o natężeniu $E$
		* po prawej – zmiana strumienia magnetycznego w czasie
			* z [[10 Notatki/SEM (Prawo Faradaya)\|SEM (Prawo Faradaya)]] – $-\frac{d\Phi_{m}}{dt}$
	* zmieniający się strumień magnetyczny przechodzący przez pętlę generuje rotujące pole elektryczne w tej pętli, które to pole generuje napięcie elektryczne w tej pętli
	* i vice versa
* ## 4. równanie
	* inaczej: uogólnione prawo Ampere'a
	* $\nabla\times B=\mu_{0}j+\mu_{0}\epsilon_{0}\frac{dE}{dt}$
		* po lewej – rotujące pole magnetyczne
		* po prawej gęstość prądu $j=\frac{S}{I}$ 
			* $S$ – pole powierzchni pętli
			* $I$ – sumaryczny prąd przechodzący przez pętlę
			* i zmiana pola elektrycznego
	* rotujące pole magnetyczne zamkniętej pętli powstaje wskutek przypływu prądu prostopadle do tej pętli oraz zmianom pola elektrycznego przechodzącego przez tę pętlę
	* i vice versa oczywiście