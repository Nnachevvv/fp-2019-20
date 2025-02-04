Упражнение 8
============

Задачи
------
За решаването на задачите използвайте основните процедури за работа с потоци,
дефинирани в [stream.scm](stream.scm).

1. Дефинирайте процедура `(repeat value)`, която връща безкраен поток, който
генерира стойности `value`.

   ```scheme
   (repeat 1) ; 1, 1, ..., 1, 1, ...
   (repeat '(1 2 3)) ; (1 2 3), (1 2 3), ..., (1 2 3), (1 2 3), ...
   ```

2. Дефинирайте процедура `(cycle l)`, която връща безкраен поток, който генерира
елементите на списъка `l`.

   ```scheme
   (cycle (1)) ; 1, 1, ..., 1, 1, ...
   (cycle (1 2 3)) ; 1, 2, 3, 1, 2, 3, 1, ...
   ```

3. Дефинирайте процедура `(iterate f x)`, която връща безкрайния поток
`x, f(x), f(f(x)), f(f(f(x))), ...`.

4. Питагорова тройка наричаме наредената тройка от числа (a, b, c) такава, че
a<sup>2</sup> + b<sup>2</sup> = c<sup>2</sup>. Дефинирайте поток
`pythagorean-triples` от Питагоровите тройки (a, b, c) такива, че 1 ≤ a ≤ b ≤ c,
където a, b и c са цели числа.
