Определился с официальным руководителем. Им будет Лев Владимирович Уткин.

Прочёл некоторые статьи, из которых три заслуживают упоминания:
1. Consistency-based semi-supervised learning for object detection / NeurIPS 2019.
Основная идея: самый продвинутый сейчас метод SSL для классификации - Consistency-Based SSL, но в задаче SSL для детекции объектов до сих пор, как правило, используется более примитивная технология Semi-Supervised Data Mining: алгоритм обучается на размеченной части выборки; после этого выбираются участки изображений из неразмеченной части, на которых этот алгоритм с высокой уверенностью что-то распознаёт, эти кусочки вырезаются и с присвоенными псевдо-метками добавляются в тренировочный набор, после чего процесс повторяется.
Процесс медленный: после каждой итерации обучения обрабатываем все неразмеченные данные.
Consistency-based не применяли ранее, т. к. (так пишут в статье) не совсем понятно, как при внесении возмущений в изображения понять, оказались ограничивающие рамки на том же месте или на ином (комментарий: мне не очень понятно, почему им непонятно.
Сдвинули камеру влево на X, рамка тоже должна отъехать на X и т. д).
Поэтому авторы статьи предлагают вместо поворотов и сдвигов просто зеркально отражать изображения и считать, что ограничивающие рамки должны совпадать с точностью до зеркального отражения.
Впрочем, у авторов не очень получается (требование симметрии делает фильтры нейросети симметричными), распознавание улучшается лишь ненамного.
2. In defence of pseudo-labeling: an uncertainty-aware pseudo-label selection framework for semi-supervised learning (2020).
Исследуется проблема классификации.
Утверждается, что, должным образом организовав процесс, можно добиться того же качества обучения с «обычными» псевдо-метками, что и при consistency-based.
3. Deep Clustering for unsupervised learning of visual features (2019, Facebook AI Research).
Статья про обучение без учителя (кластеризация) в применении к классификации.
Современные методы обучения без учителя успешно конкурируют с полуконтролируемым обучением.

Попытался поизучать Angelina Braille Reader и связаться с автором, Ильёй Геннадиевичем Оводовым.
Написал ему письмо, а также добавил в его программу перевод в греческие символы и оформил pull request.
Pull Request он посмотрел, на письмо пока не ответил.

Дальнейшие планы:
- поскольку ещё не писал никогда CNN (которые используются в качестве базовой модели для SSL for detection), начал и буду продолжать смотреть лекции курса “Convolutional Neural Networks” от известного популяризатора ML Andrew NG на Coursera,  а также постараюсь почитать, как писать CNN на tensorflow
- Буду продолжать читать статьи, в том числе по Semi–Supervised Data Mining
