---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 4.03 – Analiza prostego obwodu magnetycznego z magnesem trwałym i szczeliną powietrzną/","tags":["wiedza/zettel"]}
---

* ## Analogie do obwodów elektrycznych

| wielkość elektryczna          | wielkość magnetyczna                                       | jednostka wielkości magnetycznej     |
| ----------------------------- | ---------------------------------------------------------- | ------------------------------------ |
| prąd<br>$I$                   | strumień magnetyczny<br>$\Phi$                             | weber<br>$[\text{Wb}]$               |
| napięcie<br>$U$               | siła magnetomotoryczna<br>$F_{m}$                          | amper * liczba zwojów<br>$\text{An}$ |
| rezystancja (oporność)<br>$R$ | opór magnetyczny<br>$R_{m}$                                | $\frac{\text{Wb}}{\text{An}}$        |
| prawo Ohma<br>$U=I*R$         | prawo Ohma dla obwodów magnetycznych<br>$F_{m}=\Phi*R_{m}$ |                                      |
|                               |                                                            |                                      |
* ## Źródło pola
	* Źródłem pola jest magnes trwały, którego siłę magnetomotoryczną oblicza się ze wzoru
		* $F_{m}=B_{r} *l_{m}$
			* $B_{r}$ – [[10 Notatki/EGZ INŻ 4.01 – Podział materiałów magnetycznych. Charakterystyki magnesowania i właściwości materiałów magnetycznych stosowanych w obwodach magnetycznych o stałym i zmiennym polu magnetycznym#^15f22b\|remanencja]]
			* $l_{m}$ – długość magnesu
* ## Opór
	* Znów można to potraktować na zasadzie analogii do obliczania rezystancji:
	* zamiast $$R=\frac{l}{\sigma*S}$$
	* mamy
		* $$R_{m}=\frac{l_{m}}{\mu*\mu_{0}*S}$$
	* $l, l_{m}$ – długość przewodu; długość czegoś, przez co ma przechodzić strumień (np. szczeliny powietrznej)
	* $\sigma, \mu*\mu_{0}$ – przewodność materiału (elektryczna), względna przenikalność materiału (dla próżni = 1) x przenikalność próżni
	* $S$ – pole przekroju przewodnika, czegoś, co ma przenosić strumień magnetyczny
* ## Przykład obwodu magnetycznego
	* ![Pasted image 20250208205228.png](/img/user/80%20Zasoby/Pasted%20image%2020250208205228.png)
	* Wartość strumienia w tym obwodzie wynosi (z analogii do prawa Ohma)
		* $\Phi=\frac{F_{m}}{R_{tot}}$
			* bo $I=\frac{U}{R}$
	* Tak jak w przypadku rezystancji w obwodach elektrycznych, tak też tutaj, ze względu na fakt, że szczelina powietrzna ma znacząco większą oporność a niżeli rdzeń, to straty energii (w tym ciepła) będą odkładały się właśnie na tej szczelinie
* ## Energia magnetyczna szczeliny powietrznej
	* wyraża ją się wzorem
		* $$E_{m}=\frac{1}{2}*\mu_{0}*H_{g}^2*V_{g}$$
			* $H_{g}$ – natężenie pola magnetycznego w szczelinie powietrznej
			* $V_{g}$ – objętość szczeliny powietrznej
	* i tutaj też można znaleźć delikatną analogię, tym razem do energii zgromadzonej na okładach kondensatora:
		* $E_{c}=\frac{1}{2}*CU^2$
		* albo bardziej:
		* $$E_{c}=\frac{1}{2}*\epsilon*\frac{S}{d}*U^2$$
			* $\epsilon$ – przenikalność elektryczna materiału między okładkami kondensatora
			* $S$ – pole powierzchni okładek kondensatora
			* $d$ – odległość między okładkami kondensatora
* ## Zastosowanie szczeliny powietrznej
	* ### Głośniki
		* szczelina jest po prostu przestrzenią roboczą dla drgającej cewki
		* w szczelinie powietrznej wewnątrz magnesu trwałego znajduje się cewka głośnika, która poruszając się wprawia w ruch membranę, która generuje fale dźwiękowe
		* szczelina powietrzna ogranicza pole magnetyczne do obszaru, w którym pracuje cewka
		* zapewnia też stałe pole magnetyczne, co umożliwia liniową pracę cewki i minimalizuje zniekształcenia dźwięku
	* ### Czujniki położenia
		* pole magnetyczne z magnesu przenika przez szczelinę, umożliwiając detekcję pola przez czujnik
		* wielkość szczeliny wpływ na czułość i zakres pomiarowy
	* ### [[10 Notatki/Maszyna asynchroniczna (indukcyjna)\|Maszyna asynchroniczna (indukcyjna)]]
		* dzięki szczelinie powietrznej, strumień jest przenoszony do klatki wirnika
		* chociaż tutaj nacisk kładzie się na to, by szczelina powietrzna była jak najmniejsza