# 🪑 Desk Setup – Moduł stanowiska komputerowego

Moduł **Desk Setup** odpowiada za automatyzację stanowiska komputerowego w ramach systemu Smart Room. Skupia się na sterowaniu fizycznymi urządzeniami, zdalnym logowaniu oraz obsłudze KVM.

## 📦 Funkcje

- ✅ Włączanie PC i laptopa (zdalne sterowanie przyciskiem POWER)
- ✅ Włączanie i wyłączanie monitorów (poprzez odcinanie zasilania gniazdek)
- ✅ Automatyczne logowanie do komputerów (emulacja klawiatury przez ESP32)
- ✅ Przełączanie wejść KVM (nie zadziała z każdą KVM)

## ⚙️ Zastosowane komponenty

- **ESP32-S2** – sterownik modułu, obsługuje komunikację MQTT i HID przez USB
- **Przekaźniki** – sterowanie zasilaniem monitorów i symulacją przycisków POWER
- **Tranzystory NPN** – do sterowania obwodami niskoprądowymi
- **Przyciski fizyczne** – lokalne sterowanie
- **MQTT** – dwukierunkowa komunikacja z brokerem

## 🧠 Automatyzacje

- uruchomienie PC i laptopa, włączenie monitorów
- wyłączenie monitorów, blokada sesji
- przełączenie KVM na inne źródło
- wpisanie loginu/hasła za pomocą HID

## 🛠️ Konfiguracja

1. Wgraj firmware do ESP32-S2
2. Uruchom broker MQTT i skonfiguruj komunikację
3. Podłącz moduły do MCU
4. Skonfiguruj emulację HID na ESP32-S2 (np. login do Windowsa/Linuxa)

## 🛑 Uwaga prawna

> ⚠️ **Niektóre funkcje mogą wymagać modyfikacji sprzętowej**, np. podłączenia się do przycisków zasilania, portów USB lub obwodów niskonapięciowych. Może to skutkować **utratą gwarancji** oraz – w przypadku błędów – **uszkodzeniem sprzętu**.  
>  
> Autor projektu **nie ponosi odpowiedzialności za ewentualne szkody**.  
>  
> Jeśli nie masz doświadczenia z elektroniką lub nie jesteś pewien, co robisz – **zastanów się dwa razy** lub poproś o pomoc osobę z odpowiednimi umiejętnościami.
