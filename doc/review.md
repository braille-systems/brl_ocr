# Обзор 24 мая 2021 г.
## Google: [braille character detection convolutional network](https://www.google.com/search?q=braille+character+detection+convolutional+network&oq=braille+character+detection+convolutional+network)
1. [Gonçalves, 2020](https://sol.sbc.org.br/index.php/wvc/article/download/13492/13340/). Braille character detection using deep neural
networks for an educational robot for visually
impaired people.
**Ерунда. Распознают не бумажные символы Брайля, а искусственно сделанные увеличенные символы (ещё и точки покрашены).**
1. [Smelyakov, 2018](https://ieeexplore.ieee.org/document/8478615). Braille Character Recognition Based on Neural Networks.
**Видимо, тоже ерунда. Только планы, даже без датасета.**
1. [Ovodov, 2020](https://arxiv.org/ftp/arxiv/papers/2012/2012.12412.pdf). Optical Braille Recognition Using Object Detection
CNN. **Статья Ильи Оводова из Москвы.**
1. [Prakash, July 2020](http://wthtjsjs.cn/gallery/26-whjj-july-5558.pdf). Braille Recognition using Convolutional Neural Networks.
**Работа интересная, собран датасет из 14 000 брайлевских букв (букв, не страниц).
Но CNN использована только на этапе классификации символов, детекция происходит геометрическими методами, а 
это не подходит для фото, сделанных на смартфон! Только для качественных сканов!**
1. [Subur, 2015](https://iptek.its.ac.id/index.php/jps/article/view/1048/941). Braille Character Recognition Using Artificial
Neural Network. **Неинтересно, детекция геометрическими методами. Система не работает вообще, если лист повёрнут более, чем на 1 градус**.
1. [AlSalman, 2021](https://www.techscience.com/cmc/v67n3/41628/pdf) A Deep Learning-Based Recognition Approach for the
Conversion of Multilingual Braille Images. **Тоже не очень интересно. При детекции вращают картинку, пока не найдут параллельные линии. Конечно же, это подходит не для всех изображений**.
1. [Baumgärtner, 2020](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7972593/). Image-Based Recognition of Braille Using Neural Networks on Mobile Devices. **Опять начинают с детекции прямых брайлевских линий (правда, используют для этого Faster R-CNN, а не геометрию). Разработали Android-приложение и сервер на Tensorflow, в этом смысле молодцы. Используют вспышку для равномерного освещения. Может, это и может работать, но ведь брайлевские линии обычно не прямые, а кривые!**

## Google Scholar: 5 статей, которые цитируют статью китайцев
Сама статья китайцев: [Li 2020](https://openaccess.thecvf.com/content_CVPRW_2020/html/w34/Li_Optical_Braille_Recognition_Based_on_Semantic_Segmentation_Network_With_Auxiliary_CVPRW_2020_paper.html), Optical Braille Recognition Based on Semantic Segmentation Network With Auxiliary Learning Strategy.

Поиск: https://scholar.google.com/scholar?cites=11115639400057108047&as_sdt=2005&sciodt=0,5

1. [Ovodov, 2021](https://ieeexplore.ieee.org/abstract/document/9396534). Semantic-based Annotation Enhancement Algorithm for Semi-supervised Machine Learning Efficiency Improvement Applied to Optical Braille Recognition. **SSL от Ильи Оводова. Очень полезная статья. Весь код на GitHub в ветке develop.**
1. [AlSalman, 2021](https://www.researchgate.net/profile/Suheer-Alhadhrami/publication/350022456_A_Deep_Learning-Based_Recognition_Approach_for_the_Conversion_of_Multilingual_Braille_Images/links/604c0111a6fdcccfee79c592/A-Deep-Learning-Based-Recognition-Approach-for-the-Conversion-of-Multilingual-Braille-Images.pdf). Упоминалось выше.
1. [Alufaisan, 2021](https://books.google.ru/books?hl=ru&lr=&id=Se4lEAAAQBAJ&oi=fnd&pg=PA87&ots=dW2I335C6_&sig=G4zq8Z576SzvJz0kr8uIzTuoLeM&redir_esc=y#v=onepage&q&f=false), Arabic Braille Numeral Recognition Using Convolutional Neural Networks. **? не очень понятно, что они сделали. Перечитать.**
1. [Ortoncelli, 2021](https://arxiv.org/abs/2103.03935). An automated approach to mitigate transcription errors in braille texts for the Portuguese language. **Линии детектируются с помощью преобразования Хоу, только прямые.
Статья, впрочем, написана качественно, явно старались люди.
Ещё, что интересно, они пытаются исправить ошибки в распознавании, подсчитывая расстояние Левенштейна между словом и словами из словаря. Есть датасет!! Но!! Он не собран и размечен, а как-то сгенерирован.
TODO написать авторам, а то ссылки битые**.
1. [Ovodov, 2020](https://arxiv.org/abs/2012.12412). Optical Braille Recognition Using Object Detection CNN. О ней уже выше написано.

## GitHub: поиск [Braille recognition](https://github.com/search?q=braille+recognition)

В основном геометрическое распознавание одностороннего брайля (или вообще сгенерированных картинок).
Однако поиск не выдал DSBI вообще, AngelinaDataset и AngelinaReader - только на вкладке "topics", наши работы только на вкладке  "wiki", поэтому может быть ещё что-то, что я не нашёл. 

# Выводы

Самое интересное, что найдено - Ortoncelli, 2021.
Ovodov, Li ещё интереснее (но уже было известно до этого).