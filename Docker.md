## Docker контейнер
### Порядок установки
1. Установите Docker
2. Получите образ контейнера с помощью команды:
```shell script
docker pull qwertyadrian/tg_autoposter
```
3. Запустите docker контейнер командой (при необходимости укажите параметры запуска бота)
```shell script
docker run -it --name tgautoposter -v <путь к каталогу с файлом конфигурации и списком стоп-слов>:/data tg_autoposter [параметры запуска бота]
```
6. При остановке работы контейнера можно возобновить работу командой (параметр `-ai` необходим только для интерактивного режима, для запуска в фоне можно не указывать):
```shell script
docker start -ai tgautoposter
```