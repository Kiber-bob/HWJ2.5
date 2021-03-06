Jacoco включает в себя счетчики покрытия в различных масштабах, включая уровень команд, ветви, цикломатическую сложность, линии, методы (неабстрактные методы), класс (классы).

INSTRUCTION: Самая маленькая единица, которую вычисляет Jacoco, является инструкцией байт-кода. Охват инструкций указывает, какие инструкции были выполнены, а какие не были выполнены во всех инструкциях. Этот индекс полностью независим от исходного формата и действителен при любых обстоятельствах и не требует отладочной информации для файлов классов.
 
BRANCH: Jacoco рассчитывает покрытие ветви для всех инструкций if и switch. Этот индикатор будет подсчитывать количество всех ветвей и одновременно тратить, какие ветви выполняются, а какие не выполняются. Этот показатель также действителен в любом случае. Обработка исключений не рассматривается в рамках ветви.

С помощью отладочной информации точки ветвления могут быть сопоставлены с каждой строкой в ​​исходном коде и выделены.
* Красный бриллиант: нет покрытия, ветки не выполнены.
* Желтый бриллиант: частично покрытый, частично разветвленный.
* Зеленый бриллиант: полное покрытие, все ветки выполнены.

LINE: этот индекс рассчитывается с помощью информации отладки.

Поскольку каждая строка кода может генерировать несколько инструкций байт-кода, мы используем три разных состояния для представления покрытия строки
* Красный фон: нет покрытия, все инструкции в этой строке не выполняются.
* Желтый фон: частичное покрытие, некоторые инструкции в этой строке выполнены.
* Зеленый фон: полное покрытие, все инструкции в этой строке выполнены.