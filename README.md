# awesome-imgcook

[imgcook](https://github.com/imgcook) is an ingenious chef who specializes in cooking with something for the Web intelligence.

## Contents

- [JavaScript packages for machine learning](#javaScript-packages-for-machine-learning)
  - [Neural networks](#neural-networks)
  - [Feature engineering](#feature-engineering)
  - [Natural language processing](#natural-language-processing)
  - [Tools](#tools)
- [Pipcook Pipelines](#pipcook-pipelines)
- [Pipcook Plugins](#pipcook-plugins)
  - [Data Collect](#data-collectdataset)
  - Data Access
  - Data Process
  - [Model Define](#model-define)
  - [Model Train](#model-train)
  - Model Evaluate
- [Resources](#resources)
  - [Tutorials](#tutorials)
  - [Notebooks](#notebooks)
  - [Books](#books)

## JavaScript packages for machine learning

### Neural networks

- [tensorflow/tfjs](https://github.com/tensorflow/tfjs) - A WebGL accelerated JavaScript library for training and deploying ML models.
- [yorkie/tensorflow-nodejs](https://github.com/yorkie/tensorflow-nodejs) - TensorFlow Node.js provides idiomatic JavaScript language bindings and a high layer API for Node.js users.
- [BrainJS/brain.js](https://github.com/BrainJS/brain.js) - Machine-learning framework.
- [microsoft/onnxjs](https://github.com/microsoft/onnxjs) - ONNX.js: run ONNX models using JavaScript.

### Feature engineering

- [imgcook/datacook](https://github.com/imgcook/datacook) - Data processing in pure JavaScript.
- [opensource9ja/danfojs](https://github.com/opensource9ja/danfojs) - danfo.js is an open source, JavaScript library providing high performance, intuitive, and easy to use data structures for manipulating and processing structured data.
- [oliver-moran/jimp](https://github.com/oliver-moran/jimp) - An image processing library written entirely in JavaScript for Node, with zero external or native dependencies.

### Natural language processing

- [wooorm/retext](https://github.com/wooorm/retext) - An extensible natural language system.
- [wooorm/franc](https://github.com/wooorm/franc) - Detect the language of text.
- [sindresorhus/leven](https://github.com/sindresorhus/leven) - Measure the difference between two strings using the Levenshtein distance algorithm.
- [NaturalNode/natural](https://github.com/NaturalNode/natural) - Natural language facility.
- [axa-group/nlp.js](https://github.com/axa-group/nlp.js) - Building bots, with entity extraction, sentiment analysis, automatic language identify, and more.

### Tools

- [opensource9ja/dnotebook](https://github.com/opensource9ja/dnotebook) - Dnotebook is a Jupyter-like library for javaScript environment. It allows you to create and share pages that contain live code, text and visualizations.
- [alibaba/pipcook](https://github.com/alibaba/pipcook) - Front-End Algorithm Engineering Platform.

## Pipcook Pipelines

This section will list some useful pipelines that you could train locally and use:

```sh
$ pipcook run https://uri/to/pipeline
```

- Image classification
  - [databinding-image-classification-mobilenet.json](https://raw.githubusercontent.com/alibaba/pipcook/main/example/pipelines/databinding-image-classification-mobilenet.json) a pipeline to classify image in mobilenet.
  - [databinding-image-classification-resnet.json](https://raw.githubusercontent.com/alibaba/pipcook/main/example/pipelines/databinding-image-classification-resnet.json) a pipeline to classify image in resnet.
- Object Detection
  - [object-detection-yolov5.json](https://github.com/alibaba/pipcook/blob/main/example/pipelines/object-detection-yolov5.json)(Recommanded) object detection pipeline in lightweight yolov5 model.
  - [object-detection-fasterrcnn.json](https://raw.githubusercontent.com/alibaba/pipcook/main/example/pipelines/object-detection-fasterrcnn.json) object detection pipeline in Faster-RCNN model.
- Text Classification
  - [text-bayes-classification](https://raw.githubusercontent.com/alibaba/pipcook/main/example/pipelines/text-bayes-classification.json) a bayesian-based model to classify texts.
- Text Creation
  - [chinese-poem-creation.json](https://raw.githubusercontent.com/alibaba/pipcook/main/example/pipelines/chinese-poem-creation.json) creating Chinese poems by yourself.

## Pipcook Plugins

The following lists Pipcook plugins in category.

### Data Collect(Dataset)

- [imgcook/pipcook-plugin-mnist-data-collector](https://github.com/imgcook/pipcook-plugin-mnist-data-collector) Mnist dataset Collector.
- [imgcook/pipcook-plugin-csv-data-collector](https://github.com/imgcook/pipcook-plugin-csv-data-collector) CSV dataset collector.
- [imgcook/pipcook-plugin-fasttext-data-collector](https://github.com/imgcook/pipcook-plugin-fasttext-data-collector) FastText-compatible dataset collector.
- [imgcook/pipcook-plugin-ui-generator](https://github.com/imgcook/pipcook-plugin-ui-generator) Generate UI samples for object detection and image classification pipelines.

### Model Define

- [imgcook/pipcook-plugin-fasttext-model](https://github.com/imgcook/pipcook-plugin-fasttext-model) Pipcook plugin for fasttext model definition.
- [imgcook/pipcook-plugin-detectron-maskrcnn-model](https://github.com/imgcook/pipcook-plugin-detectron-maskrcnn-model) Pipcook plugin for detectron maskrcnn model definition.

### Model Train

- [imgcook/pipcook-plugin-tensorflow-bert-ner-model-train](https://github.com/imgcook/pipcook-plugin-tensorflow-bert-ner-model-train) train a tensorflow-based NER model.
- [imgcook/pipcook-plugin-detectron-model-train](https://github.com/imgcook/pipcook-plugin-detectron-model-train) train a detectron2-based vision model.
- [imgcook/pipcook-plugin-tensorflow-image-classification-model-train](https://github.com/imgcook/pipcook-plugin-tensorflow-image-classification-model-train) train a tensorflow-based image classfication model.
- [imgcook/pipcook-plugin-tfjs-image-classification-model-train](https://github.com/imgcook/pipcook-plugin-tfjs-image-classification-model-train) train a tfjs-based image classification model.

## Resources

### Tutorials

- [体验机器学习：在Mac电脑上训练和部署一个图片分类模型](https://github.com/imgcook/ml-mac-classify)
- [Boa: Use Python functions in Node.js](https://www.reddit.com/r/Pipcook/comments/ime8ij/boa_use_python_functions_in_nodejs/)
- [How to use free GPU/TPU with Pipcook on Google Colab](https://www.reddit.com/r/Pipcook/comments/im4vrp/how_to_use_free_gputpu_with_pipcook_on_google/)

### Notebooks

The notebooks is based on Google Colab, you can enable its free GPU/TPU to save your time:

- [Pipcook tutorial: image classification in frontend](https://colab.research.google.com/github/alibaba/pipcook/blob/master/notebooks/pipcook_image_classification.ipynb)
- [Pipcook tutorial: object detection in frontend](https://colab.research.google.com/github/alibaba/pipcook/blob/master/notebooks/pipcook_object_detection.ipynb)

### Documentations

- [Pipcook docs](https://alibaba.github.io/pipcook/#/)
- [imgcook docs](https://www.imgcook.com/docs)

## License

MIT.
