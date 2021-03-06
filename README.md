# ml-experiments

My experiments with machine learning

## Dependencies

```sh
sudo apt-get install \
    build-essential \
    python3-dev \
    libopenblas-dev \
    libgraphviz-dev \
    pkg-config
```

## Virtualenv

```sh
mkvirtualenv ml-experiments -p /usr/bin/python3
pip install -U pip setuptools
pip install -r requirements.txt
```

## Kaggle CLI

```sh
kg config -g -u username -p password
```

## `~/.keras/keras.json`

```json
{
    "image_data_format": "channels_first",
    "epsilon": 1e-07,
    "floatx": "float32",
    "backend": "theano"
}
```

## `~/theanorc`

```ini
[global]
device = cpu
floatX = float32

[blas]
ldflags = -L/usr/local/lib -lopenblas
```
