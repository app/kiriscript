### Read this file as UTF-8 Russian text  
: ' 
<!--
'
# Run this file in bash to view its content formatted
#
pandoc -s -f markdown -t man $0 | man -l - ; exit
: '
-->
'

# Общая информация  
Код разрабатывается и отлаживается под Linux (Ubuntu 16.04 LTS)  

# С чего начать
Забираем код из git репозитория и устанвливаем зависимости указанной ниже командой

# Зависимости  
В системе должен быть установлен менеджер пакетов npm (node.js package manager)  
Иногда он устанавливается вместе с node.js  
Для установки требуемых для сборки kiri библиотек выполняем команду  
```npm install ```

# Запуск тестов  
make test  

# Сборка kiri из исходников
make

# Запуск kiri
``` 
./bin/kiri --help
```

# Запуск coffeelint
npm run lint
