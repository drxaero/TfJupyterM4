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