# Pip Cheatsheet

1) Upgrade pip

```sh
python -m pip install pip --upgrade
```

2) Install Virtual Environment

```sh
pip install virtualenv
```

3) Activate Environemnt

- On windows with `Powershell terminal` or `Command prompt`

```sh
.\venv\Scripts\activate.bat
```

- On Windows with `Git Bash Terminal`

```sh
source ./venv/Scripts/activate
```

- On `Unix based terminals` (Ubuntu, Mac, ...)

```sh
source ./venv/bin/activate
```


4) Install packages with pip in activated virtualenv

- Install one package with pip

```sh
pip install pyment
```

- Install two packages with pip

```sh
pip install pyment flake8
```

5) Save all new packages that installed in activated virtualenv

```sh
pip freeze > requirements.txt
```

6) To deactivate virtualenv

```sh
deactivate
```