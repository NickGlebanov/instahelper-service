# Пререквизиты:
1. Должен быть установлен Python 3 версии
2. Далее установите pip `sudo apt install python3-pip`
3. Установите библиотеку для работы плагина ansible `sudo pip install user boto3`
4. Должна быть развернута инфраструктура из проекта https://github.com/NickGlebanov/instahelper-infra

# Запуск ansible скриптов
1. Перед запуском проверьте запущены ли сервера `ansible-inventory --graph -i aws_ec2.yml`
2. Если сервера запущены, то выполните одну из следующих команд:

### Простой запуск (без использования Docker и Systemd)
`ansible-playbook service_without_docker_playbook.yml`

### Запуск с использованием Docker (без использования Systemd)
`ansible-playbook service_with_docker_playbook.yml`

### Запуск с использованием Docker и Systemd
`ansible-playbook unit_service_with_docker_playbook.yml`