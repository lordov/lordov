<br clear="both">

<div align="center">
  <img height="300" width="600" src="https://user-images.githubusercontent.com/74038190/225813708-98b745f2-7d22-48cf-9150-083f1b00d6c9.gif"  />
</div>

<h1 align="center">Привет 👋 Меня зовут Святослав!</h1>

<div align="center">
  <a href="https://t.me/Lordovat" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Telegram&logo=telegram&label=&color=2CA5E0&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="telegram logo" />
  </a>
</div>

###

<h3 align="left">👨‍💻 Обо мне</h3>

<p align="left">
Я backend-разработчик на Python. Занимаюсь разработкой API, Telegram-ботов, интеграциями с внешними сервисами, автоматизацией бизнес-процессов и построением систем с фоновой обработкой задач, очередями сообщений и хранением данных.
</p>

<p align="left">
Мой путь в IT начался в 2023 году после курсов IBA Group. Сейчас я развиваюсь в backend-разработке, микросервисной архитектуре, асинхронном Python, DevOps-практиках и Data Engineering.
</p>

## 🔧 Что я делаю

- Разрабатываю backend-сервисы на **FastAPI**, **Django** и **Django REST Framework**.
- Создаю Telegram-ботов на **aiogram 3** и **aiogram-dialog**.
- Проектирую REST API, административные панели, сервисный слой и бизнес-логику.
- Работаю с **PostgreSQL**, **MySQL**, **SQLAlchemy Async**, **Django ORM** и миграциями через **Alembic/Django migrations**.
- Настраиваю фоновые задачи и планировщики через **Celery**, **Taskiq**, **APScheduler**, **aiocron**.
- Использую **Redis** для FSM, кэша, временных состояний и очередей.
- Работаю с event-driven подходом через **NATS**, **NATS JetStream**, **FastStream**.
- Интегрирую внешние API: **Wildberries**, **Ozon**, **МойСклад**, **Digiseller**, **DesslyHub**, Steam-related API, NewsAPI.
- Автоматизирую сбор, обработку и сохранение данных по продажам, заказам, остаткам, рекламным кампаниям и финансовым отчетам.
- Реализую авторизацию, роли, permissions, JWT, хранение и шифрование API-ключей.
- Настраиваю контейнеризацию через **Docker** и **docker-compose**.
- Работаю с логированием, мониторингом и надежностью: **structlog**, Prometheus, Grafana, обработка ошибок внешних API.

## 🛠 Мой backend-стек

- **Язык:** Python 3.12
- **Backend:** FastAPI, Django, Django REST Framework, ADRF
- **Telegram:** aiogram 3, aiogram-dialog, Fluentogram
- **Базы данных:** PostgreSQL, MySQL, SQLite, SQLAlchemy 2.0, Django ORM, Alembic
- **Очереди и задачи:** Celery, Taskiq, NATS JetStream, FastStream, APScheduler
- **Кэш и состояния:** Redis, django-redis
- **Валидация:** Pydantic, DRF Serializers
- **Интеграции:** aiohttp, requests, Wildberries API, Ozon API, МойСклад API, Digiseller API, DesslyHub API, NewsAPI
- **Данные и отчеты:** pandas, openpyxl, CSV/Excel processing
- **Безопасность:** JWT, SimpleJWT, bcrypt, passlib, Fernet, encrypted API keys
- **Инфраструктура:** Docker, docker-compose, Nginx, Gunicorn, Uvicorn
- **Мониторинг и логи:** structlog, Prometheus, Grafana
- **Качество кода:** Ruff, mypy
## 🚀 Проекты и опыт

### 🎁 Steam Gift Automation

Backend-сервис для автоматизации Steam Gift-заказов.

- FastAPI backend с асинхронной архитектурой.
- Интеграция с Digiseller для проверки оплат и товаров.
- Интеграция с DesslyHub для отправки Steam Gift и проверки транзакций.
- Синхронизация игр, товаров, регионов и цен.
- NATS/FastStream уведомления о статусах заказов.
- Redis-кэширование повторных уведомлений.
- Taskiq scheduler/worker для фоновых синхронизаций.
- SQLAlchemy Async, Alembic, PostgreSQL, Docker Compose.

### 👥 HR Service

Django/DRF backend для управления сотрудниками и HR-процессами.

- REST API для сотрудников, профилей, рабочих мест и специализаций.
- JWT-аутентификация через SimpleJWT.
- Ролевая логика и permissions для сотрудников, руководителей и администраторов.
- Кэширование списков и карточек сотрудников через Redis.
- Согласование изменений профиля: draft, approve, reject.
- Email-уведомления через Celery.
- Импорт сотрудников из CSV в фоне.
- Интеграция с микросервисом кодовых фраз.
- Интеграция с survey-сервисом через NATS/JetStream.
- Интеграция с NewsAPI.

### 📊 Marketplace Analytics / WB_SOFT

Сервис автоматизации аналитики и сбора данных по маркетплейсам.

- Интеграции с **Wildberries**, **Ozon** и **МойСклад**.
- Сбор заказов, продаж, остатков, поставок, тарифов, рекламных кампаний и отчетов.
- Обработка больших периодов через чанки и лимиты API.
- Загрузка и обработка Excel/CSV-отчетов через pandas/openpyxl.
- Pydantic-схемы для валидации данных API.
- SQLAlchemy, Alembic, MySQL/PostgreSQL.
- Telegram-уведомления о заказах.
- Планировщики задач для регулярной синхронизации.
- Работа с рекламной статистикой, воронкой продаж, реализациями и финансовыми отчетами.

### 🔔 WB Vision Bot / WB Notification

Telegram-бот для уведомлений по Wildberries.

- Подключение пользовательских API-ключей Wildberries.
- Шифрование API-ключей через Fernet.
- Автоматические уведомления о новых заказах.
- Поддержка сотрудников, которые получают уведомления владельца.
- Предзагрузка заказов и остатков.
- Фоновые задачи через Taskiq + NATS JetStream.
- Контроль зависших и повторяющихся задач.
- Unit of Work + Repository pattern.
- Redis FSM, aiogram-dialog, Fluent/Fluentogram.
- Prometheus/Grafana для мониторинга.
- Docker Compose окружение.

### 🔐 Authentication Bot

Telegram-бот для выдачи и контроля аккаунтов/кодов доступа.

- aiogram 3 и aiogram-dialog.
- PostgreSQL/SQLite, SQLAlchemy, Alembic.
- Redis FSM с fallback на MemoryStorage.
- Мультиязычность через Fluentogram.
- NATS-интеграции для уведомлений и broadcast-сценариев.
- Работа с аккаунтами, секретными словами, лимитами использования и сроками действия.
- Шифрование чувствительных данных.
- Админские сценарии, поддержка пользователей, рассылки.
- Интеграция с Digiseller-данными.
- Плановые отчеты и уведомления через scheduler.

## 🎯 Мои цели

- Развиваться как **Backend Engineer** на Python.
- Глубже изучать микросервисную и event-driven архитектуру.
- Улучшать навыки проектирования надежных API и интеграций с внешними сервисами.
- Прокачивать DevOps-практики: Docker, CI/CD, мониторинг, production-ready конфигурации.
- Писать чистый, типизированный и поддерживаемый backend-код.

###

<h3 align="left">🔥 Моя статистика:</h3>

<div align="center">
  <table>
    <tr>
      <td>
        <img src="https://streak-stats.demolab.com?user=lordov&locale=en&mode=daily&theme=dark&hide_border=false&border_radius=5&order=3" height="220" alt="streak graph" />
      </td>
      <td>
        <img src="https://github-readme-stats.vercel.app/api/top-langs?username=lordov&locale=en&hide_title=false&layout=compact&card_width=320&langs_count=5&theme=dracula&hide_border=false&order=2" height="150" alt="languages graph" />
      </td>
    </tr>
  </table>
</div>
