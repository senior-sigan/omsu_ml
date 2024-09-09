# Настройка окружения

В курсе мы используем Python и Jupyter, как IDE.

- Рекомендуем всё делать в [Google Colab](https://colab.research.google.com/) — это бесплатный облачный jupyter. Даже GPU есть для обучения нейросетей.
- Можно делать на своем компе. Мы рекомендуем Linux.

## Использование Google Colab

TODO: 5-минутный видос, как пользоваться.

## Установка Python на Linux или MacOS

В дистрибутивах linux и в MacOS можно установить Python сразу из репозиториев, но я предлагаю пойти более правильным путём и установить [менеджер версий python](https://github.com/pyenv/pyenv). Это может вам пригодиться в будущем.

### Установка Pyenv Для Ubuntu/Debian/Mint

Если у вас другой дистрибутив, то читайте [официальную доку](https://github.com/pyenv/pyenv/wiki#suggested-build-environment) от pyenv.

Сначала нам необходимо поствавить пакеты для сборки python.

Запустите терминал, скопируйте команду снизу, вставьте в консоль, нажмите enter, введите пароль пользователя. Ждите конца установки.

```sh
sudo apt-get update; sudo apt-get install git make build-essential libssl-dev zlib1g-dev \
libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm \
libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
```

Выполните команду:

```sh
curl https://pyenv.run | bash
```

Перезапустите shell, то есть закройте терминал и откройте снова.

### Установка Python через Pyenv

Выполните команду:

```sh
pyenv install 3.12.4
```

Сделайте этот python дефолтным:

```sh
pyenv global 3.12.4
```

Можете презапустить темринал. Проверьте что вверсия питона правильная

```sh
python --version
```

### Установка pip пакетов

```sh
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

### Запуск Jupyter IDE

Создайте папку, где будете хранить весь код и данные. Откройте терминал в этой папке и запустите juputer командой

```sh
jupyter-notebook
```

Вы увидите в терминале что-то такое:

![](jupyter-start.png)

Обычно после этого открывается браузер по умолчанию по адресу http://localhost:8888 + какой-то токен. Вы можете в терминале через ctrl-click открыть jypyter.

## Установка Python на Windows WSL2 (Рекомендуем!)

TODO: настройка wsl2

Далее идентично установке на Linux.

## Установка Python на Windows (Conda)

TODO