Обновляем наш `pip`
```shell
pip install --upgrade pip
```
Установим `jupyter notebook` в нашей виртуальной среде!
```shell
pipenv install jupyter
```
И установим `ipykernel` который нам поможет запускать `jupyter notebook` внутри виртуальной среды
```shell
pipenv install ipykernel
```
Используем возможность установить нашу виртуальную среду
```shell
python -m ipykernel install --user --name=my-virtualenv-name
```
Так-же установим все нужные нам библиотеки:
```shell
pipenv install matplotlib numpy tensorflow tensorflow_hub
```
И у нас здесь конфликт зависимостей который можно исправить двумя командами:
```shell
pipenv lock --pre
pipenv sync
```
Если работаем с клонированой репозиторией пользуемся командой `pipenv install --deploy`

Далее запустим нашу среду и тетрадь.
```shell
pipenv shell
jupyter notebook
```
Дальше мы будем следовать `TF Hub` https://colab.research.google.com/github/tensorflow/hub/blob/master/examples/colab/tf2_arbitrary_image_stylization.ipynb#scrollTo=v-KXRY5XBu2u

Откройте `Style Transfer.ipynb`
