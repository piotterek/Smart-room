# 🪑 Desk Setup – Moduł stanowiska komputerowego

Moduł **Desk Setup** odpowiada za automatyzację stanowiska komputerowego w ramach systemu Smart Room. Skupia się na sterowaniu fizycznymi urządzeniami, zdalnym logowaniu oraz obsłudze KVM.

## 📦 Funkcje

- ✅ Włączanie PC i laptopa (zdalne sterowanie przyciskiem POWER)
- ✅ Włączanie i wyłączanie monitorów (poprzez odcinanie zasilania gniazdek)
- ✅ Automatyczne logowanie do komputerów (emulacja klawiatury przez ESP32)
- ✅ Przełączanie wejść KVM (np. przez IR, przekaźnik lub HID)

## ⚙️ Zastosowane komponenty

- **ESP32-S2** – sterownik modułu, obsługuje komunikację MQTT i HID przez USB
- **Przekaźniki** – sterowanie zasilaniem monitorów i symulacją przycisków POWER
- **Tranzystory NPN/P-MOSFET** – do sterowania obwodami niskoprądowymi
- **Przyciski fizyczne** – lokalne sterowanie (np. ręczne przełączanie KVM)
- **MQTT** – dwukierunkowa komunikacja z brokerem (np. Mosquitto)

## 🧠 Automatyzacje

- `scene/start_work`: uruchomienie PC i laptopa, włączenie monitorów
- `scene/leave_desk`: wyłączenie monitorów, blokada sesji
- `scene/switch_kvm`: przełączenie KVM na inne źródło
- `scene/login_pc`: wpisanie loginu/hasła za pomocą HID

## 🛠️ Konfiguracja

1. Wgraj firmware do ESP32-S2 (kod w `firmware/`)
2. Skonfiguruj komunikację MQTT (tematy w `mqtt_topics.md`)
3. Podłącz przekaźniki i tranzystory do sterowania urządzeniami
4. Skonfiguruj emulację HID na ESP32-S2 (np. login do Windowsa/Linuxa)

## 🛑 Uwaga prawna

> ⚠️ **Niektóre funkcje mogą wymagać modyfikacji sprzętowej**, np. podłączenia się do przycisków zasilania, portów USB lub obwodów niskonapięciowych. Może to skutkować **utratą gwarancji** oraz – w przypadku błędów – **uszkodzeniem sprzętu**.  
>  
> Autor projektu **nie ponosi odpowiedzialności za ewentualne szkody**.  
>  
> Jeśli nie masz doświadczenia z elektroniką lub nie jesteś pewien, co robisz – **zastanów się dwa razy** lub poproś o pomoc osobę z odpowiednimi umiejętnościami.
