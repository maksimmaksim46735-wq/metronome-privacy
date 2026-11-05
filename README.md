# Публикация политики конфиденциальности на GitHub Pages

© 2026 max.art

## Что здесь лежит

| Файл | Назначение |
|---|---|
| `index.html` | политика конфиденциальности (RU + EN) — готова к публикации |
| `README.md` | эта инструкция |

## Шаг 1. Создать репозиторий

1. Войдите на [github.com](https://github.com).
2. **New repository** → имя, например `metronome-privacy`.
3. Видимость: **Public** (для бесплатного GitHub Pages).
4. **Create repository**.

## Шаг 2. Загрузить файл

1. В репозитории: **Add file → Upload files**.
2. Перетащите `index.html` из этой папки.
3. **Commit changes**.

Либо через Git:

```bash
git init
git add index.html
git commit -m "privacy policy"
git branch -M main
git remote add origin https://github.com/<ваш-логин>/metronome-privacy.git
git push -u origin main
```

## Шаг 3. Включить GitHub Pages

1. В репозитории: **Settings → Pages**.
2. **Source**: Deploy from a branch.
3. **Branch**: `main`, папка `/ (root)`.
4. **Save**.

Через 1–2 минуты сайт будет доступен по адресу:

```
https://<ваш-логин>.github.io/metronome-privacy/
```

Этот адрес и есть ссылка на политику конфиденциальности — вставьте его в карточку
RuStore и в Google Play Console.

## Проверка

- Страница открывается по HTTPS (GitHub Pages всегда отдаёт HTTPS).
- В политике указаны: отсутствие сбора данных, разрешения Android, оплата через RuStore.

## Если нужен свой домен

**Settings → Pages → Custom domain** → вписать домен и добавить CNAME-запись у регистратора.
GitHub сам выпустит сертификат.
