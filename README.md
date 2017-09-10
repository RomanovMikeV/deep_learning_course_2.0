# Материалы для/с курса по глубокому обучению

## Программное обеспечение

Для прохождения этого курса нам понадобится: python3 (или python2) с пакетами numpy, scikit-learn, scikit-image, pytorch.
Теоретически, можно писать код в любом текстовом редакторе, а для тестирования и экспериментов можно пользоваться терминалом.
Но для удобства мы будем пользоваться программой jupyter notebook, в которой есть достаточно много удобств. 
Один из самых удобных способов работы с питоном -- при помощи anaconda.

Установка ПО:
1. Ставим anaconda с сайта [Anaconda](https://www.continuum.io/downloads)
   * Можно поставить урезанный дистрибутив [Miniconda](https://conda.io/miniconda.html)

2. установка библиотек: `conda install numpy scikit-learn scikit-image` 

3. установка ноутбука: `conda install notebook`

4. установка pytorch: следуйте инструкциям на сайте http://pytorch.org/

Если у Вас нет CUDA -- не страшно, можно для тренировки пользоваться pytorch на CPU, отличие с gpu будет заключаться только в отсутствии команд .gpu() и .cpu() для перетаскивания массивов из памяти процессора в графкарту и обратно

Поскольку я очень давно не пользуюсь windows, то прилагаю мануал anaconda для windows (на всякий случай) https://conda.io/docs/install/full.html

После установки pytorch обязательно проверьте его работоспособность: запустите код (в jupyter или в терминале)

```python
import torch

x = torch.zeros(10, 10)
print(x)
```

Если все пройдет без ошибок -- все ОК
Если в процессе вылетит ошибка, то, скорее всего, пакет прийдется собирать из исходников

Рекоммендуемая литература:
1) [Теория оптимизации Nocedal Wright "Numerical Optimization"](https://www.google.ru/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&ved=0ahUKEwibs8XJhtXVAhXsHpoKHT9QCV8QFggnMAA&url=http%3A%2F%2Fwww.bioinfo.org.cn%2F~wangchao%2Fmaa%2FNumerical_Optimization.pdf&usg=AFQjCNG41Hw2uH1SCRFQgj3SvF_-uEcCGg)
2) [Лекции Джоффри Хинтона](https://ru.coursera.org/learn/neural-networks)
3) [Задания Андрея Карпаты](http://cs231n.github.io/)
4) [Книга по Глубокому Обучению от гуру](http://www.deeplearningbook.org/)
5) [Описание картинок предложениями](https://arxiv.org/pdf/1412.2306.pdf)
6) [Статья про ResNet](https://arxiv.org/abs/1512.03385)
7) [Статья про VGG](https://arxiv.org/pdf/1409.1556.pdf)

