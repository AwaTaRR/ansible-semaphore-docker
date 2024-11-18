Практикум по Ansible

Требования для выполнения playbook:
 - Установлен Ansible
 - В host.ini добавлен адрес сервера на OS Ubuntu
 - Файл данных с паролями roles/semaphore/vars/secrets.yml зашифрован Ansible-Vault

Выполнение разбито на 3 роли:
  1) Docker - Установка Docker Compose
  2) Semaphore - Копирование и запуск Docker-Compose.yml, в сотавке которого Postgresql + Semaphore
  3) Check - Проверка доступности запущенного сервиса Semaphore

Запуск Playbook:
- ansible-playbook -i hosts.ini site.yml --ask-vault-pass
  
Пароль:
- sempahore


    
