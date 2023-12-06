# Запуск машин с Ubuntu

Запуск пустых машин с Ubuntu 22.04.

По умолчанию запускаются две машины.

```
vagrant up

cd provision

ansible-playbook playbooks/environment.yml


```

Обновляются пакеты, устанавливается mysql-server-8.0, mc, nano.
