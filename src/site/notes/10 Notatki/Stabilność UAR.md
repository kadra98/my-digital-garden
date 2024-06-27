---
{"dg-publish":true,"permalink":"/10 Notatki/Stabilność UAR/","tags":["wiedza/definicja"]}
---

> Definicja i kryteria stabilności UAR (na podstawie wykładu)

* [[10 Notatki/UAR\|UAR]] będzie stabilny, jeśli po wytrąceniu go z równowagi, sam powróci do równowagi
	* Oscylacje nierosnące także są uznawane za n równowagi
		* lub naukowo:
		* *Liniowy układ regulacji automatycznej jest stabilny, jeśli jego odpowiedź na wymuszenie o ograniczonej wartości jest ograniczone*
* Stabilność UAR jest warunkiem koniecznym i niezbędnym do prawidłowej pracy układu
* Nie zależy od wymuszenia, ale zależy od położenia miejsc zerowych mianownika transmitancji w układzie {Im-Reg}
	* Równanie jest prawdziwe, jeśli jego składniki leżą w lewej półpłaszczyźnie zespolonej
* [[10 Notatki/Kryteria stabilności UAR\|Kryteria stabilności UAR]]
	* Kryterium Hurwitza
		* dla układów [[10 Notatki/Układy sterujące a regulacji\|Układy sterujące a regulacji]]
		* polega na wyznaczeniu transmitancji układu
				* człony w mianowniku musza być dodatnie
				* iloczyn środkowych składników - iloczyn skrajnych składników musi być większy od 0
			* $K_{z}(s)=\frac{k}{a_{3}s^3+a_{2}s^2+a_{1}s+a_{0}}$
				1. $a_{3}>0; a_{2}>0; a_{1}>0; a_{0}>0$
				2. $\Delta a_{2}a_{1}-a_{3}a_{0}>0$
	* Kryterium Nyquista
		* dla układów [[10 Notatki/Układy sterujące a regulacji\|Układy sterujące a regulacji]] ze [[10 Notatki/Sposoby połączeń elementów w UAR#^342e8d\|sprzężeniem zwrotnym ujemnym]]