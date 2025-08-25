# ansible-examples

Этот проект содержит примеры использования [Ansible](https://www.ansible.com/).

## О проекте

- [**ansible-playbook**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook) - `playbook` для взаимодействия с `Ansible`;
- [**ansible-playbook-vars**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-vars) - - `playbook` для взаимодействия с `Ansible` с применением *переменных*;
- [**ansible-playbook-inventory**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-inventory) - `playbook` для взаимодействия с `Ansible` с применением конфигурационнх файлов для хостов `inventory.ini`;
- [**ansible-playbook-cfg**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-cfg) - `playbook` для взаимодействия с `Ansible` с применением глобальных конфигурации `ansible.cfg`; 
- [**ansible-playbook-multi**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-multi) - `playbook` для взаимодействия с `Ansible` для демонстрации возможности работы с несколькими хостами и демонстрации `roles`;
- [**ansible-playbook-loop-until**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-multi) - `playbook` для демонстрации возможности использования циклов в `Ansible`;


## Быстрый старт

1. Установите Ansible:
   ```bash
   pip install ansible
   ```
2. Склонируйте репозиторий:
   ```bash
   git clone https://github.com/pcade/ansible-examples.git
   ```
3. Изучайте и запускайте примеры playbook'ов из каталога.

## Основные команды

- **ansible -m setup localhost** — собрать всю доступную информацию о вашей хостовой машине;
- **ansible-playbook `наименование playbook`** — запуск `playbook` при условии что `hosts` описан в самом `playbook`;
- **ansible-playbook `наименование playbook` -vv** — запуск `playbook` подробным выводом, максимальное `vvvvv` ;
- **ansible-playbook -i `наименование файла inventory` `наименование playbook`** — запуск `playbook` при условии что `hosts` описан в самом `inventory`;
- **ansible -i `наименование файла inventory` all -m ping** — проверить доступных `hosts` из `inventory`;
- `inventories/` — инвентарные файлы

## Контакты

Для вопросов и предложений — открывайте Issues или пишите в Discussions.

---
