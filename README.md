# Java Parcs - Prime Number

[Base](https://github.com/lionell/labs/tree/master/parcs)

У лабораторній роботі було створено дві ноди в регіоні europe-west6 (`app`, `hosts-server`) та по 4 ноди в зонах europe-west4 (`daemon-1`-`daemon-4`), europe-west3(`daemon-5`-`daemon-8`). Така структура проекту була обрана оскільки в google cloud встановлені обмеження на кількість нод на зону.

Тести: 

| tests\nodes        | node 1| node 2|node 3|node 4|node 8|
| ------------- |--------:| -----:| -----:| -----:|-----:|
| test 1       |15.13	|7.803	|6.507	|4.59|**5.712**|
| test 2       |15.192	|8.773|	5.794|	4.665|	3.621|
| test 3       |14.927	|8.933|	6.283|	4.598|	3.604|
| test 4       |14.949	|8.946|	5.763|	4.836|	3.612|
| test 5       |14.533	|9.03	|6.257	|4.656|	3.618|
| Mean       |14.9462|	8.697	|6.1208	|4.669	|4.0334|


При використанні 8 нод перший запуск був явно довше ніж очікувався, проте все інші розпаралелились як треба і всі інші були.
