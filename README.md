# boot-system
Задание:
- Включить отображение меню Grub.
- Попасть в систему без пароля несколькими способами.
- Установить систему с LVM, после чего переименовать VG.

# Включить отображение меню Grub.

vim /etc/default/grub

![image](https://github.com/user-attachments/assets/487bd897-5fce-4c24-96c4-af87ca3157e6)

update-grub

![image](https://github.com/user-attachments/assets/74ca217d-e63b-406f-aaea-b0cf8e1b95ed)

# Попасть в систему без пароля несколькими способами.

# Способ 1

В прошлом меню нажимаем "e" и пишем для дебиа-подобых ОС init=/bin/bash в графе linux, затем Contrl + x

![image](https://github.com/user-attachments/assets/33f90d13-29c6-4587-a8e6-ac873c560769)

mount

![image](https://github.com/user-attachments/assets/c42cc7d7-2816-4944-9c1f-a99be553cae6)

mount -o remount,rw /

![image](https://github.com/user-attachments/assets/0d8cf8e2-1b2a-4418-a02c-b9d3f20cfea0)


# Способ 2

![image](https://github.com/user-attachments/assets/17f68864-7038-4c9b-8b5d-1eb5b799bf80)


![image](https://github.com/user-attachments/assets/387f3250-d1e0-4bfd-a22c-b871e22bd8ec)

В зависимости от проблемы, делаем восстановлени:

![image](https://github.com/user-attachments/assets/fb1f784a-7c83-4231-9434-774f698e46ad)

# Установить систему с LVM, после чего переименовать VG

Дано:

![image](https://github.com/user-attachments/assets/246fdd00-63f6-4c65-9682-1ff64d2e7b85)


vgrename ubuntu-vg ubuntu-otus

![image](https://github.com/user-attachments/assets/35b04444-de1e-4f44-bef5-84c47e83e0ca)

vim /boot/grub/grub.cfg

![image](https://github.com/user-attachments/assets/e169dd2c-59ac-4881-8c1f-9fb84739c0b5)

update-grub

reboot

![image](https://github.com/user-attachments/assets/b1f50493-ad7f-4afa-954b-6e0ce896dc81)

