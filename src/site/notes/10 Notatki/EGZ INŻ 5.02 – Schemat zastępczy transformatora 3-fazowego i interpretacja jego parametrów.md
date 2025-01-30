---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 5.02 – Schemat zastępczy transformatora 3-fazowego i interpretacja jego parametrów/","tags":["wiedza/zettel"]}
---

* ## Schemat 
	* ![Pasted image 20250119142654.png](/img/user/80%20Zasoby/Pasted%20image%2020250119142654.png)
* ## Parametry
	* $U_{1}$ – napięcie strony pierwotnej
	* $U'_{2}$ – napięcie strony wtórnej
	* $R_{1}, R'_{2}$ – straty rezystancyjne w miedzi
	* $R_{Fe}$ – [[10 Notatki/EGZ INŻ 5.01 – Straty mocy czynnej w ferromagnetyku przy polu sinusoidalnie zmiennym – geneza, zależności, skutki (przykłady)\|straty czynne w rdzeniu]]
		* $R_{Fe}=\frac{3U^2_{1}}{P_{Fe}}$
	* $X_{f}$ – straty reaktancyjne odpowiadające prądowi magnesującemu $I_{f}$
		* **Prąd $I_{f}$** ten nie bierze udziału w przenoszeniu mocy obciążeni, lecz **służy do wytwarzania zmiennego strumienia magnetycznego w rdzeniu transformatora** ($\Phi$ – strumień główny)
			* ![Pasted image 20250119143935.png](/img/user/80%20Zasoby/Pasted%20image%2020250119143935.png)
		* W transformatorze rdzeń musimy przemagnesowywać. Energię do jego przemagnesowywania dostarcza właśnie prąd $I_{f}$ 
		* Jest bierny, ponieważ jego głównym zadaniem jest pokonanie reaktancji magnetycznej rdzenia (czyli jakby pokonanie reaktancji *cewki*)
		* Jego wielkość zależy od indukcyjności rdzenia, czyli od łatwości jego przemagnesowywania
		* Zgodnie z prawem Ohma, im rdzeń ma większą indukcyjność (reaktancję), tym łatwiej go namagnesować i tym prąd magnesujący jest mniejszy
			* Jeśli rdzeń ma małą indukcyjność (reaktancję), to prąd magnesujący będzie musiał być większy
		* $X_{f}=\frac{U_{1}}{I_{0}}$
	* $X_{l1,l_{2}}$ – reaktancja strumienia rozproszonego $\Phi_{s1}$
{ #0e3f25}

		* strumień, który nie zamyka się przez rdzeń i nie bierze udziału w sprzężeniu z drugim uzwojeniem, ale zamka się lokalnie wokół przewodów uzwojeń
		* to jest dodatkowa indukcyjność (a więc impedancja), która jest oporem (impedancją) dla prądu
	* Należy pamiętać, że na schemacie zastępczym, po stronie wtórej, wszystkie wielkości są ze znakiem $'$ i trzeba je przeliczyć wg zależności:
		* $I'_{2}=\frac{z_{2}}{z_{1}}*I_{2}$
		* $U'_{2}=U_{2}*\frac{z_{1}}{z_{2}}$
		* $R'_{2}=R_{2}*(\frac{z_{1}}{z_{2}})^2$
		* Podstawowe wzory na przekładnię:
			* $\frac{z_{1}}{z_{2}}=\frac{U_{1}}{U_{2}}$
			* $\frac{z_{1}}{z_{2}}=\frac{I_{2}}{I_{1}}$ – **prądy na odwrót**