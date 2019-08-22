# Computational Autonomy for Materials Discovery (CAMD)



CAMD documents and flow diagram for stable material 
discovery is available on [Google Drive](https://drive.google.com/open?id=1wvPy4qOzY_-AD5xar4SeUQ4GlcDrzF77).


## Installation

Note that, since qmpy is currently only python 2.7 compatible, CAMD python 3 
compatibility depends on a custom fork of qmpy [here](https://github.com/JosephMontoya-TRI/qmpy_py3), which is installed using
the `setup.py` procedure.

We recommend using Anaconda python, and creating a
fresh conda environment for the install (e. g. `conda create -n MY_ENV_NAME`).

### Linux

Update packages via apt and set pathing for MySQL dependency:

```angular2
apt-get update
apt install -y default-libmysqlclient-dev gcc
export PATH=$PATH:/usr/local/mysql/bin
```

Install numpy via pip first, since the build depends on this and numpy has some difficulty recognizing
its own install:

```angular2
pip install numpy
```

Then use the included setup.py procedure, from the cloned directory.

```angular2
python setup.py install
```

### Mac OSX

First dependencies via [homebrew](https://brew.sh/). Thanks to the contributors to this 
[stack exchange thread](https://stackoverflow.com/questions/12218229/my-config-h-file-not-found-when-intall-mysql-python-on-osx-10-8).

```angular2
$ brew install mysql
$ brew install postgresql
$ brew install gcc
```

Install numpy via pip first, since the build depends on this and numpy has some difficulty recognizing
its own install:

```angular2
pip install numpy
```

Then use the included setup.py procedure, from the cloned directory.

```angular2
python setup.py develop
```
