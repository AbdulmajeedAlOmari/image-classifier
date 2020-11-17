# Intro to Machine Learning - TensorFlow Project

In this project, I will classify flower types given their images by using neural networks and transfer learning techniques.

### Content
- `Project_Image_Classifier_Project.ipynb`: Jupyter notebook showing all the steps I made to create a classifier model
- `Project_Image_Classifier_Project.html`: HTML version of the jupyter notebook
- `models/1605550143.h5`: Classifier model
- `predict.py`: Python application that uses our classifier model to predict flower type

### Requirements
- Install the following modules in order to run `predict.py` application:
    - argparse
    - tensorflow
    - tensorflow_hub
    - numpy
    - PIL

### Usage
```
> predict.py --input [image_path] --model [model_path] --top_k [number_of_classes] --category_names [json_file_of_class_names]
```

Sample uses for `predict.py` application:
```
> predict.py --top_k 7
> predict.py --input './test_images/my_flower.jpg'
> predict.py --model './models/my_model.h5'
```

Note that the arguments have default values, te default values are:
- `--input`: ./test_images/orange_dahlia.jpg
- `--model`: ./models/1605550143.h5
- `--top_k`: 5
- `--category_names`: ./label_map.json