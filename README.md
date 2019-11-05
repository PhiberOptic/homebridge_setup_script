# Homebridge setup script

Итак, что же делает этот скрипт?

* Добавляет репозиторий nodejs 12.x
* Ставит `nodejs` и `libavahi-compat-libdnssd-dev`
* Через npm ставит `homebridge`
* Создает папку `.homebridge` в домашнем каталоге текущего пользователя
* Кладет туда файл конфигурации с данными для запуска веб-интерфейса
* Ставит сам плагин веб-морды - `homebridge-config-ui-x`
* Создает `homebridge.service` и запускает его
* Создает отдельный `homebridge-config-ui-x.service` и запускает его

Теперь даже при перезагрузке homebridge с кривым конфигом, Вы сможете восстановить его работоспособность используя веб-интерфейс.

Чтобы установить выполняем в терминале следуюшие команды:
* `sudo apt install git`
* `git clone https://github.com/exdee85/homebridge_setup_script`
* `cd homebridge_setup_script`
* `bash install.sh`

Процесс установки займет минут 10, в итоге Вы получите работоспособный homebridge и его веб-морду на порту `8080`.

Login: `admin`

Password: `admin`
