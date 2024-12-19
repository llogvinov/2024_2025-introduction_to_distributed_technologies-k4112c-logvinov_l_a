University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2024/2025
Group: K4112c
Author: Logvinov Lev Anatolievich
Lab: Lab1
Date of create: 20.09.2024
Date of finished: 31.09.2024


Вопросы:
1. Что сейчас произошло и что сделали команды указанные ранее?
Команды указанные ранее помогли развернуть Minikube Cluster и 
Pod, который запускает контейнер с образом HashiCorp Vault, который слушает на порту 8200. 
Далее был создан сервис типа NodePort, маршрутизирующий сетевые запросы, поступающие на порт 8200, в Pod на порт 8200. 
Настроено перенаправление сетевого трафика с порта 8200 локального компьютера в сервис на порт 8200

2. Где взять токен для входа в Vault?
В логах пода. Для этого нужно выполнить команду minikube kubectl logs vault.