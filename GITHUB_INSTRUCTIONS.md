# Инструкция по загрузке проекта в GitHub

## Вариант 1: Через GitHub Desktop (самый простой способ)

1. **Установите GitHub Desktop** (если еще не установлен):
   - Скачайте с https://desktop.github.com/
   - Установите и войдите в свой аккаунт GitHub

2. **Создайте новый репозиторий**:
   - В GitHub Desktop: File → New Repository
   - Имя: `lab2-codeforces-analysis` (или любое другое)
   - Local Path: выберите папку `C:\Users\venya\Лаб2`
   - Нажмите "Create Repository"

3. **Добавьте файлы**:
   - Все файлы уже в папке, они автоматически появятся в GitHub Desktop
   - Напишите сообщение коммита: "Initial commit: Лабораторная работа № 2"
   - Нажмите "Commit to main"

4. **Опубликуйте на GitHub**:
   - Нажмите "Publish repository"
   - Выберите, сделать ли репозиторий публичным или приватным
   - Нажмите "Publish repository"

## Вариант 2: Через веб-интерфейс GitHub

1. **Создайте новый репозиторий на GitHub**:
   - Зайдите на https://github.com
   - Нажмите "+" → "New repository"
   - Имя: `lab2-codeforces-analysis`
   - Выберите Public или Private
   - НЕ ставьте галочки на "Initialize with README"
   - Нажмите "Create repository"

2. **Загрузите файлы**:
   - На странице нового репозитория нажмите "uploading an existing file"
   - Перетащите все файлы из папки `C:\Users\venya\Лаб2`:
     - lab2.ipynb
     - contests.csv
     - rating_changes.csv
     - users.csv
     - README.md
     - .gitignore
   - Напишите сообщение коммита: "Initial commit: Лабораторная работа № 2"
   - Нажмите "Commit changes"

## Вариант 3: Через командную строку (если установлен Git)

Откройте PowerShell или Command Prompt в папке проекта и выполните:

```bash
# Инициализация репозитория
git init

# Добавление всех файлов
git add .

# Создание первого коммита
git commit -m "Initial commit: Лабораторная работа № 2"

# Добавление удаленного репозитория (замените YOUR_USERNAME на ваш логин GitHub)
git remote add origin https://github.com/YOUR_USERNAME/lab2-codeforces-analysis.git

# Переименование ветки в main (если нужно)
git branch -M main

# Отправка на GitHub
git push -u origin main
```

**Важно**: Перед выполнением команд создайте репозиторий на GitHub (Вариант 2, шаг 1)

## Что будет загружено:

✅ **Будет загружено:**
- lab2.ipynb (основной блокнот)
- contests.csv
- rating_changes.csv
- users.csv
- README.md (описание проекта)
- .gitignore (исключения для Git)

❌ **НЕ будет загружено** (благодаря .gitignore):
- Временные файлы Python
- Кэш Jupyter
- Файлы IDE
- Системные файлы

⚠️ **Примечание**: Файл `Лабораторная работа № 2.pptx` довольно большой. 
Если GitHub откажется его загружать (лимит 100MB), можно:
1. Загрузить его отдельно через Google Drive
2. Или добавить в .gitignore

## После загрузки:

1. Скопируйте ссылку на репозиторий
2. Отправьте ссылку преподавателю
3. Убедитесь, что все файлы видны на GitHub

