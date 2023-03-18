Установка и настройка protoc

1. Необходимо пройти на официальную страницу и посмотреть инструкцию
2. Если при настройке выдает ошибку
bash: /c/Users/Windows/bin/protoc: cannot execute binary file: Exec format error

1. Скачать необходимый релиз под свою ОС
```
https://github.com/protocolbuffers/protobuf/releases/
```
2. Настроить путь до исполняемого файла
```
Win + R
```
```
sysdm.cpl
```

protoc --go_out=. --go_opt=paths=source_relative \
    --go-grpc_out=. --go-grpc_opt=paths=source_relative \
    user.proto