---
{"dg-publish":true,"permalink":"/10 Notatki/Tyrystorowy regulator napięcia przeminnego/","tags":["wiedza/zettel"]}
---

* ## Układy
	* ### Z tyrystorem symetrycznym
		* ![Pasted image 20250206222352.png](/img/user/80%20Zasoby/Pasted%20image%2020250206222352.png)
		* prostszy obwód główny (tylko jeden zawór)
		* mniejsze wymiary i masa
		* ==najczęściej stosowany obecnie układ w każdym przedziale mocy==
		* Większe obciążenie tyrystora
			* bo prąd przepływa przez niego w obu kierunkach
		* Zwiększone straty mocy
			* jednocześnie przewodzą 3 zawory
		* prostszy układ sterowania
	* ### Z tyrystorami w ramionach mostka
		* ![Pasted image 20250206222426.png](/img/user/80%20Zasoby/Pasted%20image%2020250206222426.png)
		* Lepsze przy obciążeniu indukcyjnością, bo tyrystory są chronione przez diody
	* ### Odwrotnie równoległy
		* ![Pasted image 20250206222416.png](/img/user/80%20Zasoby/Pasted%20image%2020250206222416.png)
		* Lepsze przy obciążeniu indukcyjnością, bo tyrystory są chronione przez diody
		* ze względu na różne potencjały katod, układy wyzwalania tyrystorów muszą być galwanicznie odizolowane
* ## Zasada działania
	* Zawór (tyrystor) włączamy z pewnym opóźnieniem, przy pewnym kącie sinusoidy
		* W efekcie, zgodnie ze wzorem na napięcie skuteczne (całka), spada wartość napięcia skutecznego na odbiorniku (bo zmniejsza się pole pod wykresem sinusoidy)
	* W praktyce działa to tak:
		* Prąd wydawany przez źródło przechodzi płynnie po sinusoidzie od wartości 0 V do pewnej wartości, którą osiąga przy kącie $\alpha$
		* W tym momencie załączamy tyrystor impulsem
		* Tyrystor wyłącza się samoistnie, gdy prąd osiąga chwilową wartość 0
		* Cykl się powtarza
* ## Przebiegi czasowe
	* 1. wykres – napięcie i prąd na odbiorniku
	* 2. wykres – napięcie na tyrystorze
	* 3. wykres – sygnał sterujący tyrystorem
	* ### [[Układ R\|Układ R]]
{ #585194}

		* ![Pasted image 20250206224304.png](/img/user/80%20Zasoby/Pasted%20image%2020250206224304.png)
	* ### [[Układ L\|Układ L]]
{ #2bc940}

		* ![Pasted image 20250206224321.png](/img/user/80%20Zasoby/Pasted%20image%2020250206224321.png)
		* uwaga: tyrystor wyłącza się w innym momencie, niż w [[10 Notatki/Tyrystorowy regulator napięcia przeminnego#^585194\|układzie R]], bo prąd jest przesunięty względem napięcia w prawo (czyli się spóźnia)
	* ### [[Układ RL\|Układ RL]]
		* ![Pasted image 20250206224507.png](/img/user/80%20Zasoby/Pasted%20image%2020250206224507.png)
		* prąd w obwodzie rozkłada się na składową sinusoidalną i składową wykładniczą
			* składowa wykładnicza wynika z *oddawania* prądu przez cewkę
			* w [[10 Notatki/Tyrystorowy regulator napięcia przeminnego#^2bc940\|układzie typu L]] składowej tej nie ma, bo
				* brak rezystancji oznacza brak tłumienia prądu
				* prąd ten oscyluje, lub momentalnie zmienia kierunek przepływu