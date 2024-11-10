Вимоги до кожного варіанту:
Напишіть програму, яка обробляє великі масиви різних чисел різними
потоками в асинхронному режимі.
Масиви потрібно заповнювати рандомними числами, згенерованими у
заданому діапазоні. Діапазон повинен задавати користувач. Кількість елементів
в масиві від 40 до 60.
Для обробки масиви потрібно розбивати на частини (наприклад, 1-100,
101-200 і т.д.), частини масиву потрібно обробляти в окремих потоках.
Використовуйте Future для збору та виводу результатів. Також останнім
рядком виводьте на екран час роботи програми.
Впишіть у логіку програми перевірки isDone() та isCancelled().

Створіть Callable, який приймає масив чисел і повертає масив
попарних добутків (кожен парний елемент множиться на непарний:
перший на другий, третій на четвертий і т.д.). Розбивайте масив на
частини, кожну з яких обробляє окремий потік, використовуючи
Future, щоб зібрати результати в один масив.
Діапазон [0; 100] – цілі числа. Використати CopyOnWriteArraySet.

Короткий опис проєкту:
У цьому коді реалізована програма, яка обробляє великі масиви цілих чисел, розбиваючи їх на частини для асинхронної обробки різними потоками. 
Масив заповнюється випадковими числами в межах, заданих користувачем, і обробляється шляхом розрахунку попарних добутків чисел (кожен парний елемент множиться на наступний непарний). 
Програма використовує Callable для обчислення попарних добутків у частинах масиву, кожна з яких передається окремому потоку. 
Результати зберігаються у CopyOnWriteArrayList, а для синхронізації результатів використовуються Future. 
Також у коді перевіряється статус виконання isDone() та isCancelled() кожного потоку, і виводиться час роботи програми в мілісекундах.
