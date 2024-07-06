---
{"dg-publish":true,"permalink":"/10 Notatki/Silnik obcowzbudny zasilany z prostownika tyrystorowego/","tags":["wiedza/definicja"]}
---

> układy, zależności, charakterystyki, rodzaje pracy silnika i przekształtnika

* ## Wiadomości ogólne
	* ### Wady i zalety
		* #### Zalety
			* **wysoka sprawność** dzięki wysokiej sprawności przekształtnika tyrystorowego
			* możliwe **płynne sterowanie**
			* dobre **właściwości dynamiczne** napędu
			* możliwe hamowania ze zwrotem energii do sieci
			* rewersja
		* #### Wady
			* odkształcenie prądu w sieci
			* niski współczynnik mocy
			* duże koszty inwestycyjne (silnik DC)
			* problemy eksploatacyjne (komutator)
	* ### Zastosowanie
		* Układ sterowany w wielu aplikacjach przemysłowych ze względu na swoją elastyczność w zakresie regulacji prędkości i momentu obrotowego
	* ### Schemat ogólny
		* ![Pasted image 20240706233558.png](/img/user/80%20Zasoby/Pasted%20image%2020240706233558.png)
* ## Układy zasilania
	* ### [[Prostownik jednofazowy\|Prostownik jednofazowy]]
		* #### Schemat
			* ![Pasted image 20240706233643.png](/img/user/80%20Zasoby/Pasted%20image%2020240706233643.png)
		* Prosty układ stosowany w mniejszych aplikacjach
		* Może być skonfigurowany jako prostownik półfalowy lub pełnookresowy
	* ### [[Prostownik trójfazowy jednokierunkowy\|Prostownik trójfazowy jednokierunkowy]]
		* #### Schemat
			* ![Pasted image 20240706234235.png](/img/user/80%20Zasoby/Pasted%20image%2020240706234235.png)
		* Używany w aplikacjach wymagających większej mocy
		* Zazwyczaj konfiguracja mostkowa (mostek trójfazowy) zapewnia bardziej płynne i stabilne napięcie wyjściowe
	* ### [[Prostownik trójfazowy sześciopulsowy\|Prostownik trójfazowy sześciopulsowy]]
		* ![Pasted image 20240706234421.png](/img/user/80%20Zasoby/Pasted%20image%2020240706234421.png)
* ## Zależności
	* ### Regulacja napięcia zasilania
		* Prędkość silnika obcowzbudnego zależy bezpośrednio od napięcia zasilania uzwojenia twornika
		* [[Prostownik tyrystorowy\|Prostownik tyrystorowy]] umożliwia regulację napięcia wyjściowego przez zmianę kąta zapłonu tyrystorów
	* ### Prąd twornika i moment obrotowy
		* Prąd twornika jest proporcjonalny do momentu obrotowego
		* Zmiana prądu twornika wpływa na moment obrotowy wytwarzany przez silnik
* ## Charakterystyki
	* ### Charakterystyka prędkościowo-momentowa
		* Prędkość obrotowa maleje z wzrostem obciążenia momentowego przy stałym napięciu zasilania
		* Regulacja napięcia zasilania pozwala na zmianę charakterystyki prędkościowej silnik
	* ### Charakterystyka prądowo-napięciowa
		* Zależność prądu twornika od napięcia zasilania pokazuje, jak zmienia się prąd przy różnych napięciach i obciążeniach
* ## Rodzaje pracy silnika
	* ### Praca w otwartej pętli (Open Loop)
		* Napięcie zasilania jest regulowane bez sprzężenia zwrotnego
		* Prędkość i moment obrotowy zależą od ustawienia prostownika i obciążenia
	* ### Praca w zamkniętej pętli (Closed Loop)
		* Używa się sprzężenia zwrotnego, aby kontrolować prędkość lub moment obrotowy
		* Czujniki prędkości lub momentu dostarczają sygnały zwrotne do regulatora, który odpowiednio dostosowuje kąt zapłonu tyrystorów
* ## Rodzaje pracy przekształtnika
	* ### Regulacja fazowa (Phase Control)
		* Regulacja napięcia wyjściowego przez zmianę kąta zapłonu tyrystorów
		* Umożliwia płynna regulację napięcia i prędkość silnika
	* ### Regulacja szerokości impulsu (PWM – Pulse Width Modulation)
		* Alternatywna metoda regulacji, chociaż rzadziej stosowana w prsotownikach tyrystorowych
		* Może być używana w bardziej zaawansowanych układach