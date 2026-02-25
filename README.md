# Proyecto: Ingeniería Inversa y Control Local - Lydsto G1

Este proyecto documenta el proceso de toma de control local de un robot aspirador Lydsto G1, eliminando la dependencia de la nube del fabricante mediante la intervención de hardware y la actualización de firmware.

## 📊 Especificaciones del Hardware
* **Modelo:** YM-G1-B01 (Fabricante: Yimu)
* **Potencia:** 40W / 14.4V
* **Chipset Wi-Fi:** Beken BK7231N (Ecosistema Zhimi/Xiaomi)

## 🛠 Hallazgos de Ingeniería Inversa
### Reconocimiento de Red
* **SSID de fábrica:** `zhimi-vacuu..._mibtD9CA`
* **Dirección MAC:** `de:ed:83:54:d9:ca`
* **IP del Robot:** `10.10.1.1`

### Interfaz Física (UART)
Se han identificado los siguientes Test Pads en la PCB para comunicación serial:
* **V**: VCC (3.3V)
* **R**: RX (Recepción)
* **T**: TX (Transmisión)
* **G**: GND (Tierra)

## 🚀 Próximos Pasos
1. Conexión física mediante Arduino Uno (Bypass mode).
2. Extracción del Token de seguridad local.
3. Flasheo de firmware libre (OpenBeken).
