# Лабораторная работа: Восстановление файлов

В этой лабораторной работе мы познакомимся с тем, как восстановить удалённые файлы и где их можно найти, когда, казалось бы, всё потеряно.

## Пример

Начнём с простого: восстановление из корзины. Создайте любой файл, например `my_favourite.bash`, а затем удалите его.
```
touch my_favourite.bash
```
Перейдите в директорию корзины по пути `~/.local/share/Trash` и восстановите удалённый файл в путь, где он изначально находился.
```
mv my_favourite.bash <ваш путь>
```

## Задание

Перейдём к процессу удаления и восстановления файлов через консоль с помощью TestDisk. Установите его командой:
```
sudo apt install testdisk
```
Снова удалите ранее созданный файл, но уже через консоль, а затем запустите PhotoRec командой ():
```
sudo photorec
```
Вашей задачей является восстановить удалённый файл в отдельную папку. Для наглядности можете назвать её Recovery. Проведите аналогичную работу, но с ext3grep. Не забывайте удалять файл через консоль. Установка и запуск производятся командами:
```
sudo apt install ext3grep
```
Создайте /mnt/T_DRIVE и перейдите туда. Создайте там файл для примера любого разрешения, а затем удалите. Запустите команду с параметром --dump-name, чтобы посмотреть все файлы, которые находились в этой директории на устройстве. Восстановите те, которые удаляли. Прикрепите скриншоты. Команда с параметром выглядит следующим образом:
```
ext3grep --dump-name <имя устройства>
```

## Источники

- [TestDisk](https://www.cgsecurity.org/wiki/TestDisk_RU)
- [PhotoRec](https://www.cgsecurity.org/wiki/PhotoRec_RU)
- [Инструкция по работе с файлами](https://selectel.ru/blog/tutorials/files-and-directories-in-linux/)
- [Сайт, где можно найти ответ на любой вопрос](https://stackoverflow.com)
