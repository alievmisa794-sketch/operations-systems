# Конспект: конфигурационные файлы GNU/Linux

Источник: слайды 28–34.

| Путь | Назначение |
|---|---|
| `/etc/sysconfig/` | Каталог с файлами конфигурации системы |
| `/etc/hostname` | Имя хоста |
| `/etc/resolv.conf` | Настройки DNS |
| `/etc/hosts` | Псевдонимы (имена) для сетевых узлов |
| `/etc/os-release` | Название и версия дистрибутива, иногда ссылки на официальные ресурсы |
| `/etc/ssh/` | Конфигурация сервера SSH |
| `$HOME/.ssh/config` | Конфигурация SSH для конкретного пользователя |
| `/etc/passwd` | Список пользователей |
| `/etc/group` | Группы пользователей |
| `/etc/shadow` | Хэши паролей пользователей |
| `/etc/sudoers` | Привилегии, относящиеся к команде `sudo` |
| `/etc/environment` | Переменные окружения, загружаемые в оболочку при запуске терминала (например, `PATH`) |
| `/etc/fstab` | Записи для монтирования файловых систем |
| `/etc/default/grub` | Конфигурация, по которой `update-grub` создаёт `/boot/grub/grub.cfg` |
| `/etc/crontab` | Конфигурация планировщика заданий (cron) |

Примеры для проверки в своей ВМ:

```bash
cat /etc/os-release
cat /etc/hostname
cat /etc/resolv.conf
cat /etc/passwd
sudo cat /etc/shadow     # только с правами root
cat /etc/fstab
cat /etc/crontab
```
