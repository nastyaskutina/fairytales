Подробное описание кода можно найти в тексте дипломной работы

coreference_data  - скрипт получения данных для разрешения кореференции. Получает на вход корпус RuCor в виде таблицы. Для каждого текста проводится синтаксический анализ, извлекаются глаголы и их аргументы. Создается таблица, каждая строчка которой отражает пару аргумент - его возможный антецендент, их морфологические свойства, информацию об их кореферентности (1 для кореферентных аргументов, иначе - 0). Ссылка на полученную таблицу (https://drive.google.com/file/d/1f_AZsGl3QFiXFq7xm6iQY7DTmjTVVw9m/view?usp=share_link)

data_process - скрипт обработки корпуса сказок и создания структуры данных для обучения модели. Получает таблицу из предыдущего скрипта, с помощь которой тренируется модель разрешения кореференции. Затем проводится обработка данных корпуса сказок, формируются документы с вхождениями пар событий (coref_event_count, coref_role_count - отличается наличием информации об аргументах для каждой пары). Также создается документ со всеми возможными событиями из сказок (all_events) и подсчетом количества событий (event_count)

results_check - тетрадка, в которой проводился обзор результатов

schema_script - дополнительный скрипт с возможной реализацией построения нарративных схем

(main - тетрадь-черновик, в которой велась непосредственная работа над кодом)
