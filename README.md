# IRIS

Repo to run the [Tensorflow estimators](https://www.tensorflow.org/guide/premade_estimators) for the [Iris dataset](https://en.wikipedia.org/wiki/Iris_flower_data_set)


```
$ python src/premade_estimator.py
...
Test set accuracy: 0.933
```

```
$ python src/custom_estimator.py
...
Test set accuracy: 0.967
```

## Deployment

### a) Docker container using [Enric Moreu's template](https://github.com/enric1994/docker)

1. Clone his repo
2. Update the requirements
3. Build and run the repo
```
$ git clone https://github.com/enric1994/docker.git
$ cd docker
$ nano 
$ ...
$ make build
$ make run
$ ...
$ make down
```

### b) Virtual Environment using Bash

1. Creation of a virtual environments done by executing the command venv
2. Command to activate virtual environment
3. Install dependencies
4. List the libraries installed on your environment
5. Do your work!
6. When you are done, the command to deactivate virtual environment
```
$ python3 -m venv env/
$ source env/bin/activate
(env) $ pip install -r requirements.txt
(env) $ pip freeze
(env) $ jupyter notebook
$ ...
(env) $ deactivate
```

## Resources

* Google Tensorflow's documentation: https://www.tensorflow.org/guide/
* Google Tensorflow's sample code: https://github.com/tensorflow/models/blob/master/samples/core/get_started/
