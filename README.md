﻿My Watching Manager.
Add chanel as user name, like www.youtube.com/user/zapatou ==> zapatou
Then sync and enjoy.
Add RuTracker, you can suscribe to user releases, like http://rutracker.org/forum/tracker.php?pid=2638398 ===> 2638398

![Main Window](https://raw.githubusercontent.com/v0vc/Ytub/master/Screens/main.png)

![Settings](https://raw.githubusercontent.com/v0vc/Ytub/master/Screens/settings.png)

![Popular](https://raw.githubusercontent.com/v0vc/Ytub/master/Screens/popular.png)

Приложение позволяет "подписаться" на канал Youtube, не имея регистрации на самом сайте. Данные хранятся в локальной базе данных. 
При синхронизации зеленым выделяются те видео, которые уже были синхронизованы, красным - новые. 
Если хотя бы одно видео новое - канал будет подсвечен красным. Списки видео можно фильтровать по названию.

Имеется возможность добавлять канал в избранное и синхронизовать только избранное.
В настройках есть опция, получать ли при старте "популярное", а также регион. На закладке Popular можно выбрать регион, отличный от того, что указан в настройках.
Каналы можно сортировать, сортировка хранится в базе.

При скачивании формируется локальная библиотека с доступом из приложения. Скачанные файлы помечаются зеленой галочкой. 
Клик по элементу колонки Download скачает видео в качестве 720р, клик по иконке File - максимально доступное качество.
Двойной клик по строке видео при наличии локального файла запустит ассоциированное приложение для просмотра. При отсутствии локального файла - MPC-BE онлайн.

Для объединения аудио и видео дорожек используется ffmpeg, т.к ютуб хранит в максимальном качестве отдельно аудио, отдельно видео.

18.12.14
Пофиксил вылет при обновлении ffmpeg в x64, сортировка в новой синхронизации.

17.12.14
Убрал тормоза при старте и синхронизации, все сторонние библиотеки - через nuget. Синхронизация - последние 25, дабы не ворочать все элементы. Но под правой кнопкой можно обновить целиком.

16.12.14
Прикрутил иконки.

15.12.14
Добавлено отображение информации для рутрекера - сидеры, размер в мб и общее количество скачиваний (позволяет быстро найти наиболее популярные торренты).