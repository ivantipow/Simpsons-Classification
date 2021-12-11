# Simpsons Classification

В <a href="https://github.com/ivantipow/Simpsons-Classification/blob/main/simpsons-classification.ipynb">данном ноутбуке</a> рассматривается решение задачи классификации изображений в рамках учебного Kaggle-соревнования [Journey to Springfield](https://www.kaggle.com/c/journey-springfield) от [Deep Learning School](https://www.dlschool.org/). Для решения используется техника Transfer Learning/Fine tuning над нейронными сетями [`Efficientnet_B4`](https://arxiv.org/pdf/1905.11946.pdf) и `ResNet 18`, предобученными на ImageNet. В этом блокноте приведён основной training loop, выполняется аугментация изображений, в качестве оптимизатора используется [AdamW](https://pytorch.org/docs/stable/generated/torch.optim.AdamW.html). Для работы с learning rate используется scheduler [`StepLR`](https://pytorch.org/docs/stable/generated/torch.optim.lr_scheduler.StepLR.html). Для борьбы с дисбалансом классов используется oversampling.

Результат на Kaggle: 0.99362 `F1-Score`.
