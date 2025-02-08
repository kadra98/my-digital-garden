---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 3.03 – Metody pomiaru napięcia i prądu stałego oraz wartości skutecznej napięcia i prądu przemiennego/","tags":["wiedza/zettel"]}
---

* ## Pomiar napięcia DC
	* Oprócz tradycyjnego wpięcia woltomierza, można zastosować również mostek kompensacyjny
	* ### [[10 Notatki/Pomiar napięcia metoda kompensacyjną\|Pomiar napięcia metoda kompensacyjną]]
	* 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/10-notatki/pomiar-napiecia-metoda-kompensacyjna/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




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

</div></div>

* ## Pomiar pradu DC
	* ### Pomiar przez bocznik
		* oprócz klasycznego amperomierza, możemy zastosować metodę bocznikową
		* jest to po prostu pomiar spadku napięcia na boczniku, a następnie obliczyć przepływający przez niego prąd z prawa Ohma
		* Bocznik takki powinien być / zazwyczaj jest
			* niska, ale znana rezystancja
			* stabilny współczynnik temperaturowy
			* konstrukcja umożliwia odprowadzanie ciepła
	* ### Pomiar cęgami hallotronowymi
		* dzięki czujnikom opartym na [[efekt Halla\|efekt Halla]]
* ## Pomiary wartości skutecznej prądu i napięcia przemiennego
	* ### Pomiary za pomocą mierników analogowych
		* #### Mierniki elektromagnetyczne #to-do/research 
			* wykorzystują oddziaływanie pola magnetycznego na ruchomy element mechaniczny
				* przecież wskazówka amperomierza nie napierdala jak pojebana przy prądzie sinusoidalnym, tylko pokazuje stała wartość – właśnie RMS
			* nie nadają się do pomiaru przebiegów odkształconych
		* #### Mierniki termiczne (termoelektryczne)
			* wykorzystują elementy termiczne do pomiaru mocy strat w rezystorze
			* nadają się do przebiegów odkształconych – na zasadzie analogii do jednej z definicji wartości skutecznej
			* wysoka dokładność, ale wola odpowiedź czasowa
	* ### Pomiar za pomocą mierników cyfrowych
		* #### Mierniki True RMS
			* stosują przetwornik True RMS, który realizuje cyfrową całkę średniokwadratową
			* nadają się do przebiegów odkształconych
		* #### Mierniki średniokwadratowe
			* mierzą wartość średnią wyprostowanego napięcia i przeliczają na RMS
			* nadają się tylko do przebiegów nieodkształconych
		* #### Oscyloskopy
			* za pomocą przetworników mogą obliczać wartość RMS w czasie rzeczywistym