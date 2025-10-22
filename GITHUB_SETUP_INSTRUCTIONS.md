# 📋 Інструкція з налаштування GitHub

## ✅ Що вже зроблено:

1. ✓ Ініціалізовано Git репозиторій
2. ✓ Створено 6 комітів:
   - `feat: add table with different cell heights (table1.html)`
   - `feat: add table with nested child table structure (table2.html)`
   - `feat: add Mondrian-style artistic table (table3.html)`
   - `style: add shared CSS styles for all tables`
   - `feat: add main landing page with navigation (index.html)`
   - `docs: add comprehensive README with project documentation`

## 🚀 Наступні кроки для вас:

### Крок 1: Створення репозиторію на GitHub

1. Перейдіть на [GitHub](https://github.com)
2. Натисніть на "+" у верхньому правому куті
3. Виберіть "New repository"
4. Заповніть форму:
   - **Repository name**: `LEK5-7`
   - **Description**: "HTML Tables Project - Навчальний проєкт з таблицями"
   - **Visibility**: Public (щоб використати GitHub Pages)
   - **НЕ вибирайте** "Initialize this repository with a README" (у вас вже є README)
5. Натисніть "Create repository"

### Крок 2: Підключення віддаленого репозиторію

Виконайте наступну команду для підключення вашого GitHub репозиторію:

```bash
git remote add origin https://github.com/veprelax/LEK5-7.git
```

### Крок 3: Перевірка віддаленого репозиторію

```bash
git remote -v
```

Ви повинні побачити:
```
origin  https://github.com/veprelax/LEK5-7.git (fetch)
origin  https://github.com/veprelax/LEK5-7.git (push)
```

### Крок 4: Запуш коду на GitHub

```bash
git push -u origin master
```

або якщо GitHub використовує `main` як головну гілку:

```bash
git branch -M main
git push -u origin main
```

**Примітка**: GitHub може попросити вас авторизуватися. Використовуйте Personal Access Token замість пароля.

### Крок 5: Активація GitHub Pages

1. Перейдіть у ваш репозиторій на GitHub
2. Натисніть на "Settings" (Налаштування)
3. У лівому меню знайдіть "Pages"
4. У розділі "Source" виберіть:
   - Branch: `master` (або `main`)
   - Folder: `/ (root)`
5. Натисніть "Save"
6. Зачекайте 1-2 хвилини
7. GitHub покаже посилання на вашу сторінку: `https://veprelax.github.io/LEK5-7/`

### Крок 6: Перевірка сторінки

Відкрийте посилання GitHub Pages у браузері. Ви повинні побачити вашу головну сторінку з трьома картками таблиць.

## 📝 Використання GitHub Issues

### Створення Issue:

1. У вашому репозиторії натисніть на вкладку "Issues"
2. Натисніть "New issue"
3. Введіть заголовок та опис
4. Приклади Issues:

**Issue 1: Покращення дизайну**
```
Заголовок: Покращити адаптивність для мобільних пристроїв
Опис: Додати media queries для екранів менше 480px
Labels: enhancement
```

**Issue 2: Нова функція**
```
Заголовок: Додати темну тему
Опис: Реалізувати перемикач між світлою та темною темою
Labels: enhancement, feature
```

**Issue 3: Виправлення помилки**
```
Заголовок: Виправити відображення таблиці в Safari
Опис: Таблиця Мондріана некоректно відображається в Safari
Labels: bug
```

## 🎯 Фінальне завдання

Після виконання всіх кроків, надішліть два посилання:

1. **GitHub Repository**: `https://github.com/veprelax/LEK5-7`
2. **GitHub Pages**: `https://veprelax.github.io/LEK5-7/`

---

## 💡 Корисні команди Git

```bash
# Перевірити статус
git status

# Подивитися всі коміти
git log --oneline

# Подивитися віддалені репозиторії
git remote -v

# Перевірити поточну гілку
git branch
```

## ❓ Можливі проблеми та рішення

### Проблема 1: Помилка автентифікації
**Рішення**: Створіть Personal Access Token на GitHub:
1. Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Generate new token (classic)
3. Виберіть права: `repo`, `workflow`
4. Використовуйте токен замість пароля

### Проблема 2: GitHub Pages не працює
**Рішення**:
- Перевірте, що репозиторій публічний
- Переконайтеся, що файл `index.html` існує в кореневій папці
- Зачекайте 5-10 хвилин після активації

### Проблема 3: Конфлікт гілок (master vs main)
**Рішення**:
```bash
# Перейменувати локальну гілку на main
git branch -M main

# Запушити на main
git push -u origin main
```

---

**Успіхів у виконанні завдання! 🚀**

