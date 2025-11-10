# Поддержка МСВ Сфера ОС в Wazuh

Данный форк добавляет официальную поддержку **МСВ Сфера ОС 9.6** в Wazuh.

## Что сделано

- Добавлена детекция ОС через стандартный механизм парсинга `/etc/os-release`.
- Поддержка включена для:
  - агента (`wazuh-agent`)
  - менеджера (`wazuh-manager`)
  - модуля обновления (`agent_upgrade`)
- Проверено на **ветке `main`**

## Как определяется МСВ Сфера

На основе `/etc/os-release`:
```ini
NAME="MSVSphere"
ID="msvsphere"
VERSION_ID="9.6"
PRETTY_NAME="MSVSphere 9.6 Server Certified"
