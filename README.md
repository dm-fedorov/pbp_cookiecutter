#  Cookiecutter Template: Repeatable Data Analysis with Notebooks 

A [cookiecutter template](https://cookiecutter.readthedocs.io/en/1.7.2/) for simple data analysis.

Full details and walk-through over at [**Practical Business Python:  Building a Repeatable Data Analysis Process with Jupyter Notebooks** ](http://pbpython.com/notebook-process.html) on the background and how to use this cookiecutter template.

## Структура директорий

This template will jumpstart your data science projects with the following predictable organizational file structure:

```bash
.
├── 1-Data_Prep.ipynb  # Блокнот для подготовки данных
├── 2-EDA.ipynb        # Блокнот для анализа данных
├── data               # Директория с данными
│   ├── interim        # Рабочая директория для временных файлов
│   ├── processed      # Очищенные данные, готовые к анализу
│   └── raw            # Оригинальные (сырые) данные
└── reports            # Финальные отчеты
```

## Установка

```bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```

## Использование

В директории, в которой вы хотите держать запускаемый проект, запустите шаблон следующим образом, ответив на вопросы, относящиеся к вашему проекту:

```bash
$ cookiecutter https://github.com/dm-fedorov/pbp_cookiecutter        
project_name [project_name]: data_journalism_project
directory_name [data_journalism_project]: 
description [More background on the project]: Research into latest news trends.
```

В результате получится директория `data_journalism_project`, в которой хранятся необходимые файлы.