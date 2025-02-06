---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 2.02 – Tyrystory – rodzaje, właściwości i zastosowanie/","tags":["wiedza/zettel"]}
---

* ## Rodzaje
	* ### Jednokierunkowy (struktura czterowarstwowa)
		* #### Diodowy (dynistor)
			* ![Pasted image 20250206185109.png](/img/user/80%20Zasoby/Pasted%20image%2020250206185109.png)
			* nie ma bramki sterującej
			* powrót do stanu blokowania następuje jedynie poniżej prądu przewodzenia
		* #### [[10 Notatki/Tyrystor (SCR – ang. silicone control recifier)\|Triodowy (tynistor, SCR)]]
			* ![Pasted image 20250206185120.png](/img/user/80%20Zasoby/Pasted%20image%2020250206185120.png)
	* ### Dwukierunkowy (struktura pięciowarstwowa)
		* #### Diodowy (diak)
			* ![Pasted image 20250206185151.png](/img/user/80%20Zasoby/Pasted%20image%2020250206185151.png)
			* blokuje prąd aż do osiągnięcia napięcia przebicia w dowolnym kierunku
			* po osiągnięciu progu przechodzi w stan przewodzenia i zachowuje się jak zwykła dioda
		* #### Triodowy (triak)
			* ![Pasted image 20250206185205.png](/img/user/80%20Zasoby/Pasted%20image%2020250206185205.png)
			* Załączany impulsem na bramkę w obu kierunkach, niezależnie od polaryzacji napięcia na elektrodach głównych
		* #### Tetrodowy
			* ![Pasted image 20250206185218.png](/img/user/80%20Zasoby/Pasted%20image%2020250206185218.png)
			* można go sterować oddzielnymi sygnałami dla obu kierunków przewodzenia
* ## Charakterystyki statyczne
	* ![Pasted image 20250206191113.png](/img/user/80%20Zasoby/Pasted%20image%2020250206191113.png)
	* $U_{BR}$ – napięcie przebicia tyrystora
	* $U_{\text{RRM}}$ – powtarzalne wsteczne napięcie szczytowe, które wynosi $\frac{3}{4}U_{BR}$. Przy napięciu tym jest możliwe określenie prądu natężenia $I_{\text{RRM}}$
	* $U_{B0}$ – napięcie przełączania
	* $I_{L}$ – prąd załączania , czyli prąd progowy w procesie załączanie tyrystora. Przekroczenie tego progu wprowadza tyrystor na stałe w stan przewodzenia
	* $I_{H}$ – prąd wyłączenia, czyli prąd progowy w procesie wyłączania tyrystora. Zmniejszenie natężenia prądu poniżej tego progu implikuje wyłączenie tyrystora
* ## Zastosowania
	* elektroenergetyka – układy [[HVDC\|HVDC]]
	* napędy elektryczne
	* Trakcje elektryczne
	* Przekształtniki o fazowym sterowaniu np.
		* sterowniki napięcia zmiennego
		* prostowniki napięcia
		* falownik z komutacją napięciem odbiornika
	* Układy elektrotermiczne
		* regulacja mocy grzania
	* Elektrotechnika smaochodowa
		* układy do ładowania akumulatorów
		* przerywanie kierunkowskazów
		* układy regulujące częstotliwość praccy wycieraczek samochodowych
		* układy zapłonowe
	* Układy sterowania oświetleniem
		* głównie mocą - natężeniem oświetlenia
	* Niektóre z nich, np. diaki, są wykorzystywane do wyzwalania innych elementów