# Autonomiczna stacja meteorologiczna z ESP32 i zasilaniem solarnym

**Rodzaj projektu:** Praca inżynierska – Politechnika Łódzka.

**Status projektu:** W trakcie realizacji i testowania.

Projekt autonomicznej stacji meteorologicznej opartej na mikrokontrolerze ESP32, umożliwiającej monitorowanie warunków atmosferycznych, bezprzewodowe przesyłanie danych oraz pracę z wykorzystaniem energii słonecznej.

Urządzenie zostało opracowane w ramach pracy inżynierskiej na kierunku Automatyka i Sterowanie Robotów.

## Główne rozwiązania

- **ESP32** – jednostka sterująca odpowiedzialna za odczyt czujników, przetwarzanie danych i komunikację Wi-Fi.
- **BME280** – pomiar temperatury, wilgotności względnej i ciśnienia atmosferycznego.
- **LTR390** – pomiar natężenia światła i promieniowania UV.
- **AS5600** – magnetyczny czujnik kąta obrotu wykorzystywany do określania kierunku wiatru.
- **Czujnik Halla** – pomiar prędkości obrotowej anemometru w celu wyznaczania prędkości wiatru.
- **Czujnik deszczu** – wykrywanie obecności opadów atmosferycznych.
- **Zasilanie solarne** – możliwość wykorzystania panelu fotowoltaicznego jako źródła energii.
- **Zasilanie akumulatorowe** – magazynowanie energii i zasilanie urządzenia przy ograniczonym nasłonecznieniu.
- **Przetwornice DC/DC** – dostosowanie i stabilizacja napięć zasilających.
- **USB-C** – dodatkowy interfejs zasilania.
- **Wi-Fi** – bezprzewodowa transmisja danych pomiarowych.

## Zasada działania

Centralnym elementem stacji jest mikrokontroler ESP32, który odpowiada za cykliczny odczyt danych z czujników meteorologicznych.

System został zaprojektowany do monitorowania następujących parametrów:

- Temperatury powietrza.
- Wilgotności względnej.
- Ciśnienia atmosferycznego.
- Natężenia światła.
- Promieniowania UV.
- Prędkości i kierunku wiatru.
- Występowania opadów atmosferycznych.

Zebrane dane mają być przesyłane za pośrednictwem sieci Wi-Fi, umożliwiając zdalne monitorowanie warunków pogodowych.

### System zasilania

Projekt zakłada wykorzystanie panelu fotowoltaicznego oraz akumulatorów do zapewnienia możliwie autonomicznej pracy urządzenia.

Układ zasilania obejmuje sekcje odpowiedzialne za przetwarzanie napięcia, ładowanie akumulatora oraz dostarczanie energii do mikrokontrolera i czujników.

## Zakres wykonanych prac

- Opracowanie koncepcji urządzenia.
- Dobór mikrokontrolera i czujników meteorologicznych.
- Projektowanie schematu elektronicznego.
- Opracowanie układów zasilania.
- Projektowanie dedykowanej płytki PCB.
- Integracja interfejsów komunikacyjnych i pomiarowych.
- Programowanie mikrokontrolera ESP32.
- Uruchamianie i testowanie poszczególnych elementów systemu.
- Przygotowanie dokumentacji technicznej.

---

## Wizualizacja 3D płytki PCB

Wizualizacja przedstawia projekt płytki integrującej ESP32, złącza czujników meteorologicznych, układy zasilania oraz interfejsy komunikacyjne.

![Wizualizacja PCB stacji meteorologicznej](<moja INZ.png>)

---

## Informacje o projekcie

Projekt realizowany samodzielnie w ramach pracy inżynierskiej na Politechnice Łódzkiej.

Obecna konstrukcja znajduje się na etapie rozwoju i testowania. Przedstawiona wizualizacja prezentuje projekt PCB, a nie końcowe, w pełni zweryfikowane urządzenie.

**Projektant elektroniki i PCB:** Radek Piątkowski

**Oprogramowanie mikrokontrolera:** Radek Piątkowski

*Pełna dokumentacja techniczna, schematy elektroniczne oraz pliki produkcyjne nie są udostępniane publicznie.*
