﻿# polytech.cs.2017.spring_project
**Название проекта: Игра Жизнь**

## Информация о проекте


### Правила
* Место действия этой игры — «вселенная» — это размеченная на клетки поверхность или плоскость — безграничная, ограниченная, или замкнутая (в пределе — бесконечная плоскость).
* Каждая клетка на этой поверхности может находиться в двух состояниях: быть «живой»(заполненной) или быть «мёртвой» (пустой). Клетка имеет восемь соседей, окружающих её.
* Распределение живых клеток в начале игры называется первым поколением. Каждое следующее поколение рассчитывается на основе предыдущего по таким правилам:
\n 1) В пустой (мёртвой) клетке, рядом с которой ровно три живые клетки, зарождается жизнь;
\n 2) Если у живой клетки есть две или три живые соседки, то эта клетка продолжает жить; в противном случае, если соседей меньше двух или больше трёх, клетка умирает («от одиночества» или «от перенаселённости»)
* Игра прекращается, если
\n 1) На поле не останется ни одной «живой» клетки
\n 2) Конфигурация на очередном шаге в точности (без сдвигов и поворотов) повторит себя же на одном из более ранних шагов (складывается периодическая конфигурация)
\n при очередном шаге ни одна из клеток не меняет своего состояния (складывается стабильная конфигурация; предыдущее правило, вырожденное до одного шага назад)

Эти простые правила приводят к огромному разнообразию форм, которые могут возникнуть в игре.

Игрок не принимает прямого участия в игре, а лишь расставляет или генерирует начальную конфигурацию «живых» клеток, которые затем взаимодействуют согласно правилам уже без его участия (он является наблюдателем).
### Интерфейс
![Image alt](https://github.com/Stig0/polytech.cs.2017.spring_project/raw/master/src/res/play_fon.jpg)
### Структура проекта
Организация проекта:

Поддиректории| Описание
-------------|-------------------
src/         | программные файлы 
src/tests    | тесты 
doc/         | Документация 
res/         | ресурсы проекта

### Сборка
Для сборки проекта пропишите:
````
make
````
Удалить все собранные файлы:
````
make clean
````
Для сборки тестов:
````
make D_UNITY=../Unity check
````
Для сборки документации:
````
make doxygen
````
Для сборки документации в формате PDF:
````
make pdf
````
Для сборки документации в формате HTML:
````
make html
````

## Авторы
* **Николаев Денис** - den11nik@yandex.ru
* **Пузько Данила** - danilapuzko@mail.ru
## Лицензия
Этот проект лицензирован под MIT License - смотри [LICENSE](LICENSE) файл для подробностей
