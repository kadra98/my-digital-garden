---
{"dg-publish":true,"permalink":"/10 Notatki/Układ regulacji prędkości obrotowej/","tags":["wiedza/definicja"]}
---

>    – Struktura układu
>    – wyjaśnienie sprzężenia od zakłócenia

* Można wykonać jako:
	* [[10 Notatki/Regulacja ze sprzężeniem od zakłócenia\|Regulacja ze sprzężeniem od zakłócenia]], lub
	* Regulacja ze sprzężeniem zwrotnym od wielkości regulowanej
* ![Pasted image 20240626213556.png](/img/user/80%20Zasoby/Pasted%20image%2020240626213556.png)
* Działanie:
	* Prąd obciążenia prądnicy to zakłócenie (bo zwiększa moment, z jakim silnik musi napędzać prądnicę)
	* Spadek napięcia na rezystancji $R_{N2}$ to $U_{R_{N2}}$  i jest to sygnał wyjściowy toru pomiaru zakłócenia
		* Więc sygnał sterowania to:
			* $kU_{0}*U_{R_{N2}}$
				* $k$ – wzmocnienie
				* $U_{0}$ – napięcie zadane
		* Sygnał dociera do węzła sumacyjnego ze znakiem $+$, bo kierunek oddziaływania zakłócenia i korekcji powinny być przeciwne
	* Układ ten dobiera wzmocnienie w taki sposób, by po ustaniu zakłócenia wartość wyjściowa była bez zmian
		* Można to zrobić metodą prób i błędów, lub analitycznie:
			* ![Pasted image 20240626214336.png](/img/user/80%20Zasoby/Pasted%20image%2020240626214336.png)
			* $k_{r}=\frac{\Delta U_{s}}{\Delta I_{2}R_{N2}k_{w}}$
				* gdzie:
				* $\Delta U_{s}=\Delta U_{s_1}-\Delta U_{s_2}$