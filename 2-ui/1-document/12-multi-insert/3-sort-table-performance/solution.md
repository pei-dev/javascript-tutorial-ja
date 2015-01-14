Для сортировки нам поможет функция `sort` массива.

Общая идея лежит на поверхности: сделать массив из строк и отсортировать его. Тонкости кроются в деталях.

В ифрейме ниже загружен документ, описывающий и реализующий разные алгоритмы. Обратите внимание: разница в производительности может достигать нескольких раз!

[iframe height=800 border=1 src="solution" link edit]

P.S. Создавать `DocumentFragment` здесь ни к чему. Можно вытащить из документа `TBODY` и иметь дело с ним в отрыве от DOM (алгоритм 4).

P.P.S. Если нужно сделать много узлов, то обычно `innerHTML` работает быстрее, чем генерация элементов через DOM-вызовы. Но в данном случае мы не создаём элементы, а сортируем и перевставляем готовые, так что результаты могут отличаться.