# 🚔 SASPA Leader Panel & Secure Terminal OS

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Google Apps Script](https://img.shields.io/badge/Google_Apps_Script-4285F4?style=for-the-badge&logo=google&logoColor=white)

Интерактивная веб-панель лидера и защищенный терминал управления личным составом для фракции **SASPA** (GTA 5 RP, сервер RAINBOW). Проект разработан для автоматизации рутины лидера, контроля квот и удобного сбора заявок на старший состав.

---

## 🌟 Основной функционал

### 1. Leader Dashboard (`index.html`)
Визитная карточка лидера Yuma Takimura.
* **Трекинг срока:** Автоматический расчет прошедших и оставшихся дней лидерского срока с визуальным прогресс-баром.
* **Синхронизация квот:** Панель в реальном времени подтягивает данные о свободных местах из Терминала.
* **Система электронных заявок:** Интегрированная форма с кастомным дизайном (включая выбор часового пояса и прайм-тайма). Данные автоматически отправляются в Google Таблицу через веб-хук на Google Apps Script (без перезагрузки страницы).

### 2. Secure Terminal OS (`indexsaspa.html`)
Закрытая база данных для управления ростером фракции.
* **Локальная БД:** Хранение данных о сотрудниках в `localStorage` браузера.
* **Авто-расчет:** Умный алгоритм сам распределяет сотрудников по отделам (A, SPD, HRD, ED, CRUSH, USMS) и считает квоты для Head и D.Head.
* **Импорт/Экспорт:** Возможность выгрузить всю базу в `.txt` отчет или Base64-код, а также импортировать её обратно в один клик.

---

## 📂 Структура проекта

```text
📦 saspa-panel
 ┣ 📜 index.html         # Публичный дашборд и форма заявок
 ┣ 📜 indexsaspa.html    # Закрытый терминал управления ростером
 ┣ 📜 photoosnova.png    # Фотография персонажа
 ┗ 📜 README.md          # Документация проекта
