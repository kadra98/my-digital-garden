---
{"dg-publish":true,"permalink":"/10 Notatki/Jednofazowy falownik tranzystorowy/","tags":["wiedza/zettel"]}
---

* ## Schemat
	* ![Pasted image 20250206212947.png](/img/user/80%20Zasoby/Pasted%20image%2020250206212947.png)
	* Diody podłączone równolegle do tranzystorów pełnią funkcję diod zwrotnych (rektyfikujących)
		* Chronią one tranzystory przed uszkodzeniem
			* W momencie wyłączenia tranzystorów, gdyby diody nie istniały, mogłoby pojawić się bardzo wysokie napięcie niszczące elementy półprzewodnikowe
			* A tak, prąd swobodnie przepływa przez diody rozładowując zgromadzoną wcześniej energię
* ## Zasada działania
	* Tego rodzaju falownik to nic innego, jak po prostu układ 4 przełączników połączonych ze sobą w układ H, które przełączają się parami
	* Bez funkcji MSI i modulacji PWM, napięcie na odbiorniku ma kształt przebiegu prostokątnego
	* W [[Falownik z MSI\|falowniku z funkcją MSI]] stosuje się [[sterowanie PWM\|sterowanie PWM]], które polega na porównywaniu za pomocą komparatora ([[10 Notatki/Wzmacniacz operacyjny\|Wzmacniacz operacyjny]]) napięcie sieciowe (sinus) z napięciem piłokształtnym
		* Wyjście wzmacniacza podłączone jest do dwóch bramek sterujących [[10 Notatki/Tranzystor polowy typu MOSFET\|MOSFETem]], z tymże jedna bramka poprzedzona jest bramką *NOT*, by nie powodować zwarcia w układzie
			* ![Pasted image 20250206213610.png](/img/user/80%20Zasoby/Pasted%20image%2020250206213610.png)
		* Jeśli różnica występuje, to wzmacniacz przeciąga impuls (impuls trwa dłużej), a jeśli jest mniejsza, to go skraca
			* ![Pasted image 20250206213751.png](/img/user/80%20Zasoby/Pasted%20image%2020250206213751.png)
		* drugi robi to samo , tylko że odwrotnie. Zsumowane sygnały wyglądają tak:
			* ![Pasted image 20250206213828.png](/img/user/80%20Zasoby/Pasted%20image%2020250206213828.png)
		* do wygładzenia sygnału stosuje się [[Filtr pasywny\|Filtr pasywny]]
			* do wygładzenia prądu – cewkę wpiętą szeregowo z odbiornikiem
			* do wygładzenia napięcia – kondensator wpięty równolegle z odbiornikiem
* ## Grafy pracy
	* Całość odbywa się wg następującego cyklu:
		1. 2 załączone zawory – prąd przepływa w pewną stronę na odbiorniku, napięcie dodatnie (1/4 okresu)
		2. 1 załączony zawór, powrót przez diodę – napięcie 0 na odbiorniku (1/4 okresu)
		3. wszystkie zawory zamknięte, prąd **wraca się** przez diody – następuje zmiana polaryzacji napięcia na odbiorniku, prąd w przeciwną stronę, niż jest wydawany przez źródło i w przeciwną do napięcia (chwila). Po zakończeniu kroku 3. prąd osiąga chwilowo wartość 0, napięcie jest już spolaryzowane ujemnie
		4. 2 przeciwne załączone zawory – prąd przepływa w przeciwną stronę przez odbiornik, napięcie ujemne na odbiorniku (1/4 okresu)
		5. 1 załączony zawór, powrót przez diodę – napięcie 0 na odbiorniku, prąd płynie w tym samym kierunku, co uprzednio
		6. wszystkie zawory zamknięte – zmiana polaryzacji napięcia na odbiorniku na dodatnią, prąd jeszcze płynie w kierunku przeciwnym
	* ![Pasted image 20250206215837.png](/img/user/80%20Zasoby/Pasted%20image%2020250206215837.png)
* ## Przebiegi czasowe
	* ![Pasted image 20250206215942.png](/img/user/80%20Zasoby/Pasted%20image%2020250206215942.png)
	* ### Ważne – na co zwrócić uwagę:
		* #### źródło
			* momentami prąd na źródle jest ujemny
			* prąd wydawany przez źródło w momencie napięcia 0 na odbiorniku wynosi również 0
		* #### prąd na odbiorniku
			* nie osiąga 0 w momencie, gdy napięcie na odbiorniku jest równe 0, tylko płynnie się rozładowuje
			* osiąga wartość 0 dopiero po powrocie (rozładowaniu) przez diody
		* #### prąd na tranzystorze
			* tożsamy z prądem odbiornika w momencie, gdy tranzystor przewodzi
				* przy powrocie przez diody, prąd spada do 0
		* #### prąd diody
			* zdecydowanie dorywczy, jedynie w okresach rozładowywania
* ## Zastosowanie
	* ### Przemysł
		* napędy silników
		* sprężarki
		* pompy
		* wentylatory
	* ### Energetyka
		* [[PV\|PV]]
		* elektrownie wiatrowe
		* [[UPS\|UPS]]
	* ### Transport
		* [[Samochody EV\|Samochody EV]]
		* metro
		* kolej
	* ### Automatyka domowa
		* [[10 Notatki/Instalacja oświetlenia\|Instalacja oświetlenia]]
			* płynna zmiana jasności oświetlenia dzięki modulacji impulsów
		* [[HVAC\|HVAC]]
		* inteligentne sterowanie energią
			* zmniejszenie zużycia energii poprzez regulację pracy pomp ciepła i wentylatorów