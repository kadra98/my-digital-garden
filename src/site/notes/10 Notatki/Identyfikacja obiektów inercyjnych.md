---
{"dg-publish":true,"permalink":"/10 Notatki/Identyfikacja obiektów inercyjnych/","tags":["wiedza/definicja"]}
---

* ### Za pomocą [[Charakterystyka częstotliwościowa\|Charakterystyka częstotliwościowa]]
	* punk po punkcie\
	* za pomocą rozwinięcia w szereg Fouriera za pomocą [[Algorytm FTT\|Algorytm FTT]]
	* ![Pasted image 20240625175115.png](/img/user/80%20Zasoby/Pasted%20image%2020240625175115.png)
	* $\frac{K_{m}}{k}=\frac{1}{2\xi \sqrt{ 1-\xi^2 }}$
	* $\frac{\omega}{\omega_{0}}=\frac{1}{\sqrt{ 1-2\xi^2 }}$
* ### Na podstawie odpowiedzi skokowych
	* #### Modele inercyjne
		* otrzymane wyniki przekształca się na skalę logarytmiczną wg:
			* $z(t_{i})=\ln{[1-\frac{h(t_{i})}{h_{ust}}]}$
		* 
		* ![Pasted image 20240625175527.png](/img/user/80%20Zasoby/Pasted%20image%2020240625175527.png)
			* dla modeli I rzędu otrzymuje się linię prostą
			* dla modeli II rzędu otrzymuje się linię zakrzywioną
		* parametry modelu:
			* $k=\frac{h_{ust}}{A}$
			* $T=-\frac{1}{a}$
				* $T_{2}=\frac{e^b-1}{e^b}*T_{1}$
	* #### Modele oscylacyjne
		* parametry wyznacza się bezpośrednio na podstawie odpowiedzi skokowej
			* $\xi=\frac{\ln{\frac{h_{1}}{h_{2}}}}{\sqrt{ 4\pi^2+[\ln{(\frac{h_{1}}{h_{2}})}]^2 }}$
			* $\omega_{0}=\frac{2\pi}{T_{w}\sqrt{ 1-\xi^2 }}$