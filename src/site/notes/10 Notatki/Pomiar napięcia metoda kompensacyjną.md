---
{"dg-publish":true,"permalink":"/10 Notatki/Pomiar napięcia metoda kompensacyjną/","tags":["wiedza/zettel"]}
---

* ## Generalna zasada działania
	* ![Pasted image 20250208161232.png](/img/user/80%20Zasoby/Pasted%20image%2020250208161232.png)
	* Należy zrobić tak, żeby spadek napięcia $U_{k}$ był taki sam, jak napięcie mierzone $U_{x}$
	* ergo: żeby przez galwanometr (bardzo dokładny amperomierz) nie płynął żaden prąd (bo nie będzie wtedy różnicy potencjałów)
* ## [[Kompensator Lindecka\|Kompensator Lindecka]] (stała rezystancja, zmienny prąd)
	* ![Pasted image 20250208161503.png](/img/user/80%20Zasoby/Pasted%20image%2020250208161503.png)
	* po lewej stronie układu wpinamy albo źródło prądowe o regulowanym pądzie, albo źródło napięciowe, a prąd regulujemy przez rezystor
	* natężenie prądu podnosimy (lub zmniejszamy rezystancję) do momentu, gdy galwanometr nie będzie pokazywał 0
	* napięcie $U_{x}$ obliczamy ze wzoru
		* $U_{x}=I_{p}*R_{N}$
		* **ważne:** wartość rezystancji $R_{N}$ jest stała (a najlepiej, żeby była wzorcowana)
	* Kompensatora używa się do pomiaru sił termoelektrycznych, gdyż umożliwia on w prosty sposób osiąganie małych zakresów mierzonych napięć. Np. stosując  amperomierz o zakresie 10 mA i rezystor o wartości 0,1 $\Omega$ osiąga się zakres 1 mV
* ## [[Kompensator np. Feussnera\|Kompensator np. Feussnera]] (stały prąd, zmienna rezystancja)
	* ![Pasted image 20250208164333.png](/img/user/80%20Zasoby/Pasted%20image%2020250208164333.png)
	* początkowo regulujemy prąd $I_{p}$ w taki sposób, by [[ogniwo Westona\|ogniwo Westona]] o znanym napięciu $E_{N}$ kompensowało spadek napięcia na rezystorze $R_{w}$ i aby spełniony został warunek
		* $R_{w}*I_{p}=E_{N}$
	* wówczas przełącznik jest ustawiony w pozycji 1, a przez galwanometr nie płynie żaden prąd
	* następnie, nie zmieniając wartości prądu $I_{p}$, przełączamy przełącznik do pozycji drugiej i dostosowujemy rezystancję $R_{k}$ w taki sposób, by całkowity spadek mierzonego napięcia odbywał się właśnie na tym rezystorze, a galwanometr by nie wskazywał żadnej wartości
		* $I_{p}*R_{kx}=U_{x}$