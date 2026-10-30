# Satis · Портфолио

Статический сайт-портфолио фриланс-разработчика (парсинг, боты, автоматизация).

- **Стек:** чистый HTML/CSS/JS, без сборщика
- **Темы:** 4 темы × светлый/тёмный = 8 образов. Переключатель — круглый FAB-кнопка внизу справа. Выбор сохраняется в localStorage.
- **Деплой:** GitHub Pages

## Темы

| Тема | Светлая | Тёмная | Характер |
|---|---|---|---|
| **Minimal** | `minimal-light` | `minimal-dark` | Ахроматичный Vercel-стиль, Geist |
| **Prism** | `prism-light` | `prism-dark` | Фиолетовые градиенты, как у Stripe |
| **Ember** | `ember-light` | `ember-dark` | Тёплый терракот, серифные заголовки (Lora) |
| **Forest** | `forest-light` | `forest-dark` | Изумрудный, как у Supabase |

Тема задаётся атрибутом `data-theme` на `<html>`, например `data-theme="minimal-dark"`.
Чтобы зафиксировать тему по умолчанию — укажите её в теге `<html>` (сейчас `minimal-light`).

## Структура

```
index.html            — разметка + переключатель + логика
css/base.css          — базовые стили: переменные, типографика, layout
css/components.css    — компоненты: карточки, кнопки, переключатель
css/palettes-a.css    — палитры Minimal + Prism (свет/тём)
css/palettes-b.css    — палитры Ember + Forest (свет/тём)
```

## Локально

```bash
python -m http.server 8000
# открыть http://localhost:8000
```

## Публикация

```bash
git add .
git commit -m "update"
git push origin main
```

Сайт: https://fsatis.github.io/portfolio/
