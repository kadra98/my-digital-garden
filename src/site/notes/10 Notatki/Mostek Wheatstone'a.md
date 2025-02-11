---
{"dg-publish":true,"permalink":"/10 Notatki/Mostek Wheatstone'a/","tags":["wiedza/zettel"]}
---

* ## Zastosowanie
	* stosowany do pomiaru rezystancji w szerokim zakresie
	* zaletą jego jest fakt, że wszystkie rezystory (przynajmniej w teorii) powinny mieć taką samą temperaturę, wiec ich przyrost rezystancji zmienia się w taki sam sposób
	* przez to, możemy badać np. jedynie oddziaływanie siły na rezystor tensometryczny
* ## Schemat i zasada działania
	* Prąd przepływa dwiema drogami:
		* przez rezystory $R_{1}$ i $R_{2}$
		* oraz przez rezystory $R_{3}$ i $R_{x}$
		* ![Pasted image 20250208192320.png](/img/user/80%20Zasoby/Pasted%20image%2020250208192320.png)
	* Zgodnie z [[10 Notatki/Metoda węzłowa\|Metoda węzłowa]]:
		* napięcie w węźle C równe jest
			* $V_{C}=\frac{R_{2}}{R_{2}+R_{1}}*E_{źr}$
		* napięcie w węźle D równe jest
			* $V_{D}=\frac{R_{x}}{R_{x}+R_{3}}*E_{źr}$
		* napięcie między węzłami C i D równa się
			* $U_{CD}=V_{C}-V_{D}$
	* konstruując mostek, musimy spełnić założenie, że $V_{C}=V_{D}$ , więc jesteśmy w stanie tak algebraicznie poprzekształcać powyższe równania, by otrzymać równanie na $R_{x}$:
		* $R_{x}=R_{3}*\frac{R_{2}}{R_{1}}$
		* $\frac{R_{2}}{R_{1}}$ traktujemy jako stałą
		* modulujemy wartość $R_{3}$ do momenty, gdy spełnione zostanie założenie, że $U_{CD}=0$
		* wówczas jesteśmy w stanie wyznaczyć (obliczyć wartość $R_{x}$)
			* a następnie badać zmiany rezystancji rezystora pod wpływem różnych czynników, np.
				* temperatury – termistor
				* światła – czujnik światła
				* siły – tensometr
* Jest to przykład przetwornika rezystancyjno-napięciowego, bo na podstawie odczytu napięcia (między dwoma ramionami – C i D), jesteśmy w stanie badać zmiany rezystancji elementu