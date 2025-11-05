# Домашнее задание к занятию "`«Система мониторинга Zabbix. Часть 2» `" - `Ефимов Вячеслав`


### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw).
   2. Выполните клонирование данного репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите вверху название занятия и вашу фамилию и имя
      - в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
      - для корректного добавления скриншотов воспользуйтесь [инструкцией "Как вставить скриншот в шаблон с решением](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md)
      - при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md))
   4. После завершения работы над домашним заданием сделайте коммит (`git commit -m "comment"`) и отправьте его на Github (`git push origin`);
   5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
   6. Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.
   
Желаем успехов в выполнении домашнего задания!
   
### Дополнительные материалы, которые могут быть полезны для выполнения задания

1. [Руководство по оформлению Markdown файлов](https://gist.github.com/Jekins/2bf2d0638163f1294637#Code)

---

### Задание 1

1. ![Задание1](https://github.com/IthnHuitn/Zabbix-HW2/blob/main/zabbix2-1-1.png)

---

### Задание 2 - ### Задание 3

1. ![Задание2-3](https://github.com/IthnHuitn/Zabbix-HW2/blob/main/zabbix2-2-3.png)

### Задание 4

1. ![Задание4](https://github.com/IthnHuitn/Zabbix-HW2/blob/main/zabbix2-4.png)


### Задание 5

1. ![Задание5](https://github.com/IthnHuitn/Zabbix-HW2/blob/main/zabbix2-5.png)


### Задание 6

1. ![Задание6](https://github.com/IthnHuitn/Zabbix-HW2/blob/main/zabbix2-6.png)

### Код скрипта 

.... !/bin/bash
.... # Скрипт для UserParameter Zabbix
.... # Возвращает ФИО или дату в зависимости от аргумента
.... 
.... # Проверяем, что передан ровно один аргумент
.... if [ $# -ne 1 ]; then
....     echo "Ошибка: Скрипт требует ровно один аргумент (1 или 2)."
....     exit 1
.... fi
.... 
.... case "$1" in
....     "1")
....         # Возвращаем ваши ФИО
....         echo "Ефимов Вячеслав Романович"
....         ;;
....     "2")
....         # Возвращаем текущую дату в формате ГГГГ-ММ-ДД
....         date +"%Y-%m-%d"
....         ;;
....     *)
....         # Обработка неверного аргумента
....         echo "Ошибка: Неверный аргумент. Используйте 1 (для ФИО) или 2 (для даты)."
....         exit 1
....         ;;
.... esac

### Задание 7

1. ![Задание7](https://github.com/IthnHuitn/Zabbix-HW2/blob/main/zabbix2-7.png)
# 
2.  https://drive.google.com/file/d/1kJMu30t5NQKD9CnVdfi6ZftkEF0SR5jw/view?usp=drive_link

### Задание 8

# Vagrantfile
1. https://drive.google.com/file/d/1IgeOmxhuTB13XiDaaU3A5XgoRAVJB6gZ/view?usp=drive_link

# Zabbix-agent.sh

2. https://drive.google.com/file/d/16TpizZkb7leIAVLPQPAXKi-r00tpGUbp/view?usp=drive_link