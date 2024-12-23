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
Снова удалите ранее созданный файл, но уже через консоль, а затем запустите TestDisk командой:
```
sudo testdisk
```
Вашей задачей является восстановить удалённый файл в ту же директорию, где он находился. После этого восстановите его в другую директорию и прикрепите скриншоты обоих вариантов.
Проведите аналогичную работу, но с PhotoRec. Для наглядности назовите файл для работы не так, как первый. Не забывайте удалять файл через консоль. Установка и запуск производятся командами:
```
sudo apt -y install photorec
sudo photorec
```

## Источники

- [TestDisk](https://www.cgsecurity.org/wiki/TestDisk_RU)
- [PhotoRec](https://www.cgsecurity.org/wiki/PhotoRec_RU)
- [Инструкция по работе с файлами](https://selectel.ru/blog/tutorials/files-and-directories-in-linux/)
- [Сайт, где можно найти ответ на любой вопрос](https://stackoverflow.com)
