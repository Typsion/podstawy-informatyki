# Topologie Sieci

## Sieci Fizyczne
Sieci fizyczne odnoszą się do fizycznego ułożenia kabli, urządzeń i połączeń. Przykłady:
- **Topologia magistrali** (Bus) : jest to jedna z topologii fizycznych sieci komputerowych charakteryzująca się tym, że wszystkie elementy sieci są podłączone do jednej magistrali.
  - Wady: minimalna odporność na awarie, niska cena sieci, małe koszty produkcji.
  - Zalety: słabe bezpieczeństwo, słaba skalowalność, awaria głównego kabla powoduje unieruchomienie całej domeny kolizyjnej.
  - Gdzie stosowane: głównie stosowana w przypadku prostego ich rozmieszczenia – niewielkie biura lub sale wykładowe (komputerowe).
- **Topologia pierścienia** (Ring): jedna z fizycznych topologii sieci komputerowych.
  - Wady: sygnał krąży tylko w jednym kierunku, dołączenie nowych stacji jest utrudnione, jeśli w pierścieniu jest wiele stacji, wymagane specjalne procedury transmisyjne.
  - Zalety: małe zużycie przewodów, możliwość zastosowania łącz optoelektronicznych, które wymagają bezpośredniego nadawania i odbierania transmitowanych sygnałów.
  - Gdzie stosowane: w sieciach komputerowych, gdzie każde urządzenie jest połączone z dwoma sąsiednimi urządzeniami, tworząc zamknięty pierścień.
- **Topologia gwiazdy** (Star): jest to sposób połączenia urządzeń w sieci komputerowej charakteryzujący się tym, że kable sieciowe od wszystkich urządzeń końcowych zbiegają się w jednym wspólnym punkcie.
  - Wady: gdy awarii ulegnie punkt centralny (koncentrator lub przełącznik), to cała sieć przestaje funkcjonować.
  - Zalety: przejrzystość sieci, awaria komputera peryferyjnego (terminala) nie blokuje sieci, łatwa rozbudowa.
  - Gdzie stosowane: W średnich i dużych sieciach lokalnych, w których pracuje wiele urządzeń (serwerów, komputerów, drukarek).


## Sieci Logiczne
Sieci logiczne opisują sposób przesyłania danych między urządzeniami, niezależnie od fizycznej struktury. Przykłady:
- **Punkt-punkt** (Point-to-Point): jest to protokół komunikacyjny warstwy łącza danych używany przy bezpośrednich połączeniach pomiędzy dwoma węzłami sieci.
  - Wady: Słabe metody uwierzytelniania, przestarzałe szyfrowanie, wymaga funkcji PPTP Passthrough w routerze Z łatwością blokowany przez zapory sieciowe
  - Zalety: Łatwa konfiguracja, duża prędkość, kompatybilność z Windowsem
  - Zastosowanie: używany przy bezpośrednich połączeniach pomiędzy dwoma węzłami sieci. PPP może być również skonfigurowany na interfejsie szeregowym asynchronicznym i synchronicznym. Umożliwia on współdziałanie programów zdalnego dostępu pochodzących od różnych producentów
- **Przekazywanie żetonu** (Token Passing): jest to jedna z deterministycznych metod dostępu do łącza danych (fizycznego medium).
  - Wady: przerwanie medium lub awaria jednego z komputerów powoduje przerwę w działaniu całej sieci, maksymalna predkosc przesylu danych wynosi 16Mb/s, technologia ta jest przestarzala i obsluguje mała liczbe urzadzen
  - Zalety: gwarantuje minimalna predkosc transmisji, ktora jest wieksza od 0.
  - Zastosowanie: Metoda dostępu do sieci, która wykorzystuje charakterystyczną sekwencję znaków jako symbol (token), który jest przekazywany z węzła do węzła, wskazując, kiedy rozpocząć transmisję.
- **Wielodostępowa** (Multiple Access): jest to system współdzielenia medium poprzez przydział odpowiednich częstotliwości. Jest najstarszym i jednocześnie najprostszym rodzajem wielodostępu.
  - Wady: trudności związane ze stabilnością częstotliwości nośnej, wykorzystanie kosztownych filtrów o stromych zboczach do separacji częstotliwościowej użytkowników
  - Zalety: odgrywają znaczącą rolę w poprawie efektywności widmowej i pojemności konkretnego systemu komunikacyjnego, transmisja prowadzona cały czas w tym samym paśmie częstotliwości, przez co jest to najprostsza metoda wielodostępu
  - Zastosowanie: był w pierwszych generacjach analogowych telefonów komórkowych. Znajduje zastosowanie raczej wśród systemów szerokopasmowych.