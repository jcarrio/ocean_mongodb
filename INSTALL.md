# Instalação do MongoDB no Windows
* criar pasta "c:\mongodb"
* descompactar "mongodb-win32-x86_64-2012plus-4.2.16.zip" em "c:\mongodb"
* criar pasta "c:\mongodb\log"
* criar pasta "c:\data\db"
* criar arquivo "c:\mongodb\mongo.config" com:
```
#store data here
dbpath=C:\data

#all output go here
logpath=C:\mongodb\log\mongo.log

#log read and write operations - erro
#diaglog=3
```
* iniciar mongodb (não pode fechar tela e nem parar):
"mongod --config C:\mongodb\mongo.config"

* instalar mongodb como serviço:
"mongod --config C:\mongodb\mongo.config --install"

* iniciar serviço:
"net start mongodb"

* parar serviço:
"net stop MongoDB"

* remover serviço:
"mongod --remove"
