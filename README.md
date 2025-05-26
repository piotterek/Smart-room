# 🧠 Smart Room – System Automatyzacji Pokoju

**Smart Room** to projekt inteligentnego pomieszczenia zbudowany w ramach mojego homelabu. Wykorzystuje mikrokontrolery ESP32, czujniki, przekaźniki, syntezatory mowy i inne elementy smart home. Wszystko oparte na otwartym oprogramowaniu.

## 🎯 Cel projektu

Zautomatyzować kluczowe funkcje pokoju (oświetlenie, powiadomienia, monitoring) w sposób tani, niezawodny i rozwojowy. Projekt służy zarówno jako praktyczne rozwiązanie, jak i poligon doświadczalny.

## 🔍 Moduły systemu

Każdy moduł jest opisany w osobnym katalogu z własnym `README.md`:

| Moduł                          | Opis                                              |
|--------------------------------|---------------------------------------------------|
| [Desk setup](Desk_setup)                 | Zarządzanie stanowiskiem komputerowym       |

## ⚙️ Technologie

- Mikrokontrolery ESP (programowany w C++ z wykorzystaniem Arduino)
- MQTT (Mosquitto)
- Node-RED (logika automatyzacji, reakcje na zdarzenia)
- Kuma Uptime (monitoring dostępności modułów i usług)

## 🚀 Status

Projekt aktywnie rozwijany. Moduły wdrażane etapami.

## 🛡️ Licencja

MIT – możesz używać, modyfikować i rozwijać dalej.

---

🛠️ Szczegółowe instrukcje znajdziesz w katalogach poszczególnych modułów!

---

## 🛑 Uwaga prawna

> ⚠️ **Niektóre funkcje mogą wymagać modyfikacji sprzętowej**, np. podłączenia się do przycisków zasilania, portów USB lub obwodów niskonapięciowych. Może to skutkować **utratą gwarancji** oraz – w przypadku błędów – **uszkodzeniem sprzętu**.  
>  
> Autor projektu **nie ponosi odpowiedzialności za ewentualne szkody**.  
>  
> Jeśli nie masz doświadczenia z elektroniką lub nie jesteś pewien, co robisz – **zastanów się dwa razy** lub poproś o pomoc osobę z odpowiednimi umiejętnościami.
