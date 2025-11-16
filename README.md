# goit-algo2-hw-04
Algo homework 04

# Tasks
logistic.py -> Implementation of Edmonds-Karp algorithm
trie_task.py -> Implementation of extended Trie class

# Logistic task results
```
Terminal 1, Shop 1, Capacity 15
Terminal 1, Shop 2, Capacity 10
Terminal 1, Shop 3, Capacity 20
Terminal 1, Shop 4, Capacity 15
Terminal 1, Shop 5, Capacity 10
Terminal 1, Shop 6, Capacity 20
Terminal 1, Shop 7, Capacity 15
Terminal 1, Shop 8, Capacity 15
Terminal 1, Shop 9, Capacity 10
Terminal 2, Shop 4, Capacity 10
Terminal 2, Shop 5, Capacity 10
Terminal 2, Shop 6, Capacity 10
Terminal 2, Shop 7, Capacity 15
Terminal 2, Shop 8, Capacity 15
Terminal 2, Shop 9, Capacity 10
Terminal 2, Shop 10, Capacity 20
Terminal 2, Shop 11, Capacity 10
Terminal 2, Shop 12, Capacity 15
Terminal 2, Shop 13, Capacity 5
Terminal 2, Shop 14, Capacity 10
```
Застосувавши алгоритм Edmonds-Karp, ми можем побачити що до кожного магазину можливий максимальний потік від терміналу.

Термінал 2 забеспечує найбільший потік до магазинів, 140 проти 130 з Терміналу 1.

В нашій ситуації, найменший загальний потік маршруту витікає з найменшої capacity конкретного магазину, тобто найменший потік буде з Терміналу 2 до Магазину 13.

Магазин 5 отримав найменше товару, і зміна маршруту до нього не змінить нічого, адже це обмеження саме магазину, а не пропусктної здатності маршруту,

Вузькими місцями мережі є саме кінцева пропускна здатність до магазинів, адже пропускна можливість мережі наразі здатна забеспечити максимальний потік до кожного мазагину. Тобто для покращення ефективності мережі потрібно розширяти саме потік до кінцевих точок.
