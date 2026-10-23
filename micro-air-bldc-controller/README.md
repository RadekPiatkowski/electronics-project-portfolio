# Micro Air — sterownik dwóch silników BLDC z sygnalizacją RGB

**Klient:** Micro Air  
**Rodzaj projektu:** realizacja komercyjna  
**Zakres:** projekt elektroniki, PCB, układu zasilania oraz sterowania dwoma silnikami BLDC

## Opis projektu

W ramach projektu zaprojektowałem **dwie współpracujące ze sobą płytki PCB**, połączone za pomocą złączy goldpin. Układ służy do sterowania dwoma silnikami BLDC oraz wizualnej prezentacji różnicy ich prędkości obrotowych.

### Płyta zasilająca

Pierwsza płytka pełni funkcję modułu zasilającego oraz wykonawczego.

Układ jest zasilany napięciem **30 V DC** i wykorzystuje dwie przetwornice DC/DC:

- **5 V** — zasilanie części elektronicznej,
- **12 V** — zasilanie części związanej z silnikami BLDC.

Na płytce znajdują się również układy odpowiedzialne za zasilanie silników oraz diody **RGB LED**, które tworzą wizualny wskaźnik różnicy prędkości pomiędzy dwoma napędami.

### Płyta sterująca

Druga płytka stanowi główny sterownik urządzenia.

Układ został oparty na mikrokontrolerze **ATmega**, który odpowiada za:

- sterowanie dwoma silnikami BLDC,
- generowanie sygnałów PWM,
- odczyt sygnałów z czujników Halla,
- pomiar i porównywanie prędkości obrotowych obu silników,
- obliczanie uchybu pomiędzy prędkościami,
- sterowanie sygnalizacją RGB.

Kolor diod informuje o wzajemnej prędkości silników:

- 🔴 **czerwony** — jeden z silników obraca się szybciej względem drugiego,
- 🔵 **niebieski** — różnica prędkości występuje w przeciwnym kierunku,
- 🟢 **zielony** — prędkości obu silników znajdują się w założonym zakresie zgodności.

Pozwala to na szybką wizualną ocenę synchronizacji obu napędów.

## Mój zakres prac

- opracowanie koncepcji elektroniki,
- zaprojektowanie dwóch płytek PCB,
- projekt sekcji zasilania **30 V / 12 V / 5 V**,
- dobór komponentów,
- projekt części sterującej opartej na mikrokontrolerze ATmega,
- sterowanie silnikami BLDC za pomocą PWM,
- obsługa sygnałów z czujników Halla,
- implementacja pomiaru i porównywania prędkości silników,
- sterowanie diodami RGB na podstawie wartości uchybu,
- przygotowanie dokumentacji produkcyjnej,
- uruchomienie i testowanie prototypu,
- wprowadzanie poprawek po testach.

## Wdrożenie

Projekt został wykorzystany **komercyjnie przez klienta i wdrożony do produkcji**.

Na podstawie przygotowanego projektu klient wyprodukował około **300 kompletów płytek PCB**.

Projekt został więc zweryfikowany nie tylko na etapie prototypu, ale również podczas seryjnej produkcji i rzeczywistego użytkowania urządzenia.

## Wizualizacja projektu

*W tym miejscu znajduje się wizualizacja 3D zaprojektowanych płytek PCB.*

## Gotowe płytki

*W tym miejscu znajduje się zdjęcie fizycznie wykonanych płytek.*

## Poufność

Ze względu na komercyjny charakter projektu publikuję wyłącznie **wizualizacje PCB oraz zdjęcia gotowych płytek**.

Schematy elektryczne, pliki produkcyjne, kod źródłowy oraz pozostała dokumentacja techniczna nie są udostępniane publicznie.
