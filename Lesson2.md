Всем привет, сегодня у нас второе занятие, а это значит что мы еще на шаг ближе к JS

Сначала я хочу поделиться электронным учебником (*кстати он бесплатный*), который помогал мне 
(https://learn.javascript.ru/)

А теперь новая задачка

## Задача. Ввод и вывод данных Задача «Дележ яблок»

Условие n школьников делят k яблок поровну, неделящийся остаток остается в корзинке. Сколько яблок достанется каждому школьнику? Сколько яблок останется в корзинке? Программа получает на вход числа n и k и должна вывести искомое количество яблок (два числа).

Во всех задачах считывайте входные данные через input() и выводите ответ через print().

* Примеры входных данных: *
6
50
* Примеры выходных данных: *
8
2

Для начала добавим в наш словарь (*надеюсь вы пишите конспекты*) несколько новых выражений

Одна из часто используемых операций при работе с числами – это округление.

В JavaScript есть несколько встроенных функций для работы с округлением:

 ###### Math.floor
Округление в меньшую сторону: 3.1 становится 3, а -1.1 — -2.
###### Math.ceil
Округление в большую сторону: 3.1 становится 4, а -1.1 — -1.
###### Math.round
Округление до ближайшего целого: 3.1 становится 3, 3.6 — 4, а -1.1 — -1.
###### … % … - деление без остатка

### А вот и готовое решение

```
let n = parseInt(prompt())
let k = parseInt(prompt())
console.log(Math.floor(k/n))
console.log(k%n)
```


