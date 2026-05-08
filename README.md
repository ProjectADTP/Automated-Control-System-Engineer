# Инженер АСУ ТП

## Обо мне

Инженер по автоматизации технологических процессов с практическим опытом разработки систем управления на базе **ПЛК**, **SCADA** и **микроконтроллеров**. Специализируюсь на создании комплексных решений: от проектирования логики в CoDeSys/CX-Programmer до визуализации на HMI и сбора данных в LabVIEW.

**СПбГУТ им. проф. М.А. Бонч-Бруевича**  
Направление: Автоматизация технологических процессов и производств

---

## Технический стек

### Промышленная автоматизация
![PLC](https://img.shields.io/badge/PLC-00599C?style=for-the-badge&logo=siemens&logoColor=white)
![CoDeSys](https://img.shields.io/badge/CoDeSys-00599C?style=for-the-badge)
![Omron](https://img.shields.io/badge/Omron-00599C?style=for-the-badge)
![IEC 61131-3](https://img.shields.io/badge/IEC_61131--3-00599C?style=for-the-badge)

- **ПЛК:** OWEN PLC100, Omron CP1L
- **Языки:** LD, FBD, CFC, ST (IEC 61131-3)
- **HMI:** Kinco MT4434TE (HMIware), SCADA Simplight

### Встраиваемые системы и IoT
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)

- **Платформы:** ESP32, Arduino (ATmega2560), TTGO T9
- **Интерфейсы:** UART, I2C, SPI, PWM, Modbus RTU/TCP
- **Датчики:** MPU9250, LM393, энкодеры

### Визуализация и Сбор Данных
![LabVIEW](https://img.shields.io/badge/LabVIEW-FFDB00?style=for-the-badge&logo=ni&logoColor=black)
![Modbus](https://img.shields.io/badge/Modbus-00599C?style=for-the-badge)
![OPC](https://img.shields.io/badge/OPC-00599C?style=for-the-badge)

- **SCADA:** Simplight, MasterOPC Server
- **DAQ:** NI USB-6008, LabVIEW VISA
- **Протоколы:** Modbus, OPC DA/UA

### Инженерное проектирование
![CAD](https://img.shields.io/badge/CAD-00599C?style=for-the-badge)
![Creo](https://img.shields.io/badge/Creo-00599C?style=for-the-badge)
![Multisim](https://img.shields.io/badge/Multisim-00599C?style=for-the-badge)

- **САПР:** PTC Creo (Schematics, Cabling), Symica (SPICE)
- **Моделирование:** Multisim (цифровая/аналоговая схемотехника)
- **Цифровые двойники:** Концепции DTP/DTI, предиктивная аналитика

### Языки программирования
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![C#](https://img.shields.io/badge/C%23-gray?style=for-the-badge&logo=mysql&logoColor=white)

- **Языки:** Python, C/C++, Structured Text, LD, Pascal Script, C (HMI Macros), C#, SQL
- **Базы данных:** PostgreSQL, MySQL, MS SQL (MasterOPC)

---

## Проекты

### Система управления насосами (OWEN PLC100 + CoDeSys)
- **Задача:** Разработка системы управления двумя насосами с резервированием.
- **Реализация:** 
  - Поочередная и параллельная работа двигателей.
  - Автоматическое переключение при аварии (контроль фаз, таймаут 3с).
  - Языки: **LD, CFC, ST**. Моделирование логики в **Multisim**.
- **Результат:** Отказоустойчивая система с диагностикой неисправностей.

### Игра «Тетрис» на ПЛК + HMI (Omron CP1L + Kinco)
- **Задача:** Создание распределенной системы управления игрой.
- **Реализация:** 
  - **ПЛК (CX-Programmer):** Обработка сигналов с тумблеров (язык **LD**).
  - **HMI (Kinco HMIware):** Графический интерфейс и логика игры на **C Macros**.
  - Обмен данными через память контроллера и панели.
- **Результат:** Демонстрация навыков интеграции ПЛК и панелей оператора.

### Автомат выдачи газет (Multisim + CoDeSys)
- **Задача:** Проектирование логики автомата с приемом монет и выдачей сдачи.
- **Реализация:** 
  - **Multisim:** Цифровая схема на JK-триггерах и логических элементах.
  - **CoDeSys:** Программная реализация на **ST** и **CFC**.
  - Функции: накопление суммы, обмен монет (10 ↔ 2x5), выдача товара.
- **Результат:** Полный цикл от схемотехники до программирования контроллера.

### Управление коллекторным двигателем (Arduino + LabVIEW)
- **Задача:** Создание виртуального прибора для управления двигателем и сбора данных.
- **Реализация:** 
  - **Hardware:** Arduino ATmega2560, драйвер MX 1616, датчик звука LM393.
  - **Software:** LabVIEW (Front Panel, Block Diagram, VISA), Arduino IDE (C++).
  - Функции: PWM управление скоростью, реверс, усреднение показаний датчиков.
- **Результат:** Работающий стенд с визуализацией в реальном времени.

### IoT-платформа на ESP32/TTGO T9
- **Компоненты:** MPU9250 (IMU), WM8978 (Audio), WS2812 (LED), SD-card.
- **Функции:** Чтение IMU, синтез звука, потоковое радио, A2DP, Wi-Fi/Bluetooth.
- **Протоколы:** I2C, SPI, I2S, UART, UDP, MQTT.

### Цифровой двойник учебной аудитории
- **Описание проекта** Разработка архитектуры программно-аппаратного комплекса цифровых двойников для формирования киберфизической среды цифрового университета. Система объединяет физические датчики в аудитории с их виртуальной 3D-копией в реальном времени
- **Задача**
  - Мониторинг параметров среды (температура, освещение, CO₂, присутствие)
  - Визуализация состояния аудитории в Unity 3D
  - Автоматизация управления оборудованием (освещение, техника)
  - Интеграция в единую киберфизическую среду вуза
- **Реализация**
  - **IoT-слой:** Микроконтроллеры ESP32 (C/C++), сбор данных с датчиков, трекинг через BLE-маячки
  - **Backend:** REST API на .NET Framework, база данных MySQL для хранения телеметрии
  - **Клиент:** Unity 3D (C#), 3D-модель аудитории, WebGL-билд для браузерного доступа
  - **Логика:** Онтологии и семантические сети для описания связей между объектами, микросервисная архитектура
**Результат**
  - **Прототип:** Работающий прототип с синхронизацией данных < 1 сек
  - **Управление:** Реализовано зонированное управление освещением (3 зоны)
  - **Трекинг:** Определение присутствия студентов и статуса оборудования
  - **Адаптивность:** Платформа легко масштабируется на офисы, цеха и другие помещения
  - **Интеграция:** Возможность привязки к BIM-моделям зданий

---

## Документации

| Документ | Ссылка |
|----------|--------|
| **Система управления насосами (ОВЕН ПЛК100 + CoDeSys)** | [📄](https://github.com/ProjectADTP/Automated-Control-System-Engineer/blob/main/Система_управления_насосами/Система_управления_насосами.pdf) |
| **Автомат выдачи газет (Multisim + CoDeSys)** | [📄](https://github.com/ProjectADTP/Automated-Control-System-Engineer/blob/main/Автомата_выдачи_газет/Автомат_выдачи_газет.pdf) |
| **Игра «Тетрис» (Omron CP1L + Kinco HMI)** | [📄](https://github.com/ProjectADTP/Automated-Control-System-Engineer/blob/main/Работа_с_ПЛК_OMRON/Работа_с_ПЛК_OMRON.pdf) |
| **Управление коллекторным двигателем (Arduino + LabVIEW)** | [📄](https://github.com/ProjectADTP/Automated-Control-System-Engineer/blob/main/Управление_коллекторным_эллектродвигателем/Управление_коллекторным_эллектродвигателем.pdf) |
| **Плата TTGO T9 TAudio (ESP32)** | [📄](https://github.com/ProjectADTP/Automated-Control-System-Engineer/blob/main/Работа%20с%20платой%20TTGO/Работа%20с%20платой%20TTGO.pdf) |
| **Цифровой двойник учебной аудитории** | [📄](https://github.com/ProjectADTP/Automated-Control-System-Engineer/blob/main/Цифровой%20двойник/Цифровой%20двойник%20учебной%20аудитории.pdf) |

---

## Сертификаты

[![Python](https://img.shields.io/badge/Python%20Basic-blue?style=for-the-badge&logo=python&logoColor=white)](https://stepik.org/cert/3124099)
[![Unity](https://img.shields.io/badge/Unity%20Dev-black?style=for-the-badge&logo=unity&logoColor=white)](https://skrinshoter.ru/sa6LmHJpzEi)
[![Manual Testing](https://img.shields.io/badge/Manual%20Testing-red?style=for-the-badge)](https://stepik.org/cert/3114414)

---

## Контакты

| Способ | Ссылка |
|--------|--------|
| **Email** | [rybalko102@gmail.com](mailto:rybalko102@gmail.com) |
| **Telegram** | [@Umage_s](https://t.me/Umage_s) |
