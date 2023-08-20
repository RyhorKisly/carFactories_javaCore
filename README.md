# Тема проекта: Фабрики по созданию автомобилей (Car Factorries)

Цель проекта - реализовать функционал для создания автомобилей разных марок, 
на разных заводах, производить изменения на разных сервисах. 
Данные действия производить под управлением одного центрального звена: Автосалон.

___

## Особенности реализации проекта

В данном проекте продемонстрирована работа с основным функционалом JavaCore:
   - Реализованы принципы ООП (абстракция, наследование, инкапсуляция, полиморфизм);
   - классы и объекты
   - работа с типами данных,
   - операторами, 
   - циклами, 
   - массивами,
   - коллекциями (List, Set, Map),
   - Generics,
   - Исключениями (создание своих и обработка ошибок),
   - и т.д.

___


## Структуру классов и методов:

1) Класс "Car" представляет собой автомобиль.

   Имеет следующие свойства:
   * Цвет
   * Модель (неизменяемая)
   * Год выпуска (неизменяемый)
   * Размер колес
   * Объем двигателя (неизменяемая)
   * Список опций (Могут быть, а могут и нет)

   Автомобилю можно:
   * Сменить цвет
   * Изменять размер колес
   * Изменять список опций (Добавлять\Удалять)

В консоль выводится информации об автомобиле.

Создано 3 разных класса автомобилей содержащие уникальные поля различающиеся по типу данных. 

У каждой марки машины кроме уникальных полей также есть свои модели, свои цвета, свои размеры колес и свои объёмы двигателей.

2) Сервис.

   Имеет следующие возможности:
   * Изменять цвет автомобиля.
   * Изменять размер колес на автомобиле
   * Добавить\Удалить опцию. 
   * Для каждой задачи существует конкретный класс сервиса.
   	Например: сервис для покраски, или сервис для замены колёс.


3) Автозавод.

   Имеет следующие особенности:
   * Имеет список моделей которые может создавать. Этот список должен задаваться
   во время создания.
   * Имеет список с объемами двигателей которые можно установить на автомобиль.
   Этот список задаётся во время создания.
   * Имеет Список цветов в которые можно покрасить автомобиль. Этот список
   задаётся во время создания.
   * Имеет список размеров колес которые можно установить на автомобиль. Этот
   список задаётся во время создания.
   * Завод имеет склад, во время создания завода он производит некоторое кол-во
   автомобилей и хранит их на складе.

   Имеет следующие возможности:
   * Реализован вывод на печать возможных для производства
   цветов/объемов двигателей/моделей/размеров дисков
   * Реализована возможность создания авто по заказу салона. Однако если автомобиль есть на
   складе это авто использовано вместо создания нового.
   * Реализована возможность выбора со склада наиболее подходящего автомобиля
   и изменения его согласно заказу. 
   * Общее количество заводов 3 (Audi, BMW, Mercedes). 
   * На заводе возможно производить только автомобили которые допустимы на данном заводе.


4) Автосалон.

   - Используется для заказа автомобиля на заводе, или изменения уже существующего авто на сервисе. 
   - Салон может изменять автомобиль на необходимом сервисе.
   	Также заказ автомобиля происходит с нужного завода.

___

## Запуск проекта

Для проверки работоспособности проекта, необходимо запустить файл CarFactories/src/Main.java
