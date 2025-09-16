# Репозиторий курса информатики (10 класс)

Здесь публикуются задания и принимаются работы учащихся через **Pull Request**.

---

## 📂 Структура репозитория
- `assignments/` — условия заданий
- `submissions/` — выполненные работы
- `students/` — карточки учащихся (по желанию)

### Пример сдачи
```
submissions/
└── practice/
    └── 2025-09-07__data-structuring/
        └── Ivanov-Ivan/
            ├── solution.md
            └── REPORT.md
```

---

## 📝 Правила именования и оформления

### 1. Файлы и папки → `kebab-case`
- Все маленькими буквами, слова разделяются дефисами.
- Пример:  
  - `data-structuring/`  
  - `solution.md`  
  - `my-script.py`

### 2. Функции и переменные → `camelCase`
- Первая буква строчная, каждое следующее слово — с заглавной.  
- Пример:
  ```python
  totalSum = 0
  def calculateAverage(values):
      ...
  ```

### 3. Классы и компоненты → `PascalCase`
- Каждое слово с заглавной буквы.  
- Пример:
  ```python
  class DataProcessor:
      def process(self):
          ...
  ```

### 4. Константы → `UPPER_SNAKE_CASE`
- Все буквы заглавные, слова через подчёркивание.  
- Пример:
  ```python
  MAX_SIZE = 100
  DEFAULT_PATH = "/usr/local/bin"
  ```

---

## 🧰 Памятка по Git

### Первичная настройка
```bash
git config --global user.name "Maksim_Shestopalov"
git config --global user.email "makssest06@gmail.com"
```

### Основные команды
```bash
git clone <url>         # скопировать репозиторий
git status              # проверить состояние
git add <file>          # добавить файл в индекс
git commit -m "msg"     # зафиксировать изменения
git push                # отправить на сервер
git pull                # подтянуть обновления
```

### Работа с ветками
```bash
git checkout -b feature/loops-intro/ivanov-ivan   # создать и перейти в ветку
git checkout main                                # вернуться на главную ветку
git branch                                       # список веток
```

### Pull Request (PR)
1. Сделать fork репозитория  
2. Создать ветку: `feature/<assignment-id>/<Фамилия-Имя>`  
3. Добавить решение в правильную папку  
4. Сделать commit + push  
5. Открыть PR в основной репозиторий  

---

## 💻 Памятка по терминалу Linux

```bash
pwd         # показать текущую папку
ls          # показать список файлов
cd <dir>    # перейти в папку
cd ..       # выйти на уровень выше
mkdir name  # создать папку
rm file     # удалить файл
rm -r dir   # удалить папку с содержимым
cp a b      # скопировать файл
mv a b      # переместить/переименовать файл
cat file    # вывести содержимое файла
nano file   # открыть текстовый редактор
```

---

## ✅ Чеклист перед сдачей
- Файлы и папки названы по правилам (`kebab-case`).
- Код оформлен в едином стиле:
  - функции и переменные → `camelCase`
  - классы → `PascalCase`
  - константы → `UPPER_SNAKE_CASE`
- В папке работы есть:
  - решение (`solution.*`)
  - отчет (`REPORT.md`)
- Всё закоммичено в **своей ветке** и отправлено PR.
