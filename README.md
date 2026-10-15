# Технологии ИИ в урбанистике

Основа учебного сайта курса «Технологии ИИ в урбанистике» на Quarto для публикации через GitHub Pages. Сведения о преподавателе и учебные материалы пока заменены заготовками.

## Структура

- `index.qmd` — описание курса, преподаватель, оценивание и контакты.
- `lectures.qmd` — список лекций и встроенные презентации.
- `lecture-01.qmd` … `lecture-04.qmd` — заготовки презентаций Reveal.js.
- `start.qmd`, `practice-01.qmd` … `practice-05.qmd`, `project.qmd` — практикум и проект.
- `homework.qmd` — домашнее задание.
- `exam.qmd`, `final-exam.qmd` — экзамен.
- `images/` — папка для ваших изображений.
- `_quarto.yml` — название сайта, навигация и настройки сборки.
- `_brand.yml`, `styles.css`, `custom.css` — оформление сайта и презентаций.
- `custom.yml` — русские подписи интерфейса.
- `.github/workflows/pages.yml` — сборка и публикация на GitHub Pages.

## Локальный просмотр

Установите [Quarto](https://quarto.org/docs/get-started/) версии 1.10.19 или новее, затем выполните:

```sh
quarto preview
```

Команда `quarto render` собирает сайт в `docs/`. Эта папка создаётся автоматически и исключена из нового репозитория.

## Новый репозиторий на GitHub

Создайте пустой репозиторий `ai-technologies-in-urbanism` в своём аккаунте. Для GitHub Pages на бесплатном тарифе выберите публичный репозиторий.

Загрузите подготовленную чистую копию с новой историей Git. Не отправляйте историю исходного проекта: в ней остаются старые материалы.

Из папки нового локального репозитория выполните, заменив `YOUR-LOGIN` своим логином:

```sh
git remote add origin https://github.com/YOUR-LOGIN/ai-technologies-in-urbanism.git
git push -u origin main
```

В GitHub откройте **Settings → Pages → Build and deployment → Source** и выберите **GitHub Actions**. Если первая публикация завершилась до включения Pages, запустите **Actions → Publish course site → Run workflow** повторно.

После успешной публикации сайт будет доступен по адресу `https://YOUR-LOGIN.github.io/ai-technologies-in-urbanism/`.

Дальнейшие изменения в ветке `main` будут публиковаться автоматически. Материалы редактируются в `.qmd`; готовые HTML-файлы править не нужно.

Настройка публикации описана в официальной документации [Quarto](https://quarto.org/docs/publishing/github-pages.html) и [GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages).
