# Opis projektu.

Celem projektu jest opracowanie programowalnego multiefektu gitarowego, łączącego analogowy tor sygnałowy z zaawansowanym cyfrowym przetwarzaniem dźwięku (DSP). System ma pełnić rolę wszechstronnego procesora audio, który w czasie rzeczywistym moduluje sygnał instrumentu, dając użytkownikowi dostęp do konfigurowalnych łańcuchów efektów i odciążając go z konieczności obsługi wielu fizycznych kostek analogowych.

Do akwizycji i modyfikacji sygnału planowane jest wykorzystanie mikrokontrolera współpracującego z zewnętrznymi przetwornikami ADC/DAC po magistrali I2S oraz odpowiednio dopasowanego, analogowego preampu wejściowego. Narzędzie ma cyfryzować dźwięk instrumentu, aplikować wybrane algorytmy matematyczne (filtry, opóźnienia, modulacje) i interpretować polecenia sterujące przekazywane przez interfejs sceniczny w locie, zachowując minimalną latencję.

Zakładane jest podejście iteracyjne, w ramach pracy planowane jest przeprowadzenie eksperymentów dla różnych topologii przetwarzania sygnału (z wykorzystaniem systemów czasu rzeczywistego RTOS), z możliwym ograniczeniem początkowego zakresu do wybranej puli efektów demonstracyjnych oraz bazowej komunikacji bezprzewodowej.

Zagadnienia wymagające doprecyzowania to:

- Dobór optymalnych parametrów analogowego bufora wejściowego oraz układów konwersji audio w celu maksymalizacji dynamiki sygnału

- Architektura oprogramowania DSP i mechanizm bezstratnego przełączania pomiędzy zapisanymi presetami brzmień

- Sposób interakcji fizycznej (np. dobór enkoderów obrotowych, footswitchy i ekranu do podglądu parametrów)

- Forma zewnętrznego interfejsu konfiguracyjnego (np. aplikacja mobilna po Bluetooth lub panel webowy) do wizualnego układania i zapisywania łańcuchów sygnałowych
