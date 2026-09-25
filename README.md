# Паттерны ООП — учебный репозиторий

Документация, реализации и тесты паттернов проектирования на PHP.
Репозиторий используется как учебная программа: каждый паттерн разбирается
по шагам — от проблемы и «кода до» к решению, тестам и анти-паттернам.

## Структура

```
docs/        теория: учебный план, шпаргалки, разборы
patterns/    реализации, сгруппированные по категориям (GoF)
  Creational/
  Structural/
  Behavioral/
tests/       тесты к реализациям (PHPUnit)
examples/    запускаемые сценарии из консоли
```

Внутри каждой директории паттерна:

```
patterns/<Категория>/<Паттерн>/
  README.md   проблема, решение, диаграмма, когда применять, анти-паттерны
  src/        реализация
  tests/      тесты (в общей директории tests/, если нужно общее состояние)
  Example.php запускаемый пример
```

## Как запустить

```bash
composer install
composer test
php examples/<Category>/<Pattern>/Example.php
```

Требуется PHP >= 8.2.

## Как здесь учиться

1. Открыть `docs/curriculum.md` и взять следующий непройденный паттерн.
2. Прочитать `README.md` паттерна: сначала раздел «Проблема», не читая реализацию.
3. Сравнить с `patterns/<Категория>/<Паттерн>/src/` и запустить тесты.
4. Сделать упражнения из раздела «Упражнения».
5. Отметить прогресс в `docs/curriculum.md` и сделать коммит.

## Категории паттернов

| Категория | Назначение | Паттерны |
|---|---|---|
| Порождающие (Creational) | Как объекты создаются | Singleton, Factory Method, Abstract Factory, Builder, Prototype, Object Pool |
| Структурные (Structural) | Как объекты взаимодействуют | Adapter, Bridge, Composite, Decorator, Facade, Flyweight, Proxy |
| Поведенческие (Behavioral) | Как объекты распределяют ответственность | Chain of Responsibility, Command, Iterator, Mediator, Memento, Observer, State, Strategy, Template Method, Visitor |

Подробности и порядок изучения — в [`docs/curriculum.md`](docs/curriculum.md).

## Лицензия

MIT
