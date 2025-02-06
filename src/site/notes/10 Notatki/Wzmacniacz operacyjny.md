---
{"dg-publish":true,"permalink":"/10 Notatki/Wzmacniacz operacyjny/","tags":["wiedza/zettel"]}
---

* ## Cechy wzmacniacza idealnego
{ #493670}

	* nieskończone wzmocnienie
	* nieskończenie szerokie pasmo przenoszenia
	* [[10 Notatki/Co w praktyce oznacza nieskończona i zerowa impedancja w elektronice\|nieskończona impedancja wejściowa]]
		* wzmacniacz nie powinien pobierać żadnego prądu
	* zerowa rezystancja wyjściowa
		* brak ograniczeń pobieranego prądu ze wzmacniacza
* ## Budowa
	* Nie ma sensu się nad tym rozwodzić, składa się głównie z kilkudziesięciu tranzystorów i rezystorów
	* ![Pasted image 20250206191942.png|300](/img/user/80%20Zasoby/Pasted%20image%2020250206191942.png)
	* monolityczny układ scalony
	* W uproszczeniu
		* ![Pasted image 20250206192447.png](/img/user/80%20Zasoby/Pasted%20image%2020250206192447.png)
		* $\text{IN+}$ – wejście nieodwracające
		* $\text{IN–}$ – wejście odwracające
		* $\text{OUT}$ – wyjście
* ## Podstawowe układy
{ #3afd03}

	* ### Wzmocnienie napięcia
		* ![Pasted image 20250206192741.png](/img/user/80%20Zasoby/Pasted%20image%2020250206192741.png)
		* sygnał podajemy między 2 wejścia
		* na wyjściu mamy napięcie maksymalne, nieco niższe od napięcia zasilania
			* gdybyśmy odwrócili polaryzację na wejściach, to na wyjściu mielibyśmy napięcie ze znakiem –
		* napięcia na obu wyjściach dążą do zrównoważenia się
		* prąd nie przepływa w pętli po lewej stronie (nie płynie między + i –)
		* słaba użyteczność, bo po co nam coś, co podnosi nam napięcie do wartości napięcia zasilania
	* ### Wtórnik napięcia / bufor
		* ![Pasted image 20250206193248.png](/img/user/80%20Zasoby/Pasted%20image%2020250206193248.png)
		* zgodnie z zasadą, że napięcia na wyjściach dążą do tej samej wartości, napięcie na wyjściu będzie równe napięciowi na wejściu
	* ### Wzmacniacz nieodwracający
		* ![Pasted image 20250206194441.png](/img/user/80%20Zasoby/Pasted%20image%2020250206194441.png)
		* żaden prąd nie wpływa do wejścia
			* bo wejście to ma ogromną impedancję
		* znamy natomiast napięcie w węźle $X$ (z zasady dążenia do wyrównania się napięć na wejściach)
			* a skoro tak, to znamy prąd płynący przez rezystor $R_{1}$ do masy
			* prąd ten w całości przepływa również przez rezystor $R_{2}$
			* możemy obliczyć więc spadek napięcia na tym rezystorze
			* a następnie dodając do niego napięcie z węzła $X$, policzyć napięcie na wyjściu wzmacniacza
	* ### Wzmacniacz odwracający
		* ![Pasted image 20250206194648.png](/img/user/80%20Zasoby/Pasted%20image%2020250206194648.png)
		* ponieważ na wejście dajemy napięcie masy, to na wejściu odwracającym również mamy napięcie masy (0)
	* ### Sumator
		* ![Pasted image 20250206195755.png](/img/user/80%20Zasoby/Pasted%20image%2020250206195755.png)
		* sumuje napięcia
		* może tez je wzmocnić – wówczas wzmacnia je wg stosunku $\frac{R_{F}}{R}$
* 