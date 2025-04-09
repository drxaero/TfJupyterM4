# Tensorflow Jupyter Environment for Mac (Apple M4/M4 Max Silicon)

A Poetry-based project that lets you run Tensorflow and Jupyter *locally* on Apple M4 or M4 Max silicon with ease.

## Setup Instructions

Install [poetry](https://python-poetry.org/docs/#installing-with-the-official-installer).

Install [Poe the Poet](https://poethepoet.natn.io/installation.html):
```bash
poetry self add 'poethepoet[poetry_plugin]'
```

Run the following commands in your shell to set up the environment:

```bash
poetry env use python3.12
poetry install
```


## Run Jupyter lab

Run the following command to launch Jupyter lab
```bash
poetry poe lab
```

## Check if GPU is available
Run the following command in the Jupyter:
```python
import tensorflow as tf

tf.config.list_physical_devices('GPU')
```
If GPU is detected, it show outputs a non-empty list:
```python
[PhysicalDevice(name='/physical_device:GPU:0', device_type='GPU')]
```
