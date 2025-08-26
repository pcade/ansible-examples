# ansible-examples

Этот проект содержит примеры использования [Ansible](https://www.ansible.com/).

## О проекте

- [**ansible-playbook**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook) - `playbook` для взаимодействия с `Ansible`;
- [**ansible-playbook-vars**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-vars) - - `playbook` для взаимодействия с `Ansible` с применением *переменных*;
- [**ansible-playbook-inventory**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-inventory) - `playbook` для взаимодействия с `Ansible` с применением конфигурационнх файлов для хостов `inventory.ini`;
- [**ansible-playbook-cfg**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-cfg) - `playbook` для взаимодействия с `Ansible` с применением глобальных конфигурации `ansible.cfg`; 
- [**ansible-playbook-multi**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-multi) - `playbook` для взаимодействия с `Ansible` для демонстрации возможности работы с несколькими хостами и демонстрации `roles`;
- [**ansible-playbook-loop-until**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-loop-until) - `playbook` для демонстрации возможности использования циклов в `Ansible`;
- [**ansible-playbook-dictionary**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-dictionary) - `playbook` для демонстрации возможности использования словарей и циклов в `Ansible`;
- [**ansible-playbook-include-import**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-include-import) - `playbook` для демонстрации раличий между модулями `import` и `include` применяемых в `Ansible`;
- [**ansible-playbook-vaults**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-vaults) - `playbook` для взаимодействия с секретами в `Ansible`;
- [**ansible-playbook-tags**](https://github.com/pcade/ansible-examples/tree/main/ansible-playbook-tags) - `playbook` для проверки работы `tags` в `Ansible`;

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
>> Vaults
- **ansible-vault create `наименование vaults`** - Создать и начать редактировать новый зашифрованный `vaults`;
- **ansible-vault edit `наименование vaults`** - Отредактировать существующий зашифрованный `vaults`;
- **ansible-vault encrypt `наименование vaults`** - Зашифровать существующий текстовый `vaults`;
- **ansible-vault view `наименование vaults`** - Просмотреть содержимое зашифрованного `vaults`;
- **ansible-playbook playbook.yml --ask-vault-pass** - Запустить плейбук с запросом пароля;
>> Tags
- **ansible-playbook demo-tags.yml --tags `update,docker`** - запустить `playbook` с определенными `tags`;
- **ansible-playbook demo-tags.yml --skip-tags `update,docker`** - запустить `playbook` без определенными `tags`;

## Контакты

Для вопросов и предложений — открывайте Issues или пишите в Discussions.

---
