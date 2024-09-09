Вот пример README для вашего проекта **Vendomat**:

---

# Vendomat

**Vendomat** — это проект системы для автоматов по продаже товаров, реализованный на C#. Проект демонстрирует создание и управление торговым автоматом, который позволяет пользователям выбирать товары и добавлять средства с использованием различных сценариев и команд.

## Оглавление
- [Описание](#описание)
- [Функциональность](#функциональность)
- [Установка](#установка)
- [Использование](#использование)
- [Структура проекта](#структура-проекта)
- [Технологии](#технологии)
- [Будущие возможности](#будущие-возможности)

## Описание
Vendomat реализует функциональность торгового автомата, поддерживая выбор товаров, добавление монет и банкнот, а также проверку баланса и наличия товара. Проект использует паттерны проектирования для управления сценариями и обработки пользовательского ввода.

## Функциональность
- **Выбор товара**: Позволяет пользователю выбрать товар из доступного списка.
- **Добавление средств**: Поддержка добавления монет и банкнот.
- **Проверка состояния**: Проверка наличия выбранного товара и баланса пользователя.

## Установка
Для установки и запуска проекта:

1. Склонируйте репозиторий:
    ```bash
    git clone https://github.com/AlexScience/vendomat.git
    ```

2. Откройте проект в вашей IDE (например, Visual Studio).

3. Соберите и запустите проект.

## Использование
1. Запустите проект.
2. Введите команду для выбора товара или добавления средств:
   - `item A:1` — для выбора товара.
   - `coin: 10` — для добавления монеты.
   - `banknote: 50` — для добавления банкноты.
3. Следуйте инструкциям на экране.

## Структура проекта

### Основные компоненты

- **`UserInputParser`**: Парсит пользовательский ввод и определяет сценарий на основе введенной команды.
- **`ScenarioRunner`**: Запускает сценарии в зависимости от выбранного действия пользователя.
- **`ProductItemsStorage`**: Хранит информацию о доступных товарах и их количестве.
- **`Commands`**: Содержит регулярные выражения для парсинга команд.

### Сценарии и Шаги

- **`SelectItemScenario`**: Управляет сценарием выбора товара.
- **`CheckProductAvailabilityStep`**: Проверяет наличие товара.
- **`CheckBalanceStep`**: Проверяет баланс пользователя.

### Модели

- **`Vendomat`**: Основной класс для управления процессом работы торгового автомата.
- **`Product`**: Представляет товар с его характеристиками.
- **`Bank`**: Управляет балансом и денежными операциями.

## Технологии
Проект реализован с использованием следующих технологий:
- **Язык программирования**: C#
- **Среда разработки**: .NET

## Будущие возможности
- Расширение функциональности для поддержки дополнительных сценариев.
- Улучшение пользовательского интерфейса и взаимодействия.
- Интеграция с реальными платежными системами.
