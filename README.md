# bash_scripts
Небольшая коллекция скриптов на `bash` для повседневного использования

# Установка
1. Склонировать этот репозиторий и положить скрипты в желаемую папку
2. Дать скрипту право на выполнение:
   `chmod +x <script_file_name>`
3. Опционально, экспортировать папку со скриптом в `PATH`. 
   Например: `export PATH="$PATH:/home/trofchik/Documents/scripts/"`
   
# Использование 
Если был выполнен шаг 3 предыдущего пункта, то скрипт можно запустить из любого места в оболочке просто введя его имя и аргументы (если нужно).
Альтернативно, перейти в папку со скриптом и запустить его как обычный бинарник. 
Например: `./script_file_name`

# Описание скриптов
`saferemove` -- безопасное извлечение USB устройства. Анмаунтит устройство, а затем отключает ему питание. Принимает "системное" название устройства в качестве аргумента. 
Например: `saferemove sdb1`

`netrestart` -- в некоторых корпоративных сетях при обрыве вайфай соединения требуется перезапуск сервиса `NetworkManager`. Содержит команду `sudo`. 
