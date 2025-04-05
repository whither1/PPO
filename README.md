# Минёр против сапёра

## Идея
Игра представляет собой переосмысление известной компьютерной "сапёр", но с добавлением второго игрока - "минёра".

## Правила
До начала игры устанавливаются: размер поля, стартовая клетка сапёра, размер стартовой зоны сапёра, размер рабочей зоны минёра, начальное положение рабочей зоны, количество мин, которое можно будет выставить или передвинуть за ход и количество мин, которое можно будет выставить до начала игры, максимальное количество мин. После начала игры минёр размещает заданное количество мин в стартовой зоне и передает ход сапёру, который начинает свой ход нажатием на стартовую клетку. После открытия области сапёр отмечает все найденные мины и передает ход минёру. В свой ход минёр может поставить или передвинуть мины, запросить перемещение рабочей зоны и закончить свой ход. Минёр может ставить и перемещать мины только в рабочей зоне. Рабочую зону можно перемещать только на территорию, примыкающую к границам существующей зоны. Минёр не обязан размещать или перемещать мины для завершения хода. Минёр не может перемещать мины, уже отмеченные сапёром, выставлять и перемещать мины на уже открытую область. Сапёр в свой ход может открыть одну клетку в своей области, отметить сколько угодно мин и закончить свой ход.
Игра заканчивается победой сапёра, если сапёр открыл всё поле и отметил все мины, или победой минёра, если сапёр подорвался на мине.

## Описание предметной области
Проект представляет собой асимметричную многопользовательскую игру в жанре стратегического противостояния, где два игрока берут на себя противоположные роли: минёр скрытно расставляет мины на игровом поле, создавая ловушки, а сапёр анализирует поле, пытаясь обезвредить все мины, избегая подрыва. Цель минёра - заманить соперника в ловушку, используя хитрое расположение мин, а цель сапёра - разгадать замысел оппонента, помечая мины флагами и открывая безопасные клетки. Игра сочетает элементы логики и тактического планирования, предлагая динамичное соревнование между созданием и разгадыванием опасных паттернов.

## Use-Case диаграмма
![Use-Case](docs/img/use-cases.svg)

## ER-диаграмма
![ER](docs/img/er.svg)

## User-flow
### Открытие клетки
![User-Flow-Open-Tile](docs/img/user-flow-open-tile.svg)
### Перемещение мины
![User-Flow-Move-Mine](docs/img/user-flow-move-mine.svg)

## Стек приложения
Desktop приложение под Linux на языке Java.

## Разбиение на компоненты
![Component-Division](docs/img/comp-division.svg)

## UML диаграммы компонента доступа к данным и компонента с бизнес-логикой
![UMLs](docs/img/uml.svg)