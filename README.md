# Zegar czasu bazujący na mikrokontrolerzee ESP-WROOM-32(ESP32 DEVKIT V1) z obsługą 3 motywów wizualnych.

> [!WARNING]
> Kod wykorzystuje biblioteki zewnętrzne, przed urzyciem upewnij się że wykorzystanie tych bibliotek jest wporządku w twoim projekcie.
> Projekt korzysta z następujących bibliotek każda z nich jest licencjonowana oddzielnie:
> - **WiFi.h**, **time.h**, **SPI.h**: (zobacz plik LICENSE)
> - **Adafruit GFX**: (zobacz plik LICENSE)
> - **Adafruit ST7789**: (zobacz plik LICENSE)

## Połączenie z WI-FI:
utwórz punkt dostępu SSID: `ESP32-AP` Hasło: `12345678` 

## Zasada działania:
- ESP łączy się z tempus1.gum.gov.pl lub tempus2.gum.gov.pl ("https://www.gum.gov.pl/pl/dla-biznesu/uslugi/zegar/524,Zegar.html");
- Pobiera dane do zmiennych a następnie ropoczyna lokalne odliczanie bez udziału serweru i wi-fi;
- 
> [!TIP]
> Jeśli zegar po podłączeniu do internetu zaczyna odliczać od 0 oznacza że serwer odmówił udzielenia informacji, wystarczy zresetować esp przyciskiem `EN`;
-
