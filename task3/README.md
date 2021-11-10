Дедлайн: 24 ноября, 23.59.

Ноутбуки сохранять с названием в формате SurnameTask3.ipynb

Перед выполнением задания --- укажите себя в исполнителях, чтобы не было дублей.


# Оформление задания
Задание сдается в jupyter notebook. Структура:
* Заголовок ноутбука
* Описание задания
* Код
* Визуализация
* Краткий комментарий, выводы

Задание оценивается по критериям:
* Корректность
* Наглядность
* Адекватность кода
* Оформление результатов
* Перекрестная защита результатов


# Список заданий
1. [Исполнитель: TODO] Визуализировать матрицы ковариаций для каждого экстремума многоэкстремальной задачи классификации. Визуализацию проводить с помощью интерактивных графиков.  Модель: однослойная нейронной сеть. Выборка: произвольная, содержащая несколько экстремумов (допускается использование синтетических выборок). Априорное распределение параметров: нормальное распределение с положительно-определеннной матрицей ковариации (N(0, A^{-1})). Оптимизацию матрицы провести итеративным методом с использованием аппроксимации Лапласа. 
* [оптимизация гиперпараметров](http://strijov.com/papers/HyperOptimizationEng.pdf)

2. [Исполнитель: TODO]  Визуализировать эмпирическое распределение параметров модели в зависимости от значения $p$ для модели с L^p регуляризацией.  Модель: произвольная. Выборка: одна из стандартных датасетов sklearn. 
* [datasets](https://scikit-learn.org/stable/datasets/toy_dataset.html)

3. [Исполнитель: TODO]  Рассмотреть логистическую регрессию с двумя параметрами. Построить поверхность со следующими осями: w1, w2, sigma (оптимальный параметр априорного распределения для модели с параметрами [w1, w2]). Цветом поверхности задать значение апостериорной вероятности в точки поверхности. Модель: логистическая регрессия. Выборка: произвольная (допускается использование синтетических выборок или использование двух наиболее значимых параметров на одном из стандартных датасетов sklearn).  Априорное распределение параметров: нормальное распределение со скалярным параметром дисперсии дисперсией (N(0, sigma^2 * I)). Оптимальное значение sigma выбрать перебором.
* [datasets](https://scikit-learn.org/stable/datasets/toy_dataset.html)

4. [Исполнитель: TODO]  Построить интерактивный график зависимости апостериорного распределения параметров от количества параметров модели, sigma (оптимальный параметр априорного распределения для модели), эмпирической дисперсии параметров. Для каждого значения количества параметров в интерактивном графике построить поверхность с осями: sigma^2, эмпирическая дисперсия параметров, апостериорная вероятность параметров. Цвет каждой поверхности задать зависимым от Evidence. Модель: логистическая регрессия на полиномах различных степеней от одного признака.  Выборка: произвольная (допускается использование синтетических выборок или использование одного наиболее значимого параметра на одном из стандартных датасетов sklearn).  Априорное распределение параметров: нормальное распределение со скалярным параметром дисперсии дисперсией (N(0, sigma^2 * I)).
* [datasets](https://scikit-learn.org/stable/datasets/toy_dataset.html)
  
5. [Исполнитель: TODO] Повторить график 28.6 из книги MacKay. Выборка: одна из стандартных датасетов sklearn. Модели: несколько моделей линейной регрессии:
    1. соответствующая оптимальному значению Evidence, с оптимальными значениями гиперпараметров
    2. с сниженной дисперсией sigma^2 относительно оптимальных значений
    3. со смещением среднего значения параметров относительно оптимальных значений (см. график)
Априорное распределение параметров: нормальное распределение со скалярным параметром дисперсии дисперсией (N(0, sigma^2 * I)).
* [datasets](https://scikit-learn.org/stable/datasets/toy_dataset.html)
* [книга](http://www.inference.org.uk/itprnn/book.pdf)
* [оптимизация гиперпараметров](http://strijov.com/papers/HyperOptimizationEng.pdf)

6. [Исполнитель: TODO] Визуализировать KL-дивергенцию (в трех вариантах, KL(p1,p2), KL(p2,p1) и 0.5 KL(p1,p2) + 0.5 KL(p2,p1)) между истинным распределением выборки и распределением генератора GAN  зависимости от количества итераций оптимизации. Выборка: синтетическая. Модель GAN: максимально простая для сгенерированной выборки.

7. [Исполнитель: TODO] Визуализировать KL-дивергенцию (в трех вариантах, KL(p1,p2), KL(p2,p1) и 0.5 KL(p1,p2) + 0.5 KL(p2,p1)) между распределением логитов ученика и учителя в задаче дистилляции знаний. Визуализация должна выглядеть как график (поверхность) от температуры и важности слагаемого дистилляции. Выборка: CIFAR-10 (для ученика при оптимизации взять только первые 10% выборки). 
Модель учителя: предобученный ResNet, модель ученика: сверточная с небольшим количеством слоев. 
* [Про дистилляцию](http://strijov.com/papers/Grabovoy2021PL.pdf)
* [Предобученные модели и классы для них](https://github.com/passalis/pkth)

8. [Исполнитель: TODO] Повторить эксперимент из статьи Bishop (график 4). Визуализировать разделяющую поверхность как интерактивный график от числа размеченных объектов выборки и значимости каждого из слагаемых.
* [Статья](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/05/Bishop-Valencia-07.pdf)

9. [Исполнитель: TODO] Повторить эксперимент из статьи Bishop (график 4) с наивной реализацией генеративно-дискриминативной модели (формула 12 из статьи). Визуализировать разделяющую поверхность как интерактивный график от числа размеченных объектов выборки и значимости каждого из слагаемых.
* [Статья](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/05/Bishop-Valencia-07.pdf)

10. [Исполнитель: TODO] Нарисовать векторное поле для автокодировщика. Нарисовать heatmap по правдоподобию объектов выборка, получаемым с помощью вариационного автокодировщика. Сопоставить результаты. Выборки: несколько синтетических 2d выборок, аналогичных по сложности визуаилизированным в статье.
* [статья](https://jmlr.csail.mit.edu/papers/volume15/alain14a/alain14a.pdf)

11. [Исполнитель: TODO] Нарисовать зависимость качества классификации от разных видов Dataset Shift. Визуализация (несколькими графиками) должна показывать как меняется выборка в зависимости от значимости сдвига, как меняется качество классификации в зависимости от значиомсти сдвига. Выборки: несколько синтетических 2d выборок. 
* [статья](https://rtg.cis.upenn.edu/cis700-2019/papers/dataset-shift/dataset-shift-terminology.pdf)

12. [Исполнитель: TODO] Визуализировать message passage на фактор-графе для алгоритма Sum Product. В визуализации должны быть указаны указаны направления сообщений из message passing. Граф и параметры должны генерироваться случайно при каждом запуске визуализаии графа. Конфигурация сгенерированного графа должна быть отображена при отрисовке (через print или прямо в картинку). Формат визуализации - по шагам, через интерактивный график или анимацию в ноутбуке.
* [Bishop](http://users.isr.ist.utl.pt/~wurmd/Livros/school/Bishop%20-%20Pattern%20Recognition%20And%20Machine%20Learning%20-%20Springer%20%202006.pdf)
* [Пример с анимацией](https://jckantor.github.io/CBE30338/A.03-Animation-in-Jupyter-Notebooks.html)