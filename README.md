# Daybook

Недельное расписание HU Berlin, зимний семестр 2026/27. Статический сайт: один `index.html` и три картинки, без сборки.

## Локальный запуск

```bash
python3 -m http.server 8000
```

Открыть http://localhost:8000.

## Как изменить расписание

Всё расписание лежит в массиве `DAYS` в `<script>` внутри `index.html`: время, предмет, тип, аудитория, преподаватель. Сетка недели пересчитывается сама.

## Публикация

GitHub Pages: Settings → Pages → Source: Deploy from a branch → `main` / `/ (root)`.
