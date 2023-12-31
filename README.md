# Segmentation
Segmentation CNNs(SegNet, UNet, UNet2) for DLS
В этом задании вам предстоит решить задачу сегментации медицинских снимков.

## Общий вывод
В ходе данной работы были проанализированы 3 архитектуры: SegNet, Unet и Unet2, а также слдеюущие лоссы: BCE, Dice, Focal и Lovasz. 

1. **Самая стабильная архитектура - UNet**
2. **Оптимальный лосс - lovasz**
Модель, лучше всего показавшая себя на тестовом датасете:

**UNet2 + lovasz** 

Исследование проводилось в следующих услвоиях: Количество эпох - 50 для всех моделей, Оптимизатор AdamW без дополнительной настройки.

Как можно было бы улучшить результат:
1. Попробовать аугментировать данные(по сути это фотографии, а у всех фотографий могут быть одинаковые проблемы)
2. Настроить Sheduler для борьбы с переобучением.
3. Существует еще много Loss функций, можно попробовать еще что-то.

Данный ноутбук можно прогнать примерно за час на Kaggle, все нейросети обучаются быстро, память очищается в цикле обучения.
