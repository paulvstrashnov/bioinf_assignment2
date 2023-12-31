## Лабораторная работа 2. Алгоритм Нидлмана-Вунша с ограниченной шириной диагонали \(k\)



Классический алгоритм NW использует подход динамического программирования для глобального выравнивания последовательностей и даёт оптимальное решение, рассматривая все возможные выравнивания. Однако при выравнивании длинных последовательностей или когда грубое решение уже известно, можно ограничить область поиска выравнивания. Один из вариантов - метод с ограничением ширины диагонали.

В алгоритме NW с ограниченной шириной диагонали \(k\) расчет матрицы динамического программирования ограничивается диагональной полосой шириной \(k\). Этот метод уменьшает время и сложность памяти, но выравнивание может быть не оптимальным, если настоящее выравнивание выпадает за пределы полосы.

## Задача

1. **Реализация**: Реализуйте версию алгоритма NW с ограниченной шириной диагонали \(k\). Функция должна принимать две последовательности равной длины, скоринг-функцию и ширину полосы \(k\) в качестве параметров.

2. **Тестирование**:
   - Используйте тестовые случаи из классической реализации NW для проверки вашей версии с ограниченной шириной диагонали \(k\). Некоторые из этих тестов могут не работать, если истинное выравнивание выпадает за пределы полосы. Определите такие случаи.
   - Разработайте дополнительные тестовые случаи специально для версии с ограниченной шириной диагонали \(k\), чтобы продемонстрировать ее эффективность и ограничения.
   - Чтобы проверить, был ли достигнут оптимальный результат, выполните алгоритм дважды с \(k\) и \(k+1\).

3. **Документация**: Добавьте комментарии к каждой функции/методу, объясняя ее назначение, входные данные, выходные данные и ключевые шаги или логику внутри.
