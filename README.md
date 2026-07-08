# Corporate Birthday Tracker Bot 🎂

A Telegram bot designed to automatically track employee birthdays and send morning reminders to HR, complete with generated, personalized greeting texts based on gender and corporate status.

## 🚀 Project Overview
This automation tool helps the HR department maintain corporate culture without manual tracking. Using a background scheduler, the bot reads an employee database (Excel file) every day at 8:00 AM. If a birthday is detected, it automatically parses the employee's name, considers their gender and management status, generates a custom congratulatory message, and sends an alert directly to the HR Telegram chat.

## ⚙️ Tech Stack
* **Language:** Python 3
* **Framework:** `aiogram` (async routing)
* **Task Scheduling:** `apscheduler` (cron jobs)
* **Data Parsing:** `openpyxl` (reading .xlsx databases)
* **Configuration:** `python-dotenv` (secure environment variables)

## 💻 How to run locally:
1. Clone the repository.
2. Rename `.env.example` to `.env` and provide your real Telegram Bot API token and HR Chat ID.
3. Place your `employees.xlsx` file in the root directory.
4. Install dependencies:
   `pip install -r requirements.txt`
5. Run the bot:
   `python birthdaybot.py`

---
*(Russian version below)*

# Корпоративный бот-поздравлятор 🎂

Telegram-бот для автоматического отслеживания дней рождений сотрудников и утренней рассылки напоминаний для HR с готовыми, сгенерированными текстами поздравлений (с учетом пола и должности).

## 🚀 Описание проекта
Инструмент автоматизации, помогающий HR-отделу поддерживать корпоративную культуру без ручного контроля. Бот использует асинхронный планировщик задач для ежедневной проверки локальной базы данных (Excel) в 8:00 утра. При обнаружении именинника скрипт обрезает ФИО до нужного формата, подбирает поздравление из пула (в зависимости от пола и цвета заливки ячейки для руководящего состава) и отправляет готовый шаблон напрямую в чат HR.

## ⚙️ Стек технологий
* **Язык:** Python 3
* **Фреймворк:** `aiogram` (асинхронность)
* **Фоновые задачи:** `apscheduler` (настройка cron-задач)
* **Парсинг данных:** `openpyxl` (чтение .xlsx таблиц)
* **Конфигурация:** `python-dotenv` (безопасное хранение ключей)

* ## 💻 Как запустить локально:
1. Клонируйте репозиторий.
2. Переименуйте файл `.env.example` в `.env` и укажите ваш реальный токен Telegram-бота и ID HR-чата.
3. Поместите ваш файл `employees.xlsx` в корневую папку проекта.
4. Установите зависимости:
   `pip install -r requirements.txt`
5. Запустите бота:
   `python birthdaybot.py`
