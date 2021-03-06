SCSI
===

## Wstęp  
Magistrala danych przeznaczona do przesyłania danych między urządzeniami. Każde urządzenie podłączone do SCSI posiada unikatowy adres i może pełnić dwie funkcje : inicjatora(rozpoczynać operację) i celu (wykonywać operację zleconą przez inicjatora). 
Magistrala SCSI pozwala na podłączenie dysku do więcej niż jednego komputera oraz przesyłanie danych bezpośrednio pomiędzy urządzeniami bez ingerencji komputera.
SCSI jest magistralą równoległą do której uczestnicy są podłączeni za pomocą kabla. Magistrala ta jest stosowana już nie tylko w małych komputerach ale także już w większych. Nie jest klasycznym złączem lub połączeniem punkt – punkt. Jest to magistrala przystosowana do pracy wielorasowej.
Każde urządzenie, które jest podłączone do SCSI posiada swój unikatowy w obrębie magistrali adres (SCSI ID). Identyfikator pełni rolę priorytetu przy rozstrzyganiu próby jednoczesnego dostępu więcej niż jednego urządzenia do magistrali. 
## Historia
* 1981 r. – po raz pierwszy zaprezentowano standard SASI (Shugart Associates System Interface). Na nim firma Shugart pracowała od 1979. 
* Od 1982r.  – magistrala przekształca się  w ogólnie obowiązujący standard magistrali z symetrycznymi sterownikami.
* 1986r. – zatwierdzenie pierwszej wersji normy dzisiaj znanej jako SCSI – 1
* 1987r. – pracę nad poszerzenie magistrali z 8 do 32 bitów. 32 – bitowa magistrala jest praktycznie nie spotykana. Wszystkie współczesne warianty SCSI korzystają z 16 – bitowej transmisji równoległej.
* Dziś jeszcze obowiązują normy międzynarodowe ISO/IEC 9316:1995, 2nd Edition (znana jako SCSI-2) oraz ISO 9316:1989, 1st Edition, znana jako SCSI-1. Aktualne są specyfikacje elektryczne SPI-3 i SPI-5 oraz przynależne warianty protokołów (zob. również specyfikacje SCSI).
## Rodzaje SCSI
SCSI występuje w różnych wersjach, które różnią się prędkością i odległością na jakiej może być prowadzona transmisja.

 **SCSI – 1:**  Najstarsza specyfikacja opracowana w 1996 r. Pozwalała na transfer z prędkością 5 MB/s na odległość 6m. 
 
 **SCSI – 2:** Zwiększono liczbę urządzeń którą można podłączyć do 15 . Pojawiło się kolejkowanie poleceń pozwalając urządzeniom na przechowywanie u ustalanie priorytetów poleceń z komputera hosta. Zwiększono transfer w dwóch wersjach : 
* Szybkie SCSI (Fast SCSI) – 10 MB/s 
* Szybkie szerokie SCSI (Wide SCSI) – 20MB\s

 **SCSI – 3:** (Znana jako Ultra SCSI): 
* Fast 20- prędkość transferu od 20 Mb/s
* Ultra szerokie SCSI prędkość do 40 MB/s 
## Właściowości
*	Magistrala wejścia\wyjścia do łączenia komputerów i urządzeń peryferyjnych 
*	Sposób transmisji : asynchroniczny i synchroniczny
*	Różne prędkości transmisji od 5 Mb/s do 640 Mb/s
*	Szerokość magistrali 8 bitów i 16 bitów


| NAZWA   | BITY  | MAX.TRANSF  | MAX.DŁ.KABLA  | PARAMETRY ELEKTRYCZNE  |
|---|---|---|---|---|
| SCSI - 1  | 8 | 5 Mb/s | 6m | SE |
| SCSI - 2 Fast | 8 | 10Mb/s | 3m | SE |
| SCSI - 2 Fast Wide | 16 | 20Mb/s | 3m | SE |
| SCSI - 3 Ultra | 8 | 20Mb/s | 1.5m | SE |
| SCSI - 3 Ultra Wide | 16 | 40Mb/s | 1.5m | SE |
| SCSI - 3 Ultra 2 | 8 | 40Mb/s | 12m | LVD |
| SCSI - 3 Ultra 2 Wide | 16 | 80Mb/s | 12m | LVD |
| SCSI - 3 Ultra 3 | 16 | 160Mb/s | 12m | LVD |
| SCSI - 3 Ultra 4 | 16 | 320Mb/s | 12m | LVD |
| SCSI - 3 Ultra 640 | 16 | 640Mb/s | 12m | LVD |

## Protokół

Protokół SCSI wyróżnia urządzenie inicjujące jako źródło transakcji i urządzenie docelowe jako jej cel. Urządzenie docelowe może składać z więcej niż jednej jednostki logicznej, LUN. Jeżeli nie zostało to inaczej określone, transakcja kierowana jest do jednostki logicznej o najniższym adresie - LUN 0. Jednostką logiczną LUN może być partycja twardego dysku, pojedynczy dysk w macierzy lub inne jednostki logiczne.  SCSI natychmiast po zainicjowaniu akcji cała aktywność na magistrali przechodzi na urządzenie peryferyjne W innych systemach jest z reguły jedno urządzenie nadrzędne i wiele urządzeń podrzędnych, a całością transmisji rządzi komputer lub karta urządzenia nadrzędnego.

## Źródła
[Źródło 1](https://www.pcworld.pl/news/Podstawy-SCSI,305377.html)

[Źródło 2](https://prezi.com/yeedic7mzp1h/temat-rownolega-magistrala-danych-scsi/)

[Źródło 3](http://kaleron.pl/Standard-SCSI.php)

