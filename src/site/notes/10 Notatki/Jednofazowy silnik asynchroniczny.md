---
{"dg-publish":true,"permalink":"/10 Notatki/Jednofazowy silnik asynchroniczny/","tags":["wiedza/zettel"]}
---

* ## Start silnika
	* skoro mamy jakby 2 wirujące pola, ale oba w przeciwnych kierunkach, to bez układu startu, silnik nie ruszy (bo z kuli jednego pola działa [[10 Notatki/Siła Lorentza\|Siła Lorentza]] w jedną stronę, a z drugiego pola w drugą stronę)
	* do tego właśnie służy [[10 Notatki/Single Phase Induction Motor, How it works#^c29d60\|uzwojenie dodatkowe (startowe)]] i podłączony do niego kondensator
		* kondensator z jedną częścią uzwojenia tworzy jakby rezonans, zwiększając w tej części chwilowo prąd, który później *oddaje* do drugiego uzwojenia.
		* kondensator ten tworzy ten jakby rezonans z tą częścią uzwojenia, do której końca jest podłączony
		* Jeśli rozpatrzylibyśmy, ze uzwojenie dodatkowe zlokalizowane jest na godz. 3 i 9, a kondensator podłączony jest między fazę a uzwojenie w części 3, to właśnie w tym uzwojeniu (na godz. 3) chwilowo prąd będzie większy, niż w części na godz. 9
		* To inicjuje ruch w zgodnie z kierunkiem wskazówek zegara
	* nie jestem przekonany, czy w 100% dobrze to zagadnienie rozumiem, dlatego temat #to-do/research , tutaj inny filmik na ten temat: https://www.youtube.com/watch?v=pbg_PF6MTwY&ab_channel=RoddyMcNamee