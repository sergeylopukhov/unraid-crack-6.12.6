Уставнока UNRAID 6.12.6

Установить на флешку unraid с помощью unraid usb creator

Во время установки перписать GUID флешки

Файл go на флешке в папке /config - отредактировать и привести к виду:
```
#!/bin/bash
export UNRAID_GUID=GUID вашей флешки
export UNRAID_NAME=Имя вашего сервера на английском языке
export UNRAID_DATE=1654646400
export UNRAID_VERSION=Pro
/lib64/ld-linux-x86-64.so.2 /boot/config/unraider
#Start the Management Utility
/usr/local/sbin/emhttp &
```
Файлы из папки crack - hook.so, trial.key, unrader переместить в папку /config на флешке

Наслаждаться
