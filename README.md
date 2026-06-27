# HealthMaster: AI-коуч по питанию

Проект по оптимизации AI-коуча на базе GPT-4o для повышения вовлечения пользователей.

## Структура проекта

```
healthmaster-project/
├── docs/
│   └── TZ.md              # Техническое задание
├── before/
│   ├── prompt.md          # Промпт ДО изменений
│   ├── settings.json      # Настройки ДО
│   └── metrics.json       # Метрики ДО (baseline)
└── after/
    ├── prompt.md          # Промпт ПОСЛЕ изменений
    ├── settings.json      # Настройки ПОСЛЕ
    └── results.md         # Результаты проекта
```

## Краткое описание

### Проблема
- Adoption: 18% (цель ≥50%)
- Return Rate: 17% (цель ≥45%)
- One-and-done: 83% (цель <50%)

### Решение
1. Durable-память для базовых фактов
2. Персональные триггеры вместо mass-рассылки
3. Visibility прогресса в каждом ответе
4. Open loops для возврата пользователей

### Результат
- Adoption: 18% → 42% (+133%)
- Return Rate: 17% → 38% (+124%)
- One-and-done: 83% → 58% (-30%)

## Как использовать

### Для клиента
1. Ознакомьтесь с TZ.md
2. Изучите файлы в before/ (текущее состояние)
3. Изучите файлы в after/ (улучшенное состояние)
4. Сравните результаты в results.md

### Для разработчика
1. Скопируйте промпт из after/prompt.md
2. Примените настройки из after/settings.json
3. Настройте durable-память в coach_trigger_service.py
4. Запустите A/B тест

## Технологии

- GPT-4o (OpenAI API)
- Python (aiogram для триггеров)
- PostgreSQL (durable-память)
- Redis (кэширование сессий)

## Контакты

Telegram: @art_buk2
Email: your@email.com
