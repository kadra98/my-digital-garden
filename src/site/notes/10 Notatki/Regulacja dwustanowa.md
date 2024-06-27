---
{"dg-publish":true,"permalink":"/10 Notatki/Regulacja dwustanowa/","tags":["wiedza/definicja"]}
---

>Ogólna charakterystyka, przebiegi regulacji z histerezą i bez histerezy
   Podstawowe parametry (w celu przygotowania się przestudiować instrukcję i sprawozdanie z ćwiczenia RDW)
   
* ### Ogólna zasada działania
	* Działa na zasadzie:
		* załącz-wyłącz
	* Charakterystyki
		* ![Pasted image 20240625194352.png](/img/user/80%20Zasoby/Pasted%20image%2020240625194352.png)
	* Rozróżnia się układu
			* z histerezą
			* bez histerezy
		* brak histerezy zwiększa częstotliwość działania tego załącz wyłącz, co może szkodzić
				* np. ten klekotający stycznik
			* ale dzięki temu podwójna amplituda jest mniejsza
		* zastosowanie histerezy odwrotnie:
			* zmniejsza częstotliwość
			* zwiększa podwójną amplitudę
	* Wartość średnia nie jest równa wielkości zadanej, ze względu na niesymetryczność:
		* ![Pasted image 20240625194507.png](/img/user/80%20Zasoby/Pasted%20image%2020240625194507.png)

* ### Regulacja dwustanowa z korekcją dynamiczną
	* Istnieje także regulacja dwustanowa z regulacją dynamiczną
		* to wpięcie regulatora PD [[10 Notatki/Sposoby połączeń elementów w UAR#^90704a\|kaskadowo]] lub w [[10 Notatki/Sposoby połączeń elementów w UAR#^342e8d\|pętli sprzężenia zwrotnego]]
			* D – żeby przewidział ;-), patrz [[10 Notatki/Regulator PID#^b8ed47\|Regulator PID#^b8ed47]]
	* głównie zastosowanie, gdzie wymagane jest utrzymywanie parametrów w wąskim zakresie lub w dynamicznie zmieniających się warunkach pracy
	* zalety regulacji z korekcją:
		* redukcja przeregulowania i oscylacji
			* oszczędność energii
		* szybsza reakcja na zmiany
		* precyzyjniejsze utrzymywanie wartości zadanej
		* zmniejsza liczbę cykli włączenia i wyłączenia