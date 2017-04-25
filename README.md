# Окружение для разработки приложений на Ember

Настройки Vagrant и плэйбук Ansible для развертывания окружения разработчика под Ember.

## Системные требования

 * Ubuntu 16.04 64-bit
 * Vagrant 1.8.6
 * VirtualBox 5.1
 * Ansible 2.3.0
 * Git 2.7.4

## Использование

Для того чтобы примонтировать директорию с исходным кодом проекта на Ember с виртуальной машины на хостовую машину, выполните
```bash
sudo mount -t cifs -o uid=ilya,gid=ilya,password=vagrant,username=vagrant,iocharset=utf8,sec=ntlm //192.168.36.10/www ./www
```

Для того, чтобы настроить обновление директории в проекте, при изменении их на виртуальной машине, по нажатию на клавишу F5 в Sublime Text 3, в меню Preferences выберите Key Bindings и добавьте
```bash
{ "keys": ["f5"], "command": "refresh_folder_list" }
```