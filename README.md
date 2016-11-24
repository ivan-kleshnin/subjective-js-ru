# Субъективный JS

Остросюжетный гайд по языку.

## От автора

Данная книга предназначена для самостоятельного изучения JS как второго (третьего...) языка.
От читателя ожидается базовое понимание Computer Science. Основной акцент сделан на особенности JS,
выделяющие его среди остальных языков, неочевидные и малоочевидные вещи.

Автор текста имеет опыт коммерческого программирования на трёх языках, некоммерческого – на 15+.
Его целью было создание информативного, но захватывающего гайда для "самого себя в прошлом".
Основная идея – изучение по аналогии – была дополнена взглядом на язык с разных ракурсов:
парадигм, истории, конкуренции, контр-примеров и поиска истины.

## [Мотивация](./0.1.motivation.md)

## [Переводы терминов](./0.2.translations.md)

## Вступление

JS часто воспринимается как простой язык и учится как [набор трюков](https://github.com/loverajoel/jstips),
заменяющих реальное знание. – Я знаю JS! – утверждает персонаж, использующий `alert` для отладки...
Несложно встретить и противоположный взгляд, по которому JS – это полностью
сломанный язык, непроходимая PITA. Мнение подкрепляется специально отобранными "ужасающими" примерами
(не встречающимися на практике).

Оба мнения расходятся с реальностью. JavaScript (в редакции ES 2016-2017) – это сравнительно
сложный язык, обладающий огромной грамматикой. Выразительные возможности JavaScript находятся на одном уровне с Python и Ruby.

JavaScript сложно выучить на однообразных задачах, возникающих в коммерческих проектах.
В то же время, значительный процент "знаний" составляют deprecated синтаксические единицы и паттерны.
В повседневной практике следует ограничивать себя отобранным подмножеством языка.

Официальное название спецификации JavaScript: EcmaScript. Разница связана с лицензиями и не представляет
особого интереса. Мы будем использовать термин JS или JavaScript в качестве названия языка и
ES5, ES6, ES2015, ES2016 для ссылок на конкретные версии.

Все версии языка, на данный момент, обладают 100% обратной совместимости.
Ни авторы ES, ни сообщество пока не смогли выработать удовлетворительного механизма удаления фич.
Небольшие исключения типа `"use strict"` можно вынести за скобки.

Ситуацию спасает практически полное отсутствие стандартных библиотек в языке. Да, да – это огромный плюс!
Python сообщество показало всем убедительный контр-пример. "Batteries included", вначале, играет всем на пользу.
Затем, из-за увязки обновления библиотек с выпуском новых версий языка, – превращает всё в археологический музей.
Стандартные пакеты Python забагованы, устарели, разлагаются. Но, вопреки всеобщей ненависти, продолжают использоваться, как "стандартные"...

JS, безусловно, страдает от противоположной крайности, однако появление Node и NPM в корне изменило ситуацию.
Проблем с поиском библиотек в экосистеме практически нет. Вероятно, даже число научных библиотек в JS превысит оное в Python,
в обозримом будущем.

Проблема с "избытком альтернатив" является меньшим злом. Конкуренция – двигатель прогресса, а
культура написания документации в JS сообществе находится на сравнительно высоком уровне
Достаточно сказать, что на титульных страницах документаций нередко можно встретить перечень отличий от "конкурентов".
Положа руку на сердце – о таком уровне большинство программистских сообществ могут лишь мечтать.
Возьмите PHP с его бесчисленными "фреймворками", ничем не отличающимися друг от друга.
Возьмите выдохшийся Java. Возьмите тот же Python. И так далее.

## Как читать эту книгу

Данная книга посвящёна JavaScript и не затрагивает вопросы API (DOM, HTTP, и т.д.). Однако, примеры кода
будут содержать `console.log`, которая не является частью языка. Впрочем, и NodeJS и Браузеры
предоставляют данную функцию и, вероятно, её стандартизация – вопрос времени.
Также, при необходимости показать функцию из сторонней библиотеки, мы будем использовать синтаксис CommonJS.
Окончательная стандартизация ES модулей ожидается в 2017 году, после чего материал будет обновлён.

Желающим запускать примеры предлагается:

* установить [NodeJS](https://nodejs.org/en/) (и редактор, если вы форматировали диск)
* копировать тексты примеров в отдельные файлы
* запускать файлы из консоли командой вида `$ node exampleX.js`

Автор книги стремился сделать ВСЕ примеры максимально простыми и понятными с первого взгляда.
Если вы испытываете сложность с пониманием какого-либо абзаца или примера при последовательном чтении –
открывайте соотв. Issue.

## Содержание

### 1. Основы

### [1.1 Примеры синтаксиса](./1.1.syntax-examples.md)

### [1.2 Инструкции, Декларации, Выражения](./1.2.statements-declarations-expressions.md)

### [1.3 Элементы первого порядка](./1.3.first-class-elements.md)

## 2. Система типов

### [2.1 Слабая динамическая типизация](./2.1.weak-typing.md)

### [2.2 Примитивы и Объекты](./2.2.primitives-and-objects.md)

### [2.3 Проверка типов](./2.3.type-checking.md)

### [2.4 Обёрточные классы](./2.4.wrapper-classes.md)

### [2.5 Коэрция типов](./2.4.type-coercion.md)

### [2.6 Практические правила](./2.4.practical-rules.md)

## 3. Переменные и скоупинг

### [3.1 Скоупинг](./2.1.scoping.md)

### [3.2 Хойстинг](./2.2.hoisting.md)

## 4. Встроенные типы

### [4.1 Undefined и Null](./3.1.undefined-and-null.md)

### [4.2 Булеаны](./3.2.boolean.md)

### [4.3 Числа](./3.3.number.md)

### [4.4 Строки](./3.4.string.md)

### [4.5 Записи](./3.5.object.md)

### [4.6 Массивы](./3.6.array.md)

### [4.7 Даты](./3.7.date.md)

### [4.8 Регулярки](./3.8.regex.md)

## 5. Прототипная модель

## 6. Динамический this

## Эквивалентность

a === b is a shorthand for
typeof a == typeof b && a == b

Одна из наиболее проблематичных областей JS. Язык определяет две функции `==` и `===` для всех типов.
Здесь и далее, мы отождествляем операции и функции поскольку первые и вторые отличаются лишь синтаксически.
С точки зрения функционального программирования, `+`, `*`, `==` и другие являются инфиксными функциями от
 двух аргументов.

Разница между `==` и `===` выглядит очень простой:
Функция `==` задействут автокоэрцию для примитивов. Функция `===` не задействует автокоэрцию для объектов.

```js
1 == "1"  // true
1 === "1" // false
```

Отсюда видно, что популярная рекомендация "всегда использовать `===`" не имеет никакого фундамента, а
является обычным "заклинанием реальности". JS сообщество выработало и догматически следует нескольким
таким мантрам. К сожалению, никакой практической пользы от них нет.

Оптимальной реакцией на сравнения двух разных типов является исключения этапа компиляции.
Следующим по оптимальности – исключение этапа выполнения (рантайм).
Наименее оптимальным – автоприведение типов. Независимо от полученного ответа (`true` или `false`),
ваша программа содержит логическую ошибку, если полагается на автокоэрцию. Нет никаких оснований
полагать, что `false` лучше `true` в данном случае. "Не равны" и "нельзя сравнивать" – два взаимоисключающих
утверждения...

Как было указано выше, для объектов автокоэрция не выполняется и `==` и `===` ведут себя идентично.
Строгие аналоги для операций `>`, `<`, `>=`, `<=` также не определены.

Исходя из вышесказанного, использование `===` вместо `==` являтся неудачной попыткой паллиативного решения.
Строгое сравнение не поможет вам ни найти баг, ни предотвратить его.

Операции сравнения для объектов в JS не определены:

```js
[] == []  // false
[] === [] // false
{} == {}  // false
{} === {} // false
``

Для сравнения объектов рекомендуется использовать библиотечные функции:

```js
let R = require("ramda")
R.equals([], []) // true
```

При правильной реализации, подобные функции поддерживают вложенные структуры и диспатчинг
на методы класса, т.е. работают с открытым множеством классов.

Сравнение с возможностью `null` и `undefined` (см. далее) следует выполнять в два этапа:

```js
if (R.isNil(x)) {
 if (equals(x, y)) {
   ...
 } else {
   ...
 }
} else {
  ...
}
```

Тело `R.isNil` эквивалентно `return x === undefined || x === null`





## Книги

* [Speaking JavaScript](http://speakingjs.com/es5/index.html)
* [Exploring ES6](http://exploringjs.com/es6/index.html)
* [Exploring ES2016-ES2017](https://leanpub.com/exploring-es2016-es2017/read)

## Разное





http://www.2ality.com/2013/01/categorizing-values.html










ХОЙСТИНГ И ОБЪЯСНЯТЬ БЛИЖЕ К КОНЦУ

сначала показать доступные примеры функций с function без зауми




Возврат значения из конструктора
сбрасывает байду только для значений (О) типов.
Ну и дела...



https://github.com/loverajoel/jstips/blob/gh-pages/_posts/en/2016-08-25-keyword-var-vs-let.md
Говорят, что `let` не хойстится. Но тогда




JS наиболее последовательно реализует идею Динамической Типизации и отказывается от классов
в пользу прототипов. Нотация `class`, добавленная в последних версиях языка, является лишь тонкой
надстройкой над ними. Роль интерфейсов же играет т.н. Утиная Типизация. Интерфейсы как отдельные сущности
не формализованы и не декларируются, однако мы можем говорить об имплицитных интерфейсах (интерфейсах "по факту").











FIXME -- декларация не является инструкцией!!!



## Поддержать проект

Данный проект является некоммерческим. Автор вложил в него более сотни часов свободного времени.
Поддержите данный проект, поставив ему звезду &starf; в правом верхнем углу и поделившись ссылкой
со знакомыми.






What is javascript

JavaScript’s nature can be summarized as follows:
It’s dynamic
Many things can be changed. For example, you can freely add and remove properties (fields) of objects after they have been created. And you can directly create objects, without creating an object factory (e.g., a class) first.
It’s dynamically typed
Variables and object properties can always hold values of any type.
It’s functional and object-oriented
JavaScript supports two programming language paradigms: functional programming (first-class functions, closures, partial application via bind(), built-in map() and reduce() for arrays, etc.) and object-oriented programming (mutable state, objects, inheritance, etc.).
It fails silently
JavaScript did not have exception handling until ECMAScript 3. That explains why the language so often fails silently and automatically converts the values of arguments and operands: it initially couldn’t throw exceptions.
It’s deployed as source code
JavaScript is always deployed as source code and compiled by JavaScript engines. Source code has the benefits of being a flexible delivery format and of abstracting the differences between the engines. Two techniques are used to keep file sizes small: compression (mainly gzip) and minification (making source code smaller by renaming variables, removing comments, etc.; see Chapter 32 for details).
It’s part of the web platform
JavaScript is such an essential part of the web platform (HTML5 APIs, DOM, etc.) that it is easy to forget that the former can also be used without the latter. However, the more JavaScript is used in nonbrowser settings (such as Node.js), the more obvious it becomes.

Bad and Good

  Quirks and Unorthodox Features
  On one hand, JavaScript has several quirks and missing features (for example, it has no block-scoped variables, no built-in modules, and no support for subclassing). Therefore, where you learn language features in other languages, you learn patterns and workarounds in JavaScript. On the other hand, JavaScript includes unorthodox features (such as prototypal inheritance and object properties). These, too, have to be learned, but are more a feature than a bug.
  Note that JavaScript engines have become quite smart and fix some of the quirks, under the hood. For example:
  Specification-wise, JavaScript does not have integers, only floating-point numbers. Internally, most engines use integers as much as possible.
  Arguably, arrays in JavaScript are too flexible: they are not indexed sequences of elements, but maps from numbers to elements. Such maps can have holes: indices “inside” the array that have no associated value. Again, engines help by using an optimized representation if an array does not have holes.

  Elegant Parts

  But JavaScript also has many elegant parts. Brendan Eich’s favorites are:[3]
  First-class functions
  Closures
  Prototypes
  Object literals
  Array literals
  The last two items, object literals and array literals, let you start with objects and introduce abstractions (such as constructors, JavaScript’s analog to classes) later. They also enable JSON (see Chapter 22).
Note that the elegant parts help you work around the quirks. For example, they allow you to implement block scoping, modules, and inheritance APIs—all within the language.



Influences
  JavaScript was influenced by several programming languages (as shown in Figure 3-1):
  Java is the role model for JavaScript’s syntax. It also led to JavaScript’s partitioning of values into primitives and objects and to the Date constructor (which is a port of java.util.Date).
  AWK inspired JavaScript’s functions. In fact, the keyword function comes from AWK.
  Scheme is the reason that JavaScript has first-class functions (they are treated like values and can be passed as arguments to functions) and closures (see Chapter 16).
  Self is responsible for JavaScript’s unusual style of object orientation; it supports prototypal inheritance between objects.
  Perl and Python influenced JavaScript’s handling of strings, arrays, and regular expressions.
  Beyond the actual language, HyperTalk influenced how JavaScript was integrated into web browsers. It led to HTML tags having event-handling attributes such as onclick.

http://speakingjs.com/es5/images/spjs_0701.png
