# Лабораторна робота №1 · Варіант 3

Фізична читальня вигаданої групи «Орбіта-03». Усі імена, навчальна збірка та номери її сторінок умовні. Обидва HTML-документи працюють без CSS та JavaScript.

## Локальний перегляд

Виконайте `python3 -m http.server 8000 --directory site` і відкрийте http://localhost:8000/. Перевірте вибір студента, обмеження курсу від 1 до 6, перехід до розділу книги й розкриття відповіді. Форма передає умовний ідентифікатор студента та курс через GET до розділу завдання. Серверне збереження даних у цій роботі не передбачене.

## Публікація у web-development-tasks

1. У репозиторії відкрийте **Settings → Pages → Build and deployment → Source** та виберіть **GitHub Actions**. Якщо середовище github-pages має обмеження гілок, у **Settings → Environments → github-pages** дозвольте розгортання з гілок за шаблоном `lab-*`.
2. Завантажте ZIP до Downloads. Для нової локальної копії виконайте:

```bash
git clone https://github.com/timofei-kasianov/web-development-tasks.git
cd web-development-tasks
git switch -c lab-01
unzip ~/Downloads/Web_Lab1_Variant3.zip
git add site .github/workflows/pages.yml README.md
git commit -m "Лабораторна 1: HTML, варіант 3"
git push -u origin lab-01
```

3. Дочекайтеся успішного **Actions → Publish laboratory pages**. Адреса роботи після публікації: https://timofei-kasianov.github.io/web-development-tasks/lab-01/
4. Відкрийте https://validator.w3.org/nu/ та перевірте публічні адреси `lab-01/index.html` і `lab-01/reader.html`. Зробіть скріншоти результатів із видимими URL і додайте їх у розділ валідації звіту.

## Наступні лабораторні

Для наступної роботи створіть гілку `lab-02` від `lab-01`, збережіть workflow і замініть вміст каталогу `site/` матеріалами другої роботи. При push у будь-яку гілку виду `lab-01`, `lab-02` тощо workflow збирає останній вміст каталогу `site/` кожної такої гілки в окремий шлях сайту. Коренева адреса містить список робіт. Звіт Word з персональними даними зберігайте окремо від `site/`.
