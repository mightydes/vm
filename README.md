# vm

## Использование

### Запуск всего playbook

```bash
ansible-playbook playbook.yml
```

### Запуск конкретной роли

```bash
ansible-playbook playbook.yml --tags fish
```

### Проверка без изменений (dry-run)

```bash
ansible-playbook playbook.yml --check
```

### Запуск с повышенной детализацией

```bash
ansible-playbook playbook.yml -v
# или
ansible-playbook playbook.yml -vvv  # максимальная детализация
```

## Переменные

Переменные можно определить в:

- `inventory/hosts.yml` - для конкретных хостов
- `group_vars/` - для групп хостов
- `host_vars/` - для отдельных хостов
- `roles/*/defaults/main.yml` - значения по умолчанию для роли
- `roles/*/vars/main.yml` - переменные роли
