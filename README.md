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
Вы читаете техническую документацию, для понимания которой требуется определенная квалификация.  
kiri разрабатывается и отлаживается под Linux (Ubuntu 16.04 LTS)  

# С чего начать сборку kiri
Забираем код из git репозитория 
```
git clone https://github.com/app/kiriscript.git
```
и устанавливаем зависимости указанной ниже командой  

# Зависимости  
В системе должен быть установлен менеджер пакетов npm (node.js package manager)  
Иногда он устанавливается вместе с node.js  
Для установки требуемых для сборки kiri библиотек выполняем команду  
```
npm install 
```

# Сборка kiri из исходников
```
make
```

# Запуск kiri
``` 
./bin/kiri --help
```

# Запуск coffeelint
```
npm run lint
```
# Запуск тестов  
```
make test  
```

# Права на использование и распространение
Исходный код kiri распространяется на условиях GNU GPL Version 3, полный текст которых находится в файле LICENSE настоящего проекта.
