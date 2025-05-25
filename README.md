# 🧠 Smart Room – System Automatyzacji Pokoju

**Smart Room** to projekt inteligentnego pomieszczenia zbudowany w ramach mojego homelabu. Wykorzystuje mikrokontrolery ESP32, czujniki, przekaźniki, syntezatory mowy i inne elementy smart home. Wszystko oparte na otwartym oprogramowaniu.

## 🎯 Cel projektu

Zautomatyzować kluczowe funkcje pokoju (oświetlenie, powiadomienia, monitoring) w sposób tani, niezawodny i rozwojowy. Projekt służy zarówno jako praktyczne rozwiązanie, jak i poligon doświadczalny.

## 🔍 Moduły systemu

Każdy moduł jest opisany w osobnym katalogu z własnym `README.md`:

| Moduł                          | Opis                                              |
|--------------------------------|---------------------------------------------------|
| [LED Lighting](modules/led-lighting)                 | Oświetlenie LED, czujnik ruchu, tryby nocne       |
| [ESP32 Desk Controller](modules/esp32-desk-controller) | Przycisk pod biurkiem sterujący scenami           |
| [Voice Alerts](modules/voice-alerts)                 | Powiadomienia głosowe przez ESP32/głośnik         |
| [Temperature Monitor](modules/temperature-monitor)   | Pomiar temperatury i wilgotności, raportowanie    |
| [Etc](modules/etc)                                   | Inne, eksperymentalne funkcje i dodatki           |

## ⚙️ Technologie

- ESP32 (programowany w C++ z wykorzystaniem Arduino)
- MQTT (Mosquitto)
- Node-RED (logika automatyzacji, reakcje na zdarzenia)
- Kuma Uptime (monitoring dostępności modułów i usług)

## 🚀 Status

Projekt aktywnie rozwijany. Moduły wdrażane etapami.

## 🛡️ Licencja

MIT – możesz używać, modyfikować i rozwijać dalej.

---

🛠️ Szczegółowe instrukcje znajdziesz w katalogach poszczególnych modułów!
