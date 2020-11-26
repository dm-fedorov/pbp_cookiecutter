#  Шаблон Cookiecutter: Повторяемый анализ данных с помощью Jupyter Блокнотов 

Идея из статьи [**Practical Business Python:  Building a Repeatable Data Analysis Process with Jupyter Notebooks** ](http://pbpython.com/notebook-process.html).

Шаблон [cookiecutter template](https://cookiecutter.readthedocs.io/en/1.7.2/) для простого анализа данных.

## Структура директорий

Типичный процесс проведения анализа данных:

![Drag Racing](https://pbpython.com/images/Notebook_Best_Practices_flow.png)

Следующий шаблон ускорит разработку проектов в области науки о данных, т.к. обладает ясной и предсказуемой структурой файлов и директорий:

```bash
.
├── 1-Data_Prep.ipynb  # Блокнот для подготовки данных
├── 2-EDA.ipynb        # Блокнот для анализа данных
├── data               # Директория с данными
│   ├── interim        # Рабочая директория для временных файлов
│   ├── processed      # Очищенные данные, готовые к анализу
│   └── raw            # Оригинальные (сырые) данные (никогда не должны изменяться)
└── reports            # Финальные отчеты
```

## Установка

```bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```

## Использование

В директории, в которой вы хотите хранить запускаемый проект, выполните шаблон следующим образом, ответив на вопросы, относящиеся к вашему проекту:

```bash
$ cookiecutter https://github.com/dm-fedorov/pbp_cookiecutter        
project_name [project_name]: data_journalism_project
directory_name [data_journalism_project]: 
description [More background on the project]: Research into latest news trends.
```

В результате появится директория `data_journalism_project`, в которой хранятся необходимые файлы.