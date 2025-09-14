# Decentrathon InDrive — Анализ геотреков и прогноз спроса

Проект по анализу обезличенных геотреков:  
- визуализации (heatmap, маршруты)  
- модель прогнозирования спроса с помощью CatBoost  
- интерактивные ноутбуки прототипов

---

## Структура репозитория

| Папка / Файл | Назначение |
|--------------|------------|
| `geotracks_project.ipynb` | Основной ноутбук: EDA, построение модели, визуализации |
| `geotracks_prototype.ipynb` | Прототип / альтернативные эксперименты |
| `catboost_info` | Информация по обучению CatBoost (например, параметры, метрики) |
| `.gitignore` | Файлы, которые не должны попадать в репозиторий |

---

## Установка и требования

1. Убедись, что у тебя установлен Python 3.8+  
2. Установи нужные библиотеки:

```bash
pip install -r requirements.txt


---

## ⚙️ Этапы: как запустить ноутбук

1. **Клонировать репозиторий**  
   `git clone https://github.com/dturgambayev/decentrathon_indrive.git`

2. **Перейти в папку проекта**  
   `cd decentrathon_indrive`

3. **Создать виртуальное окружение**  
   - Windows:  
     ```bash
     python -m venv venv
     venv\Scripts\activate
     ```
   - Linux / Mac:  
     ```bash
     python3 -m venv venv
     source venv/bin/activate
     ```

4. **Установить зависимости**  
   Если есть `requirements.txt`:  
   ```bash
   pip install -r requirements.txt
Если нет — установить вручную:

pip install pandas numpy matplotlib seaborn scikit-learn catboost h3 folium


Запустить Jupyter Notebook

jupyter notebook


или если используешь JupyterLab:

jupyter lab

Открыть и выполнить ноутбук
Например, geotracks_project.ipynb.

Просмотри первые ячейки, проверь пути к данным.

Если ноутбук требует данных, которых нет, либо внеси их в репо / добавь инструкцию скачивания.

(Опционально) Сохранить модель и визуализации

После тренировки модели — экспортировать (model.save_model("models/catboost_model.cbm"))

Сохранить графики / тепловые карты в формате .png или .html