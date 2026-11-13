# Modułowy system pomiarowy i zarządzania energią – projekt dydaktyczny

Projekt płytki PCB opracowany na indywidualne zamówienie na potrzeby zajęć dydaktycznych dla studentów uczelni technicznej.

Układ stanowi platformę edukacyjną umożliwiającą poznanie zasad działania systemów pomiarowych, zarządzania energią, zasilania akumulatorowego oraz komunikacji mikrokontrolera z modułami elektronicznymi.

## Zasada działania układu

Centralnym elementem systemu jest mikrokontroler **ESP32**, przeznaczony do zbierania i przetwarzania danych z podłączonych modułów.

Układ został zaprojektowany z wykorzystaniem następujących rozwiązań:

- **ESP32** – jednostka sterująca odpowiedzialna za komunikację z modułami i przetwarzanie danych pomiarowych.
- **BME280** – pomiar temperatury, wilgotności względnej oraz ciśnienia atmosferycznego.
- **2 × INA3221** – wielokanałowy pomiar napięcia i prądu w wybranych obwodach elektrycznych.
- **MAX17043** – monitorowanie napięcia i szacowanego poziomu naładowania akumulatora.
- **MCP73871** – zarządzanie ładowaniem akumulatora Li-Ion/Li-Po oraz zasilaniem odbiorników z wykorzystaniem funkcji Power Path.
- **TPS63070** – przetwornica DC/DC typu Buck-Boost umożliwiająca stabilizację napięcia wyjściowego przy zmieniającym się napięciu wejściowym.
- **Wyświetlacz LCD** – możliwość prezentacji danych pomiarowych.
- **Moduł microSD** – możliwość zapisywania wyników pomiarów na karcie pamięci.

### Zarządzanie zasilaniem

Układ MCP73871 umożliwia zasilanie urządzenia z zewnętrznego źródła energii oraz równoczesne ładowanie akumulatora.

W przypadku zaniku zewnętrznego zasilania funkcja Power Path umożliwia przejście na zasilanie akumulatorowe.

Przetwornica TPS63070 odpowiada za stabilizację napięcia, wykorzystując możliwość jego podwyższania lub obniżania w zależności od warunków pracy.

### System pomiarowy

Mikrokontroler ESP32 może odczytywać dane z czujnika BME280, modułów INA3221 oraz układu MAX17043.

Zebrane dane mogą być następnie przetwarzane, prezentowane na wyświetlaczu LCD lub zapisywane na karcie microSD.

Projekt umożliwia studentom zapoznanie się z komunikacją cyfrową, pomiarami elektrycznymi oraz zasadami projektowania systemów wbudowanych.

## Zakres wykonanych prac

- Opracowanie schematu elektronicznego.
- Dobór komponentów i modułów.
- Projektowanie dedykowanej płytki PCB.
- Integracja układów pomiarowych i zasilających.
- Rozmieszczenie komponentów oraz prowadzenie ścieżek.
- Przygotowanie plików produkcyjnych PCB.

---

## 1. Wizualizacja PCB – strona górna

![Wizualizacja PCB – góra](<Wizualizacja PCB – góra.png>)

## 2. Wizualizacja PCB – strona dolna

![Wizualizacja PCB – dół](<Wizualizacja PCB – dół.png>)

---

## Informacje o projekcie

Projekt wykonany na indywidualne zamówienie na potrzeby zajęć dydaktycznych.

Ze względu na prywatność zleceniodawcy nazwa uczelni oraz dane prowadzącego zajęcia nie są ujawniane.

**Projektant elektroniki i PCB:** Radek Piątkowski

*Przedstawione materiały prezentują etap projektowy oraz założoną funkcjonalność urządzenia. Pełna dokumentacja techniczna i pliki produkcyjne nie są udostępniane publicznie.*
