---
{"dg-publish":true,"permalink":"/10 Notatki/Regulator PID/","tags":["wiedza/definicja"]}
---

> Transmitancja, parametry, wskaźniki jakościowe (na podstawie wykładu)

* Wzory opisujące regulator
	* Transmitancja
{ #c15612}

		* $K(s)=k_{reg}(s)*(1+\frac{1}{sT_{i}}+sT_{d})$
	* W dziedzinie czasu
		* $h(t)=k_{r}*[1+\frac{t}{T_{i}}+T_{d}\delta(t)]$
	* Wzór na sygnał sterujący
		* $y_{ster}(t)=k_{P}\varepsilon(t)+k_{I}\int^t_{0}\varepsilon(t)dt*k_{D}\frac{d\varepsilon(t)}{dt}$
* Podział zadań xD
	* proporcjonalna (P)
		* zależy od aktualnej wartości uchybu
	* całkująca (I)
		* daje reakcję które zależy od wartości uchybu w czasie
	* różniczkująca (D)
{ #b8ed47}

		* daje reakcję od zmian uchybu w najbliższej przyszłości zmian sygnału uchybu
		* różniczkuje, czyli próbuje określić, jaka funkcja opisuje uchyb i na tej podstawie może dobrać *na przyszłość*
* [[10 Notatki/Wskaźniki jakościowe regulatora PID\|Wskaźniki jakościowe regulatora PID]]
* Schemat strukturalny regulatora PID
	* ![Pasted image 20240629144831.png](/img/user/80%20Zasoby/Pasted%20image%2020240629144831.png)

