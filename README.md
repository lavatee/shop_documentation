# **Интернет-магазин**
---
**Стек**: Микросервисная архитектура, Go, Gin, JWT, WebSockets, gRPC, Protocol Buffers, RabbitMQ, Redis, PostgreSQL, sqlx, GORM, Docker, Docker-compose, Unit Testing, Git, golang-migrate
---

## **Микросервисы**

| Микросервис | Описание |  
|--------|------------| 
| [API-Gateway](https://github.com/lavatee/shop_api_gateway) | Маршрутизирует запросы к микросервисам и хранит в себе всю логику авторизации и аутентификации. Точка входа в приложение | 
| [Микросервис Товаров](https://github.com/lavatee/shop_products) | Хранит в себе логику взаимодействия с товарами |
| [Микросервис Заказов](https://github.com/lavatee/shop_orders) | Хранит в себе логику оформления заказов с паттерном Saga через события RabbitMQ |
| [Микросервис Покупателей](https://github.com/lavatee/shop_customers) | Хранит в себе логику взаимодействия с избранным, корзиной и балансом |
| [Микросервис Отзывов](https://github.com/lavatee/shop_reviews) | Хранит в себе логику, связанную с отзывами товаров |

---

### 🛠 Технологии

| Категория           | Технологии                                                                 |
|---------------------|---------------------------------------------------------------------------|
| **Архитектура**     | Микросервисная архитектура, API Gateway                                   |
| **Язык/Фреймворк**  | Go 1.22, Gin                                                              |
| **API**             | REST (Gin), gRPC, Protocol Buffers                                        |
| **Коммуникация**    | RabbitMQ (асинхронная обработка событий, идемпотентные консьюмеры)  |
| **Базы данных**     | PostgreSQL (реляционные данные), Redis (кэширование), sqlx и gorm (библиотеки), golang-migrate (миграции БД)                                     |
| **Аутентификация**  | JWT (JSON Web Tokens)                                                     |
| **Инфраструктура**  | Docker, Docker-compose  |
| **Тестирование**    | Unit Testing             |

**[.proto-файлы для gRPC](https://github.com/lavatee/shop_protos)**
