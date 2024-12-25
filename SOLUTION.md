# Решение лабораторной работы

В данной лабораторной работе будет представлено решение к созданной лабораторной работе по восстановлению файлов.

## Задача

*Вашей задачей является восстановить файл при помощи функционала ext3grep. В конце лабораторной работы прикрепите скриншот, в котором видно, что файл восстановлен.*

## Решение

1. Для начала создадим систему ext3 для дальнейшей работы. Для этого пропишем `sudo umount /dev/sda1`.

![image](https://github.com/user-attachments/assets/d473fccc-8f1d-4fbb-ad69-6848b5e4f2c0)

2. После этого создадим папку с тремя файлами. Назовём их `file1`, `file2` и `file3`. Установим ext3grep.

![image](https://github.com/user-attachments/assets/1ac415e7-ba32-45b0-a07e-c5e2ce91d5f8)

3. Удалим файл `file1` и проведём анализ того, что было удалено.

![image](https://github.com/user-attachments/assets/1a821397-28df-4669-b399-d25b5db46555)

4. Восстановим файл командой `sudo ext3grep --restore-all /dev/sda1`.

![image](https://github.com/user-attachments/assets/63609f02-1999-4a09-aedb-18d6ae5f582f)

5. Теперь восстановленый файл можно найти в директории `~/RESTORED_FILES`.

![image](https://github.com/user-attachments/assets/facbae37-b0e2-4bbb-ba04-f5de237c0b0d)
