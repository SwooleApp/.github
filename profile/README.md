# 🚀 SwooleApp Organization

**High-Performance PHP Applications Based on Swoole Framework**

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![PHP](https://img.shields.io/badge/PHP-7.4%2B-purple.svg)](https://php.net)
[![Swoole](https://img.shields.io/badge/Swoole-4.8%2B-green.svg)](https://swoole.com)

## 📖 About the Project

SwooleApp is a collection of tools and frameworks for building high-performance PHP applications using Swoole. It enables the creation of asynchronous, non-blocking applications with support for background tasks, cyclic jobs, and integration with various databases.

## 🏗️ Organization Structure

### 📦 Core Repositories

#### [SwooleApp](https://github.com/SwooleApp/SwooleApp) - Core Framework
**Powerful Framework for Swoole Development**

- **🔄 Asynchronous Request Processing**
- **🎯 Attribute-Based Controllers**
- **🛡️ Middleware System**
- **📋 State Containers for State Management**
- **⚙️ JSON/ENV Configuration**
- **🔧 Configuration Validation**
- **🎪 Background Tasks Support**
- **⏱️ Cyclic Jobs**

#### [SwooleAppMongoConnection](https://github.com/SwooleApp/SwooleAppMongoConnection) - MongoDB Integration
**Asynchronous MongoDB Client for SwooleApp**

- **🗄️ MongoDB Connection Pool**
- **⚡ Asynchronous CRUD Operations**
- **🔗 UUID Support**
- **📦 Batch Operations**
- **🎛️ Two Connection Modes: Pool and Static**
- **🔐 Flexible Authentication Configuration**

#### [exampleSwooleApp](https://github.com/SwooleApp/exampleSwooleApp) - Usage Examples
**Ready-to-Use Examples and Project Templates**

- **📚 Controller Examples**
- **🔧 Configuration Files**
- **🐳 Docker Configurations**
- **🧪 Cyclic Job Examples**
- **🔄 Background Task Examples**

## ✨ Key Features

### 🚀 High Performance
- Asynchronous, non-blocking architecture
- Efficient resource utilization
- Parallel processing support

### 🛠️ Rich Functionality
- **Attribute-Based Routing**
- **Middleware System with Validation**
- **State Containers for Shared State**
- **Background Tasks and Cyclic Jobs**
- **MongoDB Integration**

### 🔧 Easy to Use
- Clean architecture
- Detailed documentation
- Ready-to-use examples
- Flexible configuration

## 📊 Architecture

```
┌─────────────────────────────────────────┐
│           Swoole HTTP Server            │
├─────────────────────────────────────────┤
│             SwooleApp Core              │
│  ┌─────────────┐  ┌─────────────────┐  │
│  │ Controllers │  │ Middleware      │  │
│  └─────────────┘  └─────────────────┘  │
│  ┌─────────────┐  ┌─────────────────┐  │
│  │ Tasks       │  │ State Containers│  │
│  └─────────────┘  └─────────────────┘  │
├─────────────────────────────────────────┤
│        Database Integrations            │
│  ┌───────────────────────────────────┐  │
│  │    MongoDB Connection Pool        │  │
│  └───────────────────────────────────┘  │
└─────────────────────────────────────────┘
```

## 🚀 Quick Start

- [Example Application with All Entities](https://github.com/SwooleApp/exampleSwooleApp)

### Installing the Core Framework
```bash
composer require sidalex/swoole-app
```

### Installing MongoDB Integration
```bash
composer require swooleapp/swoole-mongo-connection
```

### Creating a Server
```php
// server.php
$http = new Server("0.0.0.0", 9501);
$app = new \Sidalex\SwooleApp\Application($config);
// ... handler setup
$http->start();
```

## 📚 Documentation

### Full documentation is available in the repositories:
- [SwooleApp Documentation](https://github.com/SwooleApp/SwooleApp/blob/master/README.md)
- [MongoDB Integration Documentation](https://github.com/SwooleApp/SwooleAppMongoConnection/blob/master/README.md)
- [Usage Examples](https://github.com/SwooleApp/exampleSwooleApp)

## 🏷️ Versioning

Projects use semantic versioning. Current versions:
- **SwooleApp**: v0.2.6+
- **SwooleAppMongoConnection**: Latest stable
- **exampleSwooleApp**: Examples for the latest version

## 🤝 Contributing

We welcome contributions to the project! Please:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

All projects are distributed under the MIT license. See the [LICENSE](LICENSE) file in each repository for details.

## 👥 Authors

- **SidorkinAlex** - Lead Developer and Maintainer

## 🙏 Support

You can support the project at:  
[https://yoomoney.ru/to/410013242088802](https://yoomoney.ru/to/410013242088802)

## 🔗 Useful Links

- [Official Swoole Website](https://www.swoole.com/)
- [Swoole Documentation](https://wiki.swoole.com/)
- [Composer](https://getcomposer.org/)
- [PHP](https://www.php.net/)

---

**⭐ If you like the project, give it a star on GitHub!**

# 🚀 SwooleApp Organization

**Высокопроизводительные PHP-приложения на базе Swoole Framework**

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![PHP](https://img.shields.io/badge/PHP-7.4%2B-purple.svg)](https://php.net)
[![Swoole](https://img.shields.io/badge/Swoole-4.8%2B-green.svg)](https://swoole.com)

## 📖 О проекте

SwooleApp — это набор инструментов и фреймворков для создания высокопроизводительных PHP-приложений на базе Swoole. Позволяет создавать асинхронные, неблокирующие приложения с поддержкой фоновых задач, циклических заданий и интеграцией с различными базами данных.

## 🏗️ Структура организации

### 📦 Основные репозитории

#### [SwooleApp](https://github.com/SwooleApp/SwooleApp) - Основной фреймворк
**Мощный фреймворк для работы с Swoole**

- **🔄 Асинхронная обработка запросов**
- **🎯 Контроллеры с поддержкой атрибутов**
- **🛡️ Middleware система**
- **📋 State Containers для управления состоянием**
- **⚙️ Конфигурация через JSON/ENV**
- **🔧 Валидация конфигурации**
- **🎪 Поддержка фоновых задач (Tasks)**
- **⏱️ Циклические задания (Cyclic Jobs)**



#### [SwooleAppMongoConnection](https://github.com/SwooleApp/SwooleAppMongoConnection) - MongoDB интеграция
**Асинхронный клиент MongoDB для SwooleApp**

- **🗄️ Пул соединений MongoDB**
- **⚡ Асинхронные CRUD операции**
- **🔗 Поддержка UUID**
- **📦 Пакетные операции**
- **🎛️ Два режима подключения: Pool и Static**
- **🔐 Гибкая конфигурация аутентификации**


#### [exampleSwooleApp](https://github.com/SwooleApp/exampleSwooleApp) - Примеры использования
**Готовые примеры и шаблоны проектов**

- **📚 Примеры контроллеров**
- **🔧 Конфигурационные файлы**
- **🐳 Docker-конфигурации**
- **🧪 Примеры циклических заданий**
- **🔄 Примеры фоновых задач**

## ✨ Ключевые особенности

### 🚀 Высокая производительность
- Асинхронная, неблокирующая архитектура
- Эффективное использование ресурсов
- Поддержка параллельной обработки

### 🛠️ Богатый функционал
- **Маршрутизация на основе атрибутов**
- **Middleware система с валидацией**
- **State Containers для общего состояния**
- **Фоновые задачи и циклические задания**
- **Интеграция с MongoDB**

### 🔧 Простота использования
- Чистая архитектура
- Подробная документация
- Готовые примеры
- Гибкая конфигурация

## 📊 Архитектура

```
┌─────────────────────────────────────────┐
│           Swoole HTTP Server            │
├─────────────────────────────────────────┤
│             SwooleApp Core              │
│  ┌─────────────┐  ┌─────────────────┐  │
│  │ Controllers │  │ Middleware      │  │
│  └─────────────┘  └─────────────────┘  │
│  ┌─────────────┐  ┌─────────────────┐  │
│  │ Tasks       │  │ State Containers│  │
│  └─────────────┘  └─────────────────┘  │
├─────────────────────────────────────────┤
│        Database Integrations            │
│  ┌───────────────────────────────────┐  │
│  │    MongoDB Connection Pool        │  │
│  └───────────────────────────────────┘  │
└─────────────────────────────────────────┘
```

## 🚀 Быстрый старт

- [Пример Приложения со всеми сущностями](https://github.com/SwooleApp/exampleSwooleApp)

### Установка основного фреймворка
```bash
composer require sidalex/swoole-app
```

### Установка MongoDB интеграции
```bash
composer require swooleapp/swoole-mongo-connection
```

### Создание сервера
```php
// server.php
$http = new Server("0.0.0.0", 9501);
$app = new \Sidalex\SwooleApp\Application($config);
// ... настройка обработчиков
$http->start();
```

## 📚 Документация

### Полная документация доступна в репозиториях:
- [Документация SwooleApp](https://github.com/SwooleApp/SwooleApp/blob/master/README.md)
- [Документация MongoDB интеграции](https://github.com/SwooleApp/SwooleAppMongoConnection/blob/master/README.md)
- [Примеры использования](https://github.com/SwooleApp/exampleSwooleApp)

## 🏷️ Версионирование

Проекты используют семантическое версионирование. Актуальные версии:
- **SwooleApp**: v0.2.6+
- **SwooleAppMongoConnection**: Последняя стабильная
- **exampleSwooleApp**: Примеры для последней версии

## 🤝 Вклад в проект

Мы приветствуем вклад в развитие проекта! Пожалуйста:

1. Форкните репозиторий
2. Создайте ветку для новой функции (`git checkout -b feature/amazing-feature`)
3. Сделайте коммит изменений (`git commit -m 'Add amazing feature'`)
4. Запушьте в ветку (`git push origin feature/amazing-feature`)
5. Откройте Pull Request

## 📄 Лицензия

Все проекты распространяются под лицензией MIT. Подробнее см. в файлах [LICENSE](LICENSE) каждого репозитория.

## 👥 Авторы

- **SidorkinAlex** - Основной разработчик и мейнтейнер

## 🙏 Поддержка

Поддержать проект можно по ссылке:  
[https://yoomoney.ru/to/410013242088802](https://yoomoney.ru/to/410013242088802)

## 🔗 Полезные ссылки

- [Официальный сайт Swoole](https://www.swoole.com/)
- [Документация Swoole](https://wiki.swoole.com/)
- [Composer](https://getcomposer.org/)
- [PHP](https://www.php.net/)

---

**⭐ Если вам нравится проект, поставьте звезду на GitHub!**
