# System-boot-GRUB-
## Домашнее задание
### Попасть в систему без пароля несколькими способами
1.  **Способ 1**
2.  При загрузке ОС нажимаем  **e** .  Далее в конце строки, которая начинается с **linux /boot/vmlinuz....** пишем  ``` init=/bin/bash ```. Попадаем в ОС. Но в режиме **ro (read only)**. Используем комманду ``` mount -o remount,rw / ```  и проверяем, что можем создавать/ изменять под правами суперпользователя.
3.  ![alt text](./Pictures/1.png)
4.  ![alt text](./Pictures/2.png)
5.  ![alt text](./Pictures/3.png)
6.  **P.S.** т.к. у меня не получилось войти в систему Debian при загрузке командой ``` rd.break ```, установил ОС CentOS и изменил пароль как в ДЗ. Для Debian менял пароль root если при загрузке использовать ``` init=/bin/bash ```.
7.  **Способ 2**
8.   ![alt text](./Pictures/5.png)
9.   **Способ 3**
10.   В строке, начинающейся с linux16, заменяем ro на rw init=/sysroot/bin/sh и нажимаем сtrl-x - так же на CentOS - все получилось

