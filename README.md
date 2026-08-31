# Иван Перепелюк
Студент 3 курса МАИ, направление "Прикладная информатика".
Специализация - Machine Learning и Data Science, с основным фокусом на
табличные данные и опытом в задачах компьютерного зрения.
Прошёл курс Data Science в Яндекс Практикуме. Участник хакатонов
Lenta Tech и Альфа-Будущее. Выступил на международной научной
конференции "Гагаринские чтения" с докладом по нейросетевому анализу
аудио.

## Стек
**Языки и работа с данными**  
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

**Классический ML и градиентный бустинг**  
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![CatBoost](https://img.shields.io/badge/CatBoost-FFCC00?style=for-the-badge&logoColor=black)
![LightGBM](https://img.shields.io/badge/LightGBM-02569B?style=for-the-badge)
![XGBoost](https://img.shields.io/badge/XGBoost-AA0000?style=for-the-badge)
![Optuna](https://img.shields.io/badge/Optuna-1B4F72?style=for-the-badge)
![SHAP](https://img.shields.io/badge/SHAP-8B0000?style=for-the-badge)

**Глубокое обучение и компьютерное зрение**  
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![YOLO](https://img.shields.io/badge/YOLOv8-00FFFF?style=for-the-badge&logoColor=black)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)

**Инфраструктура**  
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

## Проекты

### Lead Prioritization: приоритизация обращений
Задача бинарной классификации с ранговой метрикой Daily Average Precision.
Полный цикл: собственная time-based кросс-валидация (в sklearn нет
готового аналога для группировки по датам), feature engineering из
сырого лога событий с контролем утечки по времени, сравнение четырёх
моделей на деревьях, блендинг CatBoost и LightGBM по рангам.
Ключевая находка - редкие категории технического контекста показали
детерминированную связь с целевой переменной, подтверждённую SHAP-анализом
на двух моделях независимо. Итоговый результат на скрытой тестовой
выборке - **Daily AP = 0.7115** (наивный baseline - 0.22).
Стек: Python, CatBoost, LightGBM, Optuna, SHAP, scikit-learn.  
[Репозиторий](https://github.com/TrueWarriorI/lead-prioritization)

### Прогнозирование отмены бронирования отеля (UrbanStay)
Бинарная классификация на реальных данных из PostgreSQL (Yandex Cloud).
Отдельный акцент - хронологический train/test split для честной оценки
на production-подобном сценарии, сравнение CatBoost и Random Forest с
подбором гиперпараметров через Optuna, изотоническая калибровка
вероятностей для интерпретируемости порогов, интерпретация модели
через SHAP. Итоговый результат на тестовой выборке - **ROC-AUC 0.9753**,
экономический эффект (Incremental Revenue) вырос на **65.8%**
относительно текущей практики овербукинга.
Стек: Python, scikit-learn, CatBoost, Optuna, SHAP, Isotonic Calibration, PostgreSQL.  
[Репозиторий](ССЫЛКА)

### Lenta Tech Life Hack: распознавание ценников
Компьютерное зрение для роботов-ретейлеров. Двухступенчатый пайплайн:
детекция ценников на видео и OCR текста внутри найденных областей.
Стек: YOLOv8, PaddleOCR, OpenCV, PyTorch, Python.  
[Репозиторий](ССЫЛКА)

### Прогнозирование поломок промышленного оборудования
Предиктивное обслуживание на данных сервисной компании. Полный
ML-цикл: EDA, feature engineering, классификация отказов и регрессия
времени до отказа, валидация на отложенной выборке.
Стек: Python, pandas, scikit-learn, XGBoost.  
[Репозиторий](ССЫЛКА)

### Определение возрастной категории посетителей сайтов
Задача классификации по логам поведения пользователей (более 1 млн
записей о сессиях). EDA, feature engineering, сравнение нескольких
моделей на метриках f1_macro/precision_macro/recall_macro. Итоговый
результат - **F1_macro 0.674** на тестовой выборке при сильном
дисбалансе классов.
Стек: Python, scikit-learn, pandas, phik.  
[Репозиторий](#)

## Статистика GitHub
![GitHub stats](https://github-readme-stats.vercel.app/api?username=TrueWarriorI&show_icons=true&theme=dark&hide_border=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=TrueWarriorI&layout=compact&theme=dark&hide_border=true)

## Контакты
Email: perepelyuk_ivan07@mail.ru  
Telegram: [@perepelyuk10](https://t.me/perepelyuk10)
