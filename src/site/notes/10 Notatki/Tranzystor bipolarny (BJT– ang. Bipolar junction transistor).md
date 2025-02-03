---
{"dg-publish":true,"permalink":"/10 Notatki/Tranzystor bipolarny (BJT– ang. Bipolar junction transistor)/","tags":["wiedza/zettel"]}
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
	* dzięki podaniu napięcia (i powstałemu w ten sposób prądowi) i zainicjowaniu ruchu między emiterem a bazą, dziury, które powstały w bazie przez ten ruch, są wykorzystywane do transmisji wolnych elektronów z emitera do kolektora
	* ![Pasted image 20250202133605.png](/img/user/80%20Zasoby/Pasted%20image%2020250202133605.png)
	* mały prąd bazy przekłada się na duży prąd kolektora
	* po zwiększeniu prądu bazy, prąd kolektora zwiększa się proporcjonalnie
		* a więc następuje wzmocnienie sygnału
* ## Rodzaje
	* #### NPN
		* ![Pasted image 20250202134604.png](/img/user/80%20Zasoby/Pasted%20image%2020250202134604.png)
		* ![Pasted image 20250202134620.png](/img/user/80%20Zasoby/Pasted%20image%2020250202134620.png)
	* #### PNP
		* ![Pasted image 20250202134640.png](/img/user/80%20Zasoby/Pasted%20image%2020250202134640.png)
		* ![Pasted image 20250202134654.png](/img/user/80%20Zasoby/Pasted%20image%2020250202134654.png)
	* sterowany prądowo
	* niewielki prąd bazy (płynący miedzy bazą a emiterem) steruje większym prądem między emiterem a kolektorem
* ## Parametry statyczne tranzystorów
	* $P_{max}$ – moc admisyjna, hiperbola mocy
	* $I_{cMAX}$ – prąd maksymalny (kolektora)
	* $I_{c{0}}$ – prąd zerowy
	* $U_{CEmax}$ – maksymalne napięcie
	* $U_{CEsat}$ – napięcie nasycenia
	* $\beta=\frac{I_{c}}{I_{B}}$ – współczynnik wzmocnienia prądowego
* ## Stany pracy
	* ### Stan odcięcia
		* gdy $U_{BE}<0$ lub gdy $I_{B}, I_{C}=0$
	* ### Stan aktywny
		* praca w obszarze liniowym
		* $I_{C}=\beta I_{B}$
	* ### Stan nasycenia
		* $I_{C}=\beta$, $I_{B}\geq\frac{E}{R}$
* ## [[10 Notatki/Układy pracy tranzystora bipolarnego (BJT)\|Układy pracy tranzystora bipolarnego (BJT)]]
	* 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/10-notatki/uklady-pracy-tranzystora-bipolarnego-bjt/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




 
* ### WB – wspólna baza
	* ![WB.jpg](/img/user/80%20Zasoby/WB.jpg)
	* prąd emitera $I_{E}$ jest podawany na wejście
	* prąd kolektora $I_{C}$ jest prawie równy prądowi emitera
	* prąd kolektora $I_{C}$ zależy głównie od prądu emitera $I_{E}$
	* $I_{C}= \alpha I_{E}$
		* $\alpha ≈ 1$
	* ![charakterystyki WB.jpg](/img/user/80%20Zasoby/charakterystyki%20WB.jpg)
* ### WE – wspólny emiter
	* ![WE 1.jpg](/img/user/80%20Zasoby/WE%201.jpg)
	* mały prąd sterujący bazy $I_{B}$ kontroluje duży prąd kolektora $I_{C}$
	* prąd kolektora $I_{C}$ zależy od prądu bazy $I_{B}$ i jest niemal niezależny od napięcia kolektor-emiter $U_{CE}$
	* $I_{C}= \beta I_{B}$
		* $\beta=20 \div 800$
* ### WC – wspólny kolektor
	* ![WC 1.jpg](/img/user/80%20Zasoby/WC%201.jpg)
	* prąd bazy $I_{B}$ steruje prądem emitera $I_{E}$
		* odwrotnie, niż w przypadku [[10 Notatki/Tranzystor bipolarny (BJT– ang. Bipolar junction transistor)#^1a9972\|układu WB]], gdzie prąd sterował prądem kolektora
	* $I_{E}=(\beta+1)I_{B}$
	* ![charakterystyki WE.jpg](/img/user/80%20Zasoby/charakterystyki%20WE.jpg)
* ## Porównanie układów pracy

| układ                  | [[10 Notatki/Tranzystor bipolarny (BJT– ang. Bipolar junction transistor)#^fffa96]\|WB]]                                                                                                                                    | [[10 Notatki/Tranzystor bipolarny (BJT– ang. Bipolar junction transistor)#^5fbc2d\|WE]]                                                                                                                                                                                            | [[10 Notatki/Tranzystor bipolarny (BJT– ang. Bipolar junction transistor)#^136fc6\|WC]]                                                                                                                                                                                                                                                                                                         |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| wzmocnienie napięciowe | **DUŻE**                                                                                                                                                       | **DUŻE**                                                                                                                                                                                                              | <1                                                                                                                                                                                                                                                                                                                                 |
| wzmocnienie prądowe    | ~1                                                                                                                                                             | **DUŻE**                                                                                                                                                                                                              | **DUŻE**                                                                                                                                                                                                                                                                                                                           |
| odwrócenie fazy        | nie                                                                                                                                                            | tak                                                                                                                                                                                                                   | nie                                                                                                                                                                                                                                                                                                                                |
| impedancja wejściowa   | niska                                                                                                                                                          | średnia                                                                                                                                                                                                               | **WYSOKA**                                                                                                                                                                                                                                                                                                                         |
| impedancja wyjściowa   | **WYSOKA**                                                                                                                                                     | średnia                                                                                                                                                                                                               | niska                                                                                                                                                                                                                                                                                                                              |
| Zastosowanie           | – wzmacniacze wysokiej częstotliwości<br>– bufory impedancyjne między źródłami<br>– bardzo niska impedancja wejściowa (utrudnia dopasowanie do źródła sygnału) | – duże wzmocnienie napięciowe i prądowe pozwala na zastosowanie układu do wzmacniania słabych sygnałów (np. mikrofonowych)<br>– stosowany w bramkach logicznych<br>– stosowany w generatorach sygnałów i oscylatorach | – dzięki wysokiej impedancji wejściowej i niskiej wyjściowej idealnie nadają się do dopasowania impedancji między różnymi stopniami wzmacniaczy<br>– stosowane jako separatory sygnału między układami o różnych impedancjach bez jego zniekształcania<br>– stosowany do sterowania tranzystorami MOSFET luub innymi układami mocy |


</div></div>

