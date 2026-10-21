# PyTorch Learning

Notebooks written while learning PyTorch with the
[Zero to Mastery PyTorch course](https://www.learnpytorch.io/) by Daniel Bourke. Both projects
classify food images (pizza, steak, sushi) and build on each other: from a model written from
scratch to transfer learning and tracked experiments.

[Русская версия](README.ru.md)

## Projects

| Project | What it covers |
|---|---|
| [01-food-vision](01-food-vision) | Loading an image dataset with `ImageFolder` and with a custom `Dataset` class, a TinyVGG model written from scratch, training and evaluation loops, saving weights, then transfer learning with a pretrained EfficientNet-B0 and predictions on new images |
| [02-experiment-tracking](02-experiment-tracking) | Experiment tracking with TensorBoard: EfficientNet-B0 and EfficientNet-B2 feature extractors trained on 10% and 20% of the data for 5, 10 and 20 epochs. The best run, EfficientNet-B0 on 20% of the data for 20 epochs, reached 0.949 test accuracy |

## Running the notebooks

```bash
pip install -r requirements.txt
```

The notebooks download the pizza, steak and sushi dataset from the course repository into
`data/` on the first run. Model weights are saved to `models/` and TensorBoard logs to `runs/`.
None of these folders are tracked by git.

`helper_functions.py` comes from the course materials.

## License

[MIT](LICENSE)
