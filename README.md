# DeepBach_Redo

This is a reproduction project of DeepBach for ECS7007P by Corey Ford, Eleanor Row, and me. The original repository is the keras branch of the [DeepBach](https://github.com/Ghadjeres/DeepBach/tree/original_keras) by [Ghadjeres](https://github.com/Ghadjeres/DeepBach/commits?author=Ghadjeres).

The DeepBach paper was limited in its evaluation, only using three categories to distinguish between participants expertise.

We aimed to extend this, exploring more deeply:

- The relationship between musical expertise and people's ability to guess the ML models.
- Analyse the musical qualities of the model outputs, discovering their weaknesses.

Compared with the original keras version only has DeepBach model, we implement Maximum Entropy and Multilayer Perceptron models (see `model_zoo.py` and `model_manager.py`) following the stuctures described by [Sam Goree](https://samgoree.github.io/2017/01/29/DeepBach.html). We retrain the models using the preprocessed data by Ghadjeres and reharmonize four pieces of Bach chorales. The generated samples are contained in `Generation/`.

We also fixed some issues of the original project:

- the pre-trained models provided by the original project cannot be loaded (see [here](https://github.com/Ghadjeres/DeepBach/issues/47)), so you have to retrain all models by yourself. If you want to access the preprocesse dataset and our re-trained model, please email me at jingjing.tang@qmul.ac.uk
- the argument problem has also been fixed (see [here](https://github.com/Ghadjeres/DeepBach/issues/43))

We choose this keras version because it is well developed for taking MIDI files as input while the new pytorch version does not support.

If you are interested in our analysis results, please look at the slides.