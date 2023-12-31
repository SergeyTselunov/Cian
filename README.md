# Cian
Apartment price prediction

Целью проекта является прогнозирование цены за один квадратный метр.
Для проекта я выбрал квартиры на сайте ЦИАН. Параметры по которым я выбирал квартиры: в г. Москва, до 5 комнат включительно, для проживания.
По 100 квартир на каждую станцию метро из 150 выбранных станций.

 `Файл` | `Описание` | 
| :-------| :-----------|
| [**Parsing Cian**](https://github.com/SergeyTselunov/Cian/blob/main/Cian_parsing.ipynb) | В данном блокноте находятся коды, которые были написан для выгрузки объявлений с сайта и выгрузки характеристик по квартирам.|
| [**DataFrame Creating**](https://github.com/SergeyTselunov/Cian/blob/main/Cian_data_creating.ipynb) | В данном блокноте мы создаем базу на основе выгруженных данных.|
| [**Cian_data_processing**](https://github.com/SergeyTselunov/Cian/blob/main/Cian_data_processing.ipynb) |  В данном блокноте мы обрабатываем наш датафрейм.|
| [**Cian_geo**](https://github.com/SergeyTselunov/Cian/blob/main/Cian_geo.ipynb) | В данном блокноте мы производим геокодирование даных для поиска координат домов и метро.|
| [**Cian_EDA**](https://github.com/SergeyTselunov/Cian/blob/main/Cian_EDA.ipynb) | В данном блокноте мы проводим разведочный анализ данных.
| [**Cian_ML**](https://github.com/SergeyTselunov/Cian/blob/main/Cian_ML.ipynb) | В данном блокноте мы создаем модель, находим лучшие параметры и делаем предсказания.|
| [**cian.csv**](https://github.com/SergeyTselunov/Cian/blob/main/cian.csv) |  В данном файле csv содержится датафрейм созданный после парсинга.|
| [**cian_clean.csv**](https://github.com/SergeyTselunov/Cian/blob/main/cian_clean.csv) | В данном файле csv содержится датафрейм созданный после обработки данных.|
| [**cian_full.csv**](https://github.com/SergeyTselunov/Cian/blob/main/cian_full.csv) | В данном файле csv содержится датафрейм созданный после геокодирования.|
| [**cian_final.csv**](https://github.com/SergeyTselunov/Cian/blob/main/cian_final.csv) | В данном файле csv содержится датафрейм созданный после преобразования признаков.|
| [**url_final.txt**](https://github.com/SergeyTselunov/Cian/blob/main/url_final.txt) | В данном файле содержатся выгруженные ссылки для каждого объявления.|
| [**get_metrics.py**](https://github.com/SergeyTselunov/Cian/blob/main/get_metrics.py) | В данном файле находятся функции для расчета метрик.|

## `Наименование признаков`
- `Название` - Название объявления
- `Адрес` - Адрес квартиры
- `Метро` - Ближайшая станция метро
- `Время до метро` - Время до ближайшей станции метро (мин)
- `Цена` - Цена за квартиру (руб)
- <b>`Цена за квадрат` - Цена за квадратный метр (руб) (Целевой признак)</b>
- `Общая площадь` - Общая площадь (кв. метры)
- `Жилая площадь` - Жилая площадь (кв. метры)
- `Площадь кухни` - Площадь кухни (кв. метры)
- `Этаж` - Номер этажа из всех этажей дома 
- `Год постройки` - Год постройки дома
- `Тип жилья` - Вторичка или новостройка 
- `Высота потолков` - Высота потолков (метры) 
- `Санузел` - Количество и тип санузлов
- `Вид из окон` - Вид из окон
- `Ремонт` - Тип римонта
- `Строительная серия` - Строительная серия
- `Мусоропровод` - Наличие мусоропровода 
- `Количество лифтов` - количество лифтов в доме
- `Тип дома` - Тип дома
- `Тип перекрытий` - Тип перекрытий
- `Парковка` - Вид парковки
- `Подъезды` - Количество подъездов
- `Отопление` - Тип отопления
- `Аварийность` - Аварийность
- `Газоснабжение` - Наличие газоснабжения
- `Балкон/лоджия` - Количество и тип балкона/лоджии
- `Год сдачи` - Год сдачи квартир в доме
- `Дом` - Сдан или нет
- `Отделка` - Тип отделки 
- `Кол-во комнат` - количество комнат в квартире.
- `Широта метро, долгота метро` - координаты метро 
- `Широта дома, долгота дома` - координаты дома 
- `Расстояние до метро, расстояние до центра` - Расстояния до ближайшего метро и центра Москвы соответсвенно.
- `Округ` - Округ Москвы в котором находится квартира.
