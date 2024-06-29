---
{"dg-publish":true,"permalink":"/10 Notatki/Układy sterujące a regulacji/","tags":["wiedza/definicja"]}
---

* ### Układ sterujący / korekcyjny (idea sterowania) = układ otwarty
{ #243423}

	* w tym układzie za pomocą odpowiednio dobranego korektora dynamicznego zmieniamy właściwości dynamiczne układu
	* ![Pasted image 20240625182741.png](/img/user/80%20Zasoby/Pasted%20image%2020240625182741.png)
* ### Układ regulacji = układ zamknięty
{ #c15323}

	* to jest właśnie [[10 Notatki/UAR\|UAR]]
	* ![Pasted image 20240625183007.png](/img/user/80%20Zasoby/Pasted%20image%2020240625183007.png)
	* zakłócenie powoduje uchyb $\epsilon$
		* tenże uchyb jest sygnałem wejściowym dla regulatora
			* który generuje sygnał sterujący
				* a ten podaje go na obiekt
	* #### Typy [[10 Notatki/UAR\|UAR]]
{ #bab1c5}

		* **regulacja stałowartościowa (układ stabilizacji)**
{ #cc6781}

			* rolę wymuszeń pełnią zakłócenia,
				* to oznacza, że układ działa tak:
					* ok, temperatura / prędkość / itd spadła wskutek czegoś o tyle, więc należy ją podnieść
					* jednym z rodzajów tej regulacji jest regulacja dwustanowa
					* ale można realizować rówież regulację stałowartościową za pomoca regulatorów PID
						* jednak info nt uchybu biorą już z dokonanego faktu
							* ok spadło to tyle, w jakim czasie (I), jak to będzie się zmianiło w najbliższej przyszłości (D) i ile x trzeba zadziałać, żeby uchyb było 0 (P)
				* przykład to tempomat: przecież on mierzy tylko prędkość, nie mierzy wiatru, oporu powietrza, nachylenia terenu, poślizgu nawierchni
		* **regulacja programowa**
			* rolę wymuszeń pełnią wielkości zadane, np.
				* programowanie regulacji temperatury w piecu
		* **[[10 Notatki/Regulacja nadążna\|Regulacja nadążna]]**
			* rolę wymuszeń pełnią wielkości wyjściowe
			* oznacza to, że musimy mierzyć te zakłócenia, np. prąd prądnicy, temperaturę zewnętrzną, nasłonecznienie
			* Regulator temperatury, który mierzyłby nasłnecznienie szyby w samochodzie, temperaturę zewnętrzną, itd, to byłaby regulacja nadążna
				* ale jeśli mierzy jedynie temperaturę wewnętrzną, to jest to regulacja stałowartościowa