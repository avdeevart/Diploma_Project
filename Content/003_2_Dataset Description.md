
# 4.1 Описание данных и источников

---

### [Полный справочник полей данных](https://github.com/avdeevart/Diploma_Project/blob/main/Content/Dataset/DataDescript.docx)

---

### Описание данных и источников для разработки сервиса

#### 1. Технико-Экономические Характеристики Многоквартирных Домов
Данный набор данных предоставляет подробную информацию о различных параметрах многоквартирных домов, включая материалы, из которых они построены, года постройки и реконструкции, размеры и дополнительные спецификации.

- **Применение:** Эти данные необходимы для анализа текущего состояния жилищного фонда и могут быть использованы для планирования работ по капремонту и ассоциации с данными о происшествиях и проведенных работах.

#### 2. Регистрация Инцидентов на Объектах Городской Инфраструктуры
Этот датасет предоставляет информацию о зарегистрированных инцидентах, содержащую даты, места и детали инцидентов.

- **Применение:** Данные о инцидентах могут служить для анализа корреляции с характеристиками домов и для выявления потенциальных проблемных зон в жилищном фонде.

#### 3. Выполненные Работы по Капитальному Ремонту
Набор данных содержит подробную информацию о прошлых работах по капремонту, включая периоды, статусы, стоимость и другие параметры.

- **Применение:** Анализ этих данных позволит выявить зависимости и тенденции в работах по ремонту, а также спрогнозировать будущие потребности.

#### 4. Классификация Видов Работ
Данные предоставляют разделение работ на типы, группы и другие категории.

- **Применение:** Классификация обеспечивает структурированное разделение работ и может использоваться для планирования и категоризации будущих работ по капремонту.

#### 5. Классификация Типов Событий
Данный раздел предоставляет классификацию событий и происшествий, которые могут быть зарегистрированы.

- **Применение:** Классификация событий необходима для структурированного анализа и реагирования на инциденты в многоквартирных домах.

### Выводы и Рекомендации для Разработки Сервиса
Предоставленные данные служат фундаментом для разработки сервиса, который может эффективно анализировать и прогнозировать потребности в работах по капитальному ремонту, а также выявлять потенциальные проблемные зоны на основе анализа прошлых инцидентов и работ. Рекомендуется провести дополнительный анализ данных на предмет пропусков и аномалий, а также разработать методологию для интеграции и обновления данных в будущем.

 Следует также уделить внимание взаимосвязям между различными типами данных для создания комплексных моделей анализа и прогнозирования.

---

### Описание файлов датасета:

---
Файл [`1_M_buildings_tech_econom_char.xlsx`](https://github.com/avdeevart/Diploma_Project/blob/main/Content/Dataset/1_M_buildings_tech_econom_char.xlsx) содержит данные о различных зданиях и их технико-экономических характеристиках. Первый взгляд на данные дает следующую информацию:

### Общая информация:
- **Количество записей (строк):** 18,433
- **Количество атрибутов (столбцов):** 32

### Атрибуты:
Некоторые из атрибутов в данных:
- ID
- NAME
- PARENT_ID
- LOGIN
- COL_754
- COL_755
- ... и другие, названия которых представляют собой коды.

Замечание: Названия столбцов (как "COL_754", "COL_755" и т. д.) не являются информативными и, возможно, требуют дополнительной метаинформации для понимания их содержания.

### Пропущенные значения:
Некоторые столбцы имеют значительное количество пропущенных значений. Например:
- PARENT_ID: 18,411 пропущенных значений
- COL_754: 14,277 пропущенных значений
- COL_755: 18,432 пропущенных значений
- ... и так далее.

### Превью данных:
Первые несколько строк данных предоставляют нам следующее:

| ID | NAME | PARENT_ID | LOGIN | COL_754 |
|----|------|-----------|-------|---------|
| NaN | NaN | NaN | NaN | Назначение |
| 1500923.0 | Дом по адресу Красковская ул., д.121А | NaN | WS | NaN |
| 1500933.0 | Дом по адресу Байкальская ул., д.18, к.2 | NaN | WS | NaN |
| 1500943.0 | Дом по адресу Перовская ул., д.48 | NaN | WS | NaN |
| 1500951.0 | Дом по адресу Парковая 3-я ул., д.39, к.3 | NaN | 404070001 | NaN |

В целом, эти данные, вероятно, содержат важную информацию о различных зданиях и их характеристиках, хотя точное понимание каждого атрибута требует дополнительного контекста или метаданных.

---

Файл [`2_Incidents_registered_at_municipal_facilities.xlsx`](https://disk.yandex.ru/d/ohVNotlcOqCiYg) содержит информацию о различных инцидентах, зарегистрированных в муниципальных объектах. Обзор первых 10 строк данных указывает на то, что данный файл содержит разнообразную информацию, отмеченную временными метками и, возможно, географическими данными.


### Basic Information 
**Shape:** (10, 6)

### Columns 
1. Отклонение ГВС ниже нормы ночью (мониторинг)
2. ASUPR
3. 2022-06-18 03:46:09.000000
4. 2022-06-18 00:46:58.531000
5. ВАО
6. внутригородская территория муниципальный округ Ивановское, улица Сталеваров, дом 8А

### Missing Values 
- Отклонение ГВС ниже нормы ночью (мониторинг): 0
- ASUPR: 0
- 2022-06-18 03:46:09.000000: 0
- 2022-06-18 00:46:58.531000: 0
- ВАО: 0
- внутригородская территория муниципальный округ Ивановское, улица Сталеваров, дом 8А: 0

### Data Preview 
| Отклонение ГВС ниже нормы ночью (мониторинг) | ASUPR | 2022-06-18 03:46:09.000000 | 2022-06-18 00:46:58.531000 | ВАО | внутригородская территория муниципальный округ Ивановское, улица Сталеваров, дом 8А |
|---|---|---|---|---|---|
| Критичное отклонение температуры ГВС ниже норм... | ASUPR | 2022-06-17 18:55:07.000000 | 2022-06-17 15:55:22.002000 | ВАО | внутригородская территория муниципальный округ... |
| Отсутствует циркуляция ГВС | ASUPR | 2022-06-16 15:54:58.000000 | 2022-06-16 20:54:21.676000 | ВАО | внутригородская территория муниципальный округ... |
| ... | ... | ... | ... | ... | ... |


#### Ключевые особенности данных:
- **Отклонение ГВС ниже нормы ночью (мониторинг):** Вероятно, содержит описания или категории отклонений или инцидентов.
- **ASUPR:** Не ясно из предоставленной выборки, требуется дополнительный контекст.
- **2022-06-18 03:46:09.000000 и 2022-06-18 00:46:58.531000:** Кажется, содержат временные метки, но необходимо проверить наличие стандартности во всем столбце.
- **ВАО:** Возможно, географическое или административное разделение, но требуется подтверждение.
- **внутригородская территория муниципальный округ Ивановское, улица Сталеваров, дом 8А:** Вероятно, содержит адреса или геолокацию инцидентов.

#### Примечания и рекомендации:
- **Качество данных:** Из первоначального просмотра данных не обнаружено пропущенных значений, но проверка полного набора

 данных на наличие дубликатов, консистентности и точности крайне рекомендуется.
- **Оптимизация:** Столбцы с датой и временем следует преобразовать в формат datetime для оптимизации хранения и анализа данных.
- **Структура данных:** Рекомендуется дополнительный анализ для определения, являются ли столбцы единообразными и стандартными на протяжении всего набора данных.
- **Подробный анализ:** Глубокий анализ каждого столбца с использованием всего объема данных даст более точную картину и поможет выявить скрытые особенности или проблемы данных.

Это заключение основано на предварительном просмотре ограниченного набора данных. Более детальный анализ полного набора данных с использованием подходящих инструментов анализа данных может выявить дополнительные особенности и проблемы.

---

Файл [`3_Capital_repair_works_performed_in_apartment_buildings.xlsx`]([Файл](https://github.com/avdeevart/Diploma_Project/blob/main/Content/Dataset/3_Capital_repair_works_performed_in_apartment_buildings.xlsx)) содержит информацию о капитальном ремонте, проведенном в жилых зданиях, с различными характеристиками и параметрами работ. Данные включают временные рамки (планируемые и фактические даты начала и окончания работ), географическую локацию (административная зона, район, адрес), и спецификации работы (например, название работы). 


#### Basic Information 
- **Shape:** Неопределенно (предварительный просмотр 10 строк)
  
#### Columns 
1. `global_id`: Уникальный идентификатор (нет пропущенных значений)
2. `PERIOD`: Период (нет пропущенных значений)
3. `WORK_NAME`: Название работы или вида работ (нет пропущенных значений)
4. `NUM_ENTRANCE`: Номер подъезда (7 пропущенных значений)
5. `ElevatorNumber`: Номер лифта (7 пропущенных значений)
6. `PLAN_DATE_START`: Планируемая дата начала (нет пропущенных значений)
7. `PLAN_DATE_END`: Планируемая дата окончания (нет пропущенных значений)
8. `FACT_DATE_START`: Фактическая дата начала (нет пропущенных значений)
9. `FACT_DATE_END`: Фактическая дата окончания (нет пропущенных значений)
10. `AdmArea`: Административная зона (нет пропущенных значений)
11. `District`: Район (нет пропущенных значений)
12. `Address`: Адрес (нет пропущенных значений)
13. `UNOM`: Неясно (нет пропущенных значений)

#### Missing Values 
- `NUM_ENTRANCE`: 7
- `ElevatorNumber`: 7

#### Data Preview 

| global_id | PERIOD | WORK_NAME | NUM_ENTRANCE | ElevatorNumber | PLAN_DATE_START | PLAN_DATE_END | FACT_DATE_START | FACT_DATE_END | AdmArea | District | Address | UNOM |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 351060 | 2022 | замена лифтового оборудования | 1.0 | 1.0 | 15.07.2022 | 28.08.2022 | 27.06.2022 | 14.10.2022 | ВАО | район Богородское | Российская Федерация, город Москва, внутригородская территория... | 20151 |
| ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |


Поле `global_id` вероятно является уникальным идентификатором каждой записи, в то время как `NUM_ENTRANCE` и `ElevatorNumber` имеют некоторое количество пропущенных значений, что может указывать на отсутствие лифтов или подъездов в некоторых объектах или же на недостаток данных. 

Поля `PLAN_DATE_START`, `PLAN_DATE_END`, `FACT_DATE_START`, и `FACT_DATE_END` содержат временные метки, которые могут быть использованы для анализа длительности работ и возможных задержек. 

Географические метаданные (`AdmArea`, `District`, `Address`) предоставляют возможность для пространственного анализа и могут быть использованы для определения географических закономерностей или трендов в данных.

В целом, данные представляют собой комплексный набор информации, который может быть использован для анализа эффективности проведения капитального ремонта в разных районах и временных периодах, а также для выявления возможных проблемных зон или определения будущих приоритетов работ. Всегда рекомендуется провести дополнительный анализ и предобработку данных перед использованием их в исследовании или модели машинного обучения.

---

Файл [`4.1_Work_types_for_capital_repair_of_apartment_buildings.xlsx`](https://github.com/avdeevart/Diploma_Project/blob/main/Content/Dataset/4.1_Work_types_for_capital_repair_of_apartment_buildings.xlsx
) содержит информацию о различных типах работ, связанных с капитальным ремонтом жилых зданий. Каждый вид работы имеет уникальный код, наименование, тип и группу работ, а также сокращенное наименование. Данные, вероятно, могут быть использованы для классификации и категоризации различных видов работ в рамках проектов капитального ремонта, и их можно использовать для аналитики и планирования ремонтных работ. 


#### Basic Information 
- **Shape:** Неопределенно (предварительный просмотр 10 строк)
  
#### Columns 
Колонки не имеют осмысленных названий и следует переименовать их для лучшего понимания содержимого:
1. `No`: Номер п/п (нет пропущенных значений)
2. `Code`: Код (нет пропущенных значений)
3. `Name`: Наименование (нет пропущенных значений)
4. `CommonPropertyObject`: Наименование объекта общего имущества (нет пропущенных значений)
5. `WorkType`: Тип работ (нет пропущенных значений)
6. `WorkGroup`: Группа работ (нет пропущенных значений)
7. `ShortWorkName`: Сокращенное наименование работы (нет пропущенных значений)

#### Missing Values 
Пропущенных значений нет.

#### Data Preview 
| No | Code | Name | CommonPropertyObject | WorkType | WorkGroup | ShortWorkName |
|---|---|---|---|---|---|---|
| 1 | 105 | строительный контроль | Строительный контроль | Услуга | Стройконтроль | СК |
| 2 | 26 | ремонт подъездов... | Подъезд | Работа | СМР | Подъезд |
| ... | ... | ... | ... | ... | ... | ... |


Основываясь на предварительном просмотре данных, следует отметить, что данными, вероятно, можно пользоваться для сопоставления и анализа в других датасетах, используя уникальный код работы как связующее звено. Также может быть полезно использовать этот датасет для анализа распределения типов работ в различных проектах и районах, а также для определения, какие виды работ являются наиболее распространенными или критическими в контексте капитального ремонта.

Также стоит проверить полный датасет на предмет консистентности данных и возможных дубликатов для уверенности в качестве данных перед их использованием в аналитических или моделировочных задачах.

---

Файл [`4.2_Work_types_for_maintenance_and_repair_of_common_property_of_apartment_buildings.xlsx`](https://github.com/avdeevart/Diploma_Project/blob/main/Content/Dataset/4.2_Work_types_for_maintenance_and_repair_of_common_property_of_apartment_buildings.xlsx) содержит информацию о различных типах работ, связанных с обслуживанием и ремонтом общего имущества в жилых зданиях. Он включает в себя идентификаторы, названия работ и дополнительную техническую информацию, структура и содержание которой требует дополнительного разбора.


#### Basic Information 
- **Shape:** Неопределенно (предварительный просмотр 10 строк)
  
#### Columns 
Колонки имеют технические идентификаторы, и их следует переименовать для удобства интерпретации:
1. `ID`: Идентификатор записи (нет пропущенных значений)
2. `NAME`: Название работы (нет пропущенных значений)
3. `PARENT_ID`: Идентификатор родительской категории (нет пропущенных значений)
4. `LOGIN`: Информация о входе (нет пропущенных значений)
5. ... Другие столбцы с неизвестным содержимым и неинформативными названиями

#### Missing Values 
Несколько столбцов имеют пропущенные значения во всех просмотренных строках, что требует дальнейшего исследования для понимания их природы и необходимости.

#### Data Preview 
| ID | NAME | PARENT_ID | LOGIN | ... |
|---|---|---|---|---|
| 3682661 | Ремонт кровельного покрытия дома | 26352880 | migration | ... |
| 3682664 | Ремонт мусоропроводов | 26352883 | migration | ... |
| ... | ... | ... | ... | ... |


- **Структура данных:** Столбцы, начиная с `COL_1044`, `COL_1045` и так далее, не имеют осмысленных названий, что затрудняет понимание их функций и содержания. Необходимо провести дополнительный анализ или консультацию с экспертами домена для интерпретации этих данных.
- **Пропущенные значения:** Некоторые столбцы имеют пропущенные значения во всех просмотренных строках, что может указывать на отсутствие данных или их нерелевантность для некоторых записей.
- **Очистка данных:** Данные могут потребовать дополнительной очистки и предобработки, включая нормализацию текста и обработку пропущенных значений, перед тем как они будут готовы к использованию в аналитических задачах или моделях машинного обучения.

В целом, данные представляют полезный ресурс для анализа и планирования работ по обслуживанию и ремонту общего имущества в жилых зданиях. Однако, перед использованием данных в аналитических или моделировочных задачах, их следует тщательно исследовать и предобработать для обеспечения их качества и релевантности.

---

Данный файл [`5_Types_of_events_to_be_registered_by_object_type_apartment_building.xlsx`](https://github.com/avdeevart/Diploma_Project/blob/main/Content/Dataset/5_Types_of_events_to_be_registered_by_object_type_apartment_building.xlsx) содержит информацию о различных типах событий, которые следует регистрировать по типу объекта "жилой дом". Каждое событие имеет уникальный идентификатор, название и относится к определенной системе.

#### Basic Information 
- **Shape:** Неопределенно (предварительный просмотр 10 строк)
  
#### Columns 
1. `id`: Уникальный идентификатор события (нет пропущенных значений)
2. `name`: Название события (нет пропущенных значений)
3. `system`: Система, к которой относится событие (нет пропущенных значений)

#### Missing Values 
Пропущенных значений нет.

#### Data Preview 
| id | name | system |
|---|---|---|
| 001b91e9-2ac5-4949-bff0-bb51d4f3057c | Нарушение в работе  АГВ | MOS_GAS |
| 0089fd48-aa7a-443d-85a5-00470285b076 | Проверить на загазованность дюкер Гольяновский | MOS_GAS |
| ... | ... | ... |

- **Типы событий:** Название событий представляют собой текстовые строки, которые описывают конкретные инциденты или ситуации, которые могут возникнуть в контексте жилых зданий. Например, "Нарушение в работе АГВ" или "Запах газа от ГРП".
- **Системы:** Системы, кажется, относят события к определенным категориям или подсистемам в контексте управления жилыми зданиями. Например, "MOS_GAS" может относиться к событиям, связанным с газовыми системами или утилитами.

Эти данные могут быть полезны для анализа типов и частоты различных событий в контексте управления жилыми зданиями, позволяя создать систему мониторинга или уведомлений для быстрого реагирования на инциденты и оптимизации планов обслуживания и ремонта. Также это может помочь в выявлении повторяющихся проблем или областей, требующих дополнительного внимания в стратегии обслуживания и ремонта.

---

Данный файл [`predict_by_house.xlsx`](https://github.com/avdeevart/Diploma_Project/blob/main/Content/Dataset/predict_by_house.xlsx) содержит информацию о планируемых работах по ремонту для разных домов, идентифицируемых уникальным номером (`unom`). Каждая запись включает в себя список планируемых работ (`works`) и их количество (`num_works`).


#### Basic Information 
- **Shape:** Неопределенно (предварительный просмотр 10 строк)
  
#### Columns 
1. `unom`: Уникальный номер дома (нет пропущенных значений)
2. `works`: Список планируемых работ (нет пропущенных значений)
3. `num_works`: Количество планируемых работ (нет пропущенных значений)

#### Missing Values 
Пропущенных значений нет.

#### Data Preview 
| unom | works | num_works |
|---|---|---|
| 17687 | ['замена лифтового оборудования', 'ремонт внут...'] | 10 |
| 16182 | ['замена лифтового оборудования', 'ремонт внут...'] | 10 |
| ... | ... | ... |


- **Планируемые работы:** Список работ представлен в виде строковой записи, которую, возможно, потребуется дополнительно обработать для преобразования в удобный для анализа формат (например, список или множество).
- **Количество работ:** В данном столбце указано количество планируемых работ, что может быть полезно для быстрого определения объема работ для каждого дома.

Данные могут быть полезны для анализа и планирования работ по ремонту, а также для выявления возможных трендов или закономерностей в распределении работ между разными домами. Также, эти данные могут быть использованы для предсказания потребности в ресурсах или для определения приоритетов в планировании работ на будущее. Однако, следует учесть необходимость дополнительной предобработки данных для обеспечения их качества и удобства использования.

---

Файл [`prediction_by_inc.xlsx`](https://github.com/avdeevart/Diploma_Project/blob/main/Content/Dataset/prediction_by_inc.xlsx) предоставляет информацию о планируемых работах по ремонту для различных домов, идентифицируемых уникальными номерами (`unom`). Каждый объект (дом) имеет связанный с ним список планируемых работ (`works_list`) и их количество (`num_works`). 

#### Basic Information 
- **Shape:** Неопределенно (предварительный просмотр 10 строк)
  
#### Columns 
1. `unom`: Уникальный номер дома (нет пропущенных значений)
2. `works_list`: Список планируемых работ (нет пропущенных значений)
3. `num_works`: Количество планируемых работ (нет пропущенных значений)

#### Missing Values 
Пропущенных значений нет.

#### Data Preview 
| unom | works_list | num_works |
|---|---|---|
| 2930 | ['замена лифтового оборудования', 'ремонт внут...'] | 15 |
| 15130 | ['замена лифтового оборудования', 'ремонт внут...'] | 14 |
| ... | ... | ... |

- **Планируемые работы:** Список работ представлен в виде строковой записи, которую, возможно, потребуется дополнительно обработать для преобразования в удобный для анализа формат (например, список или множество).
- **Количество работ:** Предоставлены данные о количестве планируемых работ, что может быть полезно для быстрого определения объема работ для каждого дома.

В целом, структура данных аналогична предыдущему файлу "predict_by_house.xlsx", однако, возможно, они отражают различные аспекты или подходы к предсказанию планируемых работ. Данные могут быть использованы для анализа и планирования работ по ремонту, а также для выявления возможных трендов или закономерностей в распределении работ между разными домами. Однако, следует учесть необходимость дополнительной предобработки данных для обеспечения их качества и удобства использования.


