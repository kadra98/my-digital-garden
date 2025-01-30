---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 5.03 – Pomiarowe wyznaczenie parametrów schematu zastępczego transformatora 3-fazowego/","tags":["wiedza/zettel"]}
---

* ## 1. Próba jałowa
	* transformator rozwarty po stronie wtórnej
	* po stronie zasilanej (pierwotnej) zasilany napięciem znamionowym
	* ### Pomiary
		* Napięcie pierwotne $U_{1}$
		* Prąd jałowy $I_{0}$
		* Moc czynna $P_{0}$
	* ### Obliczone wielkości
		* Straty rezystancyjne w żelazie (Reluktancja rdzenia): $R_{Fe}=\frac{U^2_{1}}{P_{0}}$
		* Prąd cz. czynnej: $I_{R}=\frac{U_{1}}{R_{Fe}}$
		* Reaktancję żelaza: $X_{m}=\frac{U_{1}}{\sqrt{I^2_{0}-I^2_{R}}}$
* ## 2. Próba zwarciowa
	* transformator zwarty po stronie wtórnej, po stronie pierwotnej doprowadza się napięcie zwarcia $U_{z}$ powodujące przepływ prądu znamionowego $I_{1}$ przez uzwojenie pierwotne
		* $u_{k}=\frac{I_{N}*Z_{k}}{U_{n}}*100\%$
		* inna nazwa **procentowa (względna) impedancja zwarcia**
		* napięcie zwarcia podane jest zawsze w karcie katalogowej, jednak można je obliczyć znając dane konstrukcyjne transformatora.
		* Szczegółowe obliczenia i wzory w [[10 Notatki/Poradnik Inżyniera Elektryka\|Poradnik Inżyniera Elektryka]] na str. 199 Tom II cz. I
	* w obliczeniach pomija się gałęź poprzeczną
		* ([[10 Notatki/Spadek sprawności transformatora przy jego mniejszym obciążeniu\|Spadek sprawności transformatora przy jego mniejszym obciążeniu]])
		* ![Pasted image 20250119175009.png](/img/user/80%20Zasoby/Pasted%20image%2020250119175009.png)
	* ### Pomiary
		* Napięcie zwarcia $U_{z}$
		* Prąd zwarcia (znamionowy) $I_{z}$
		* Moc zwarcia $P_{z}$
	* ### Obliczenia
		* Rezystancja w miedzi: $R_{z}=\frac{P_{z}}{I^2_{z}}$
		* impedancja zwarcia: $Z_{z}=\frac{U_{z}}{I_{z}}$
		* Reaktancja rozproszona: $X_{\sigma}=\sqrt{ Z^2_{z} -R^2_{z}}$