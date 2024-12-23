# Решение лабораторной работы

В данной лабораторной работе будет представлено решение к созданной лабораторной работе по восстановлению файлов.

## Задача

*Вашей задачей является восстановить удалённый файл в ту же директорию, где он находился. После этого восстановите его в другую директорию и прикрепите скриншоты обоих вариантов. Проведите аналогичную работу, но с Recover. Для наглядности назовите файл для работы не так, как первый. Не забывайте удалять файл через консоль.*

## Решение

1. Для начала рассмотрим пример. Создадим файл `my_favourite.bash`. Удалим его в корзину и увидим, что в списке файлов его больше нет.

![image](https://github.com/user-attachments/assets/e1101ed3-9f44-4fab-af60-6795391aed62)

2. Перейдём в директорию корзины и восстановим файл оттуда.

![image](https://github.com/user-attachments/assets/fbc8dac9-7be6-487f-a23d-dad3a6b11f6d)

3. Вновь удалим файл, но в этот раз через консоль, и установим TestDisk. Через него запустим `sudo photorec` для того, чтобы восстановить удалённые файлы. После небольших манипуляций в программе мы восстановили потерянные данные в выбранную папку.

![image](https://github.com/user-attachments/assets/18904d5f-abd5-4343-9c21-c3423da12521)

![image](https://github.com/user-attachments/assets/c918ded0-e4d2-4be8-a757-1405c5a84537)

4. Повторим то же самое, но с ext3grep. Установим его и создадим папку T_DRIVE, а в ней файл second_favourite.

![image](https://github.com/user-attachments/assets/bd49a43c-1f39-4ba8-b036-39d544f2aafc)

5. 
