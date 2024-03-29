# Практическое задание 1

1. Создать в файле `worker.py` класс `Worker` для расчета зарплаты сотрудников.

   У класса `Worker` должен быть с атрибут `tax_rate` равный 10 (процент налогов).

   У класса `Worker` должен быть конструктор, который принимает один строковый аргумент (имя сотрудника) и один числовой аргумент (размер оклада). Конструктор должен сохранить имя сотрудника в атрибут `name`. Конструктор также должен сохранить размер оклада в другой атрибут объекта (идентификатор придумайте самостоятельно).

   У класса `Worker` должен быть метод `salary()` который возвращает зарплату без учета налогов (просто возвращает размер оклада).

   У класса `Worker` должен быть метод `tax()` который возвращает размер налога от зарплаты (используйте метод `salary()`).

2. Создать в файле `bonus_worker.py` производный класс `BonusWorker` (на базе класса `Worker`).

   Конструктор класса `BonusWorker` должен принимать один строковый аргумент (имя сотрудника) и два числовых аргумента (размер оклада и процент надбавки). Для сохранения имени сотрудника и размера оклада он должен использовать конструктор базового класса и затем должен задать атрибут объекта для хранения процента надбавки (идентификатор придуймате самостоятельно).

   Метод `salary()` у `BonusWorker` должен возвращать оклад увеличенный с учётом процент надбавки.

   Класс `BonusWorker` не должен переопределять метод `tax()`.

3. Написать в файле `main.py` функцию `format_worker()` которая принимает объект класса `Worker`. Функция должна вернуть строку с четыремя колонками:

   * имя сотрудника (ширина 30 символов)
   * зарплата без учета налогов с 2 знаками после запятой (ширина 10 символов)
   * налоги с 2 знаками после запятой (ширина 10 символов)
   * зарплата с вычтенным налогом с 2 знаками после запятой (ширина 10 символов)

   Каждая колонка должна быть отформатирована с помощью форматных строк до необходимой ширины. Числовые значения нужно форматировать без ведущих нулей.

   Колонка с именем сотрудника должна быть выровнена влево, остальные колонки — вправо.

   Примеры результата:

```
Иван Петров                     50000.00    500.00  45000.00
```

   При импорте файла `main.py` не должен вызываться посторонний код.

[Примеры строк форматирования](https://pyformat.info/)
