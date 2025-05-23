# 🤖 AI Telegram-ассистент: RSS → GPT → Telegram

Этот проект — автоматизация на базе [Make.com (Integromat)](https://www.make.com/), которая превращает новости из RSS-лент в персонализированные посты с изображениями для Telegram-канала. Полностью автоматически и в стиле, задаваемом с помощью GPT.

---

## 🔁 Обзор сценария

Каждый час сценарий:

1. **Проверяет RSS-ленту** на наличие новых публикаций.
2. **Загружает полную статью** по ссылке из RSS.
3. **Извлекает чистый текст** из HTML-страницы.
4. **Использует OpenAI (GPT-4)** для генерации:
   - 📌 Короткого заголовка
   - 🗨️ Комментария от лица автора Telegram-канала
5. **Меняет размер изображения**, полученного из RSS, чтобы оно подходило для Telegram.
6. **Публикует пост** (текст + изображение) напрямую в Telegram-канал через бота.

---

## 📦 Используемые технологии

- [Make.com (Integromat)](https://www.make.com/) — визуальная no-code автоматизация
- [OpenAI GPT-4](https://platform.openai.com/) — генерация текста
- [Telegram Bot API](https://core.telegram.org/bots/api) — публикация в канал
- **RSS + HTTP + HTML Parser** — извлечение и очистка контента статей
- **Image Resize** — обработка изображений под требования Telegram


---

## 💡 Основные особенности

- 🔄 **Полная автоматизация**: сценарий работает каждый час, без ручного участия
- 🎙 **Персонализированный стиль от GPT**: адаптация под нужную аудиторию (мода, коучинг, новости и др.)
- 🖼 **Работа с изображениями**: добавление и автоматическое изменение размера
- ✍️ **"Человеческий" тон**: тексты выглядят как написанные реальным автором

---

## 📍 Примеры применения

| Ниша        | Назначение                                      |
|-------------|--------------------------------------------------|
| Мода        | Публикация новостей с комментариями в стиле     |
| Коучинг     | Поделиться трендами и инсайтами автоматически   |
| Техно/Крипто| Резюме и новости без лишней воды                 |
| Вакансии    | Перевод объявлений в читабельные Telegram-посты |

---

## ⚙️ Логика запуска и обработки

- **Триггер:** автоматический, каждый час
- **Логика изображения:** публикуется только если оно есть и подходит по размеру (через Resize)
- **Логика текста:** генерация контента полностью через GPT

> 📌 _Промпт GPT не публикуется по соображениям конфиденциальности._

---
## [Диаграмма публикации в один канал](https://github.com/MikkiPolo/AI_Telegram_Assistant_RSS_GPT_Telegram/blob/main/diagram_low.png)
## [Диаграмма публикаций в несколько каналов с проверкой на наличие медиа файлов](https://github.com/MikkiPolo/AI_Telegram_Assistant_RSS_GPT_Telegram/blob/main/diagram_hight.png)
## [📲 Пример поста в Telegram](https://github.com/MikkiPolo/AI_Telegram_Assistant_RSS_GPT_Telegram/blob/main/scren%20telegram%20channel.png)
