# Internship task on Successor Representation

В данном задании предлагается разобраться с темой Successor Representations (SR) в Reinforcement Learning (RL) на примере среды AnimalAI, с которой мы сейчас работаем.

План задания:

1. Установить и разобраться со средой [AnimalAI](https://github.com/Kinds-of-Intelligence-CFI/animal-ai). [Здесь](http://animalai.org/AAI/testbed) можно посмотреть предзаданные конфигурации среды, нас интересуют задачи из секции Introductory experiments, например, "Basic Food Variations".
2. Реализовать простой model-free RL бейзлайн, например, DQN или любой метод из актор-критиков и добиться его успешной работы. Заготовку реализации можно взять из открытых источников, например, из библиотеки [ClearnRL](https://github.com/vwxyzjn/cleanrl).
3. Реализовать модификацию бейзлайна, которая бы работала в парадигме Successor Representation, и добиться ее успешной работы.
4. Сравнить скорость и качество обучения полученного алгоритма с бейзлайном. Исследовать выученные Successor Representations (например, с помощью t-SNE).
5. _Bonus task_: Добавить модификации бейзлайна и SR-варианта, которые бы дополнительно выучивали модель среды (для этого можно использовать LSTM или Sequential VAE). Добиться качественного обучения модели и добавить обучение в воображении (т.е. обучение по траекториям, полученным не в среде, а с использованием обученной модели среды, см. идею метода [Dreamer](https://arxiv.org/abs/1912.01603)). Сравнить результаты полученных model-based вариаций с предыдущими двумя model-free вариантами.

Результатом работы должна быть ссылка на ваш репозиторий с выполненным заданием и логи из [wandb](https://wandb.ai/) проекта.

Полезные ссылки по Successor Representation:

- Простое введение
  - [The present in terms of the future: Successor representations in Reinforcement learning](https://awjuliani.medium.com/the-present-in-terms-of-the-future-successor-representations-in-reinforcement-learning-316b78c5fa3)
  - [The Successor Representation, γ-Models, and Infinite-Horizon Prediction](https://bair.berkeley.edu/blog/2021/01/05/successor/)
- Примеры реализации
  - [Tabular case](https://github.com/awjuliani/successor_examples)
  - [NN case](https://github.com/bonniesjli/DQN_SR)
- Статьи
  - [Deep Successor Reinforcement Learning (2016)](https://arxiv.org/pdf/1606.02396.pdf)
  - [Successor Features for Transfer in Reinforcement Learning (2017)](https://proceedings.neurips.cc/paper/2017/file/350db081a661525235354dd3e19b8c05-Paper.pdf)
  - [Universal successor representations for transfer reinforcement learning (2018)](https://arxiv.org/pdf/1804.03758.pdf)
