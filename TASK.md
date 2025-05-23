# Курсовой проект: Анализ данных и создание интерактивного дашборда

## Цель проекта
Создание интерактивного дашборда и его деплой. По итогам проекта студенты должны предоставить:

- jupyter-notebook `eda.ipynb` с проведённым EDA-анализом выбранного датасета.
- Аналитическую записку `summary.md` с выводами по результатам проведённого EDA-анализа.
- Ссылку на репозиторий, в котором хранится код проекта.
- Ссылку на задеплоенный и работающий дашборд.

**Примечание**: Файлы `eda.ipynb` и `summary.md` должны быть размещены в репозитории проекта.

## Описание проекта

### 1. Используемые данные

- Студенты должны самостоятельно выбрать датасет, который будет использоваться для создания дашборда.
- Студенты могут использовать публично доступные датасеты из интернета либо создать свой собственный датасет из реальных данных.
- Датасет должен состоять из минимум 3 таблиц, которые можно связать друг с другом по основным и внешним ключам.

### 2. EDA

EDA-анализ должен проводиться в соответствии с теми же условиями, что и для финального проекта первой половины курса. Дополнительно в EDA-анализе студенты должны продемонстрировать использование статистики для проверки гипотез и сравнения выборок.

### 3. Структура репозитория

В репозитории обязательно наличие:

- `readme.md` — файл с описанием репозитория. Должен содержать:
  - Название проекта и его краткое описание: кем создан (если проект создан в команде, добавить ссылку на GitHub профиль второго участника), для чего и т.д.
  - Описание датасета и ссылку на источник (если датасет взят из интернета).
  - Описание структуры репозитория.
  - Описание используемых инструментов.
  - Ссылку на задеплоенный дашборд.

- `source` — папка, в которой должны храниться файлы используемого датасета в виде файлов с расширением `.csv` или `.xlsx`.
- `eda` — папка, содержащая файлы `eda.ipynb` и `summary.md`.
- `queries` — папка, которая должна содержать файлы с расширением `.sql`, в которых должны содержаться:
  - Скрипт создания таблиц в базе данных (БД).
  - Скрипты создания представлений (вьюшки).
  - Скрипты запросов.
- `my.db` — локальный файл БД DuckDB.
- `ddl.py` — модуль, отвечающий за создание таблиц в БД и заполнение их данными из источника.
- `db.py` — модуль, отвечающий за получение данных из БД для создания датафреймов.
- `main.py` — модуль, отвечающий за создание дашборда.
- `requirements.txt` — файл, содержащий список используемых библиотек и их версий. В проекте обязательно использование следующих библиотек:
  - `DuckDB` — для создания и работы с БД.
  - `Pandas` — для создания и работы с датафреймами.
  - `Plotly` — для создания диаграмм.
  - `Streamlit` — для создания дашборда.

**Примечания**: Каждая функция должна содержать doc-string. Проект должен быть хорошо задокументирован. Сложные части кода должны быть сопровожены комментариями.

ℹ️ При необходимости студенты могут добавлять дополнительные папки, модули и библиотеки.

### 4. Требования к скриптам SQL

- Каждый скрипт должен быть правильно отформатирован.
- Датафреймы должны создаваться на основе запросов к БД.
- **Не допускается** создание датафреймов путём чтения данных напрямую из файлов таблиц.
- В скриптах запросов и/или вьюшек студенты должны продемонстрировать использование:
  - Агрегирующих функций.
  - Функций работы с текстом и датами.
  - Оконных функций.
  - Подзапросов.
  - Джойнов.

### 5. Требования к дашборду

- Наличие заголовка дашборда.
- Наличие минимум двух элементов управления, фильтрующих диаграммы.
- Наличие минимум четырёх диаграмм.

### 6. Работа в команде

- Студенты могут работать над курсовым проектом как индивидуально, так и в составе команды из двух человек.

---

### Ссылки:

- Репозиторий проекта: [https://github.com/datacoach2024/adventure_works](https://github.com/datacoach2024/adventure_works)
- Задеплоенный дашборд: [https://datacoach2024-adventure-works-main-d7cqxx.streamlit.app](https://datacoach2024-adventure-works-main-d7cqxx.streamlit.app)
