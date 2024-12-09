Data Mining Habr Articles
----

Create dataset from Habr articles of 'Popular Science' topic.

Dataset собран из информации с сайта ```habr.com```, по тематике 'Научпоп'.
В файле ```Data_collection.ipynb``` рассматривается метод сбора dataset'а.
Dataset был собран для дальнейшего анализа с помощью различных методов.

## Разделы

- Сбор данных
    - Data_collection.ipynb
    - Exploratory_analysis.ipynb
- Представление TF-IDF, word2vec/fasttext эмбеддинги
    - Text_clustering.ipynb (Word2Vec и FastText с весами TF-IDF)
    - Text_vectorization&clustering.ipynb
- Классификация текстов.
    - Classification.ipynb (del_freq_words.csv.7z)
- Тематическое разбиение текстов. Выделение именованных сущностей 
    - Thematic_analysis.ipynb
- Генерация текстов
    - Text_generation/Statistical_model.ipynb
    - Text_generation/gen_statistic.csv - Сгенерированные тексты статистической моделью
    - Text_generation/Neural_model.ipynb



## Структура данных

Data columns (total 12 columns):
| #   Column          | Non-Null| Count | Dtype   |
|---|---|---|---|
|  0   url              |4338 |non-null  | object |
|  1   title            |4338 |non-null  | object |
|  2   theme            |4338 |non-null  | object |
|  3   tags             |4338 |non-null  | object |
|  4   read_time        |4338 |non-null  | int64  |
|  5   number_of_views  |4338 |non-null  | int64  |
|  6   date             |4338 |non-null  | object |
|  7   amount_of_imgs   |4338 |non-null  | int64  |
|  8   comments         |4338 |non-null  | int64  |
|  9   bookmark         |4338 |non-null  | int64  |
|  10  votes            |4338 |non-null  | int64  |
|  11  text             |4338 |non-null  | object |

|Наименование атрибута| Расшифровка|
|--|--|
|url|Ссылка на статью|
|title|Заголовок статьи|
|theme|Так, как у статьи несколько тегов вместо тем, то берется первый тег, как главная тема статьи|
|tags|Все теги статьи списком|
|read_time| Среднее время прочтения статьи|
|number_of_views| Количество просмотров|
|date|Дата публикации статьи|
|amount_of_imgs|Количество изображений, содержащихся в статье|
|comments|Количество комментариев|
|bookmark|Количество закладок|
|votes|Количество голосов|
|text|Текст статьи|



