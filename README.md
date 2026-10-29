# Портфолио Сергея Шостикова / Sergey Shostikov — QA Engineer

Статический сайт (HTML + CSS + JS, без сборки). Языки: RU / EN (переключатель в шапке, выбор запоминается).

```
index.html                 # весь сайт
assets/img/photo.jpg       # фото (можно заменить своим, квадрат от 400×400)
assets/files/*.pdf         # резюме для скачивания
.nojekyll
```

## Размещение на GitHub Pages

1. Зарегистрируйтесь на https://github.com и нажмите **New repository**.
2. Имя репозитория:
   - `ВАШ-ЛОГИН.github.io` — сайт будет по адресу `https://ВАШ-ЛОГИН.github.io/`;
   - или любое другое (например `portfolio`) — адрес будет `https://ВАШ-ЛОГИН.github.io/portfolio/`.
3. Видимость: **Public**. Нажмите **Create repository**.
4. Загрузите файлы: **Add file → Upload files**, перетащите **содержимое** папки (`index.html`, `assets`, `.nojekyll`, `README.md`) и нажмите **Commit changes**.
   Или через терминал:
   ```bash
   git init
   git add .
   git commit -m "Portfolio"
   git branch -M main
   git remote add origin https://github.com/ВАШ-ЛОГИН/ИМЯ-РЕПО.git
   git push -u origin main
   ```
5. В репозитории: **Settings → Pages → Build and deployment**: Source — **Deploy from a branch**, Branch — `main`, папка `/ (root)`, **Save**.
6. Через 1–2 минуты сайт появится по адресу в верхней части страницы Pages.

## Что менять

- Контакты: блок `#contact` в `index.html` (почта и телефон из резюме).
- Тексты и опыт: объекты `D`, `JOBS`, `SK`, `AB`, `ED` в блоке `<script>`.
- Новое резюме: замените PDF в `assets/files/` под тем же именем.
- Добавить GitHub / LinkedIn / Telegram: добавьте ссылку `<a>` в `.links`.
- Свой домен: Settings → Pages → Custom domain.

---

## Deploying to GitHub Pages (short)

Create a public repo (`USERNAME.github.io` for the root URL), upload the folder contents, then Settings → Pages → Deploy from a branch → `main` / `/ (root)` → Save. The site goes live in 1–2 minutes.
