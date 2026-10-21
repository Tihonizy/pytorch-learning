# PyTorch Learning

Ноутбуки, написанные во время изучения PyTorch по
[курсу Zero to Mastery](https://www.learnpytorch.io/) Дэниела Бурка. Оба проекта
классифицируют фотографии еды (пицца, стейк, суши) и продолжают друг друга: от модели,
написанной с нуля, до transfer learning и отслеживания экспериментов.

[English version](README.md)

## Проекты

| Проект | Что в нём |
|---|---|
| [01-food-vision](01-food-vision) | Загрузка изображений через `ImageFolder` и через свой класс `Dataset`, модель TinyVGG с нуля, циклы обучения и оценки, сохранение весов, затем transfer learning на предобученном EfficientNet-B0 и предсказания на новых картинках |
| [02-experiment-tracking](02-experiment-tracking) | Отслеживание экспериментов в TensorBoard: EfficientNet-B0 и EfficientNet-B2 как feature extractor на 10% и 20% данных, 5, 10 и 20 эпох. Лучший запуск, EfficientNet-B0 на 20% данных за 20 эпох, дал 0.949 accuracy на тесте |

## Запуск

```bash
pip install -r requirements.txt
```

При первом запуске ноутбуки сами скачивают датасет pizza, steak, sushi из репозитория курса
в папку `data/`. Веса сохраняются в `models/`, логи TensorBoard в `runs/`. Эти папки в git не попадают.

`helper_functions.py` взят из материалов курса.

## Лицензия

[MIT](LICENSE)
