# Todo API

REST API для управления задачами. Бэкенд для приложения Taskly.

## Технологии

- Python 3.10+
- Flask 3.0
- SQLite (через SQLAlchemy)

## Установка

```bash
pip install -r requirements.txt
python app.py
```

API будет доступно на http://localhost:5000

## Эндпоинты

| Метод | URL | Описание |
|-------|-----|---------|
| GET | /tasks | Все задачи |
| POST | /tasks | Создать задачу |
| GET | /tasks/:id | Задача по ID |
| PUT | /tasks/:id | Обновить задачу |
| DELETE | /tasks/:id | Удалить задачу |

## Известные проблемы

- При создании задачи без поля `description` API возвращает 500 ошибку.
  Нужно добавить проверку на None. Кирилл обещал пофиксить.
