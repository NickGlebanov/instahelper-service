#Пререквизиты:
1. Должен быть установлен Python 3 версии
2. Далее установите pip `sudo apt install python3-pip`
3. Установите библиотеку для работы плагина ansible `sudo pip install user boto3`

#Запуск ansible скриптов
1. Перед запуском проверьте запущены ли сервера `ansible-inventory --graph -i aws_ec2.yml`
2. Если сервера запущены, то выполните команду `ansible-playbook service_playbook.yml`