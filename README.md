# Daybook

A weekly class timetable that lives in your browser. Import an `.ics` calendar file from your university, then edit class names, teachers and rooms. Interface in English, Deutsch and Русский.

**Live:** https://stepan-botarev.github.io/daybook/

## How it works

- No server and no accounts to sign up for. A profile is a name stored in the browser's `localStorage` on the user's own device. The site owner cannot see anyone's timetable.
- `.ics` import is parsed in the browser. Weekly repeats, every-2-weeks repeats, `EXDATE`, `UNTIL`/`COUNT`, UTC times, cancelled and all-day events are handled. Separate events with the same title, weekday and time are merged into one weekly class.
- Each class can be edited (name, teacher, room, type, day, time, repeat) or deleted. Classes can also be added by hand.
- Several profiles on one device. "Download backup" saves a profile as a `.json` file; "Restore from backup" loads it on another device.

## Files

- `index.html`: the whole app (HTML, CSS, JavaScript)
- `favicon.svg`: browser icon
- `berlin.png`, `paris.png`, `london.png`, `bridge.png`: pictures under each day

## Run locally

```bash
python3 -m http.server 8000
```

Open http://localhost:8000.

## Publish

GitHub Pages: Settings → Pages → Deploy from a branch → `main` / `/ (root)`.

---

**RU.** Недельное расписание, которое хранится в браузере. Загрузи `.ics` из календаря университета, поправь названия, преподавателей и аудитории. Данные остаются на устройстве, у владельца сайта к ним доступа нет.
