# heat_map
тестовое задание для RB1

установить - как обычный laravel проект (PHP 7.3)

Три архива 
          heat_map_app_ngnix - для локальных версий и хостинга, на котором в конфиге nginx прописанно merge_slashes off; - эта версия отличается путем к тепловой карте(без GET параметра)
          heat_map_app_mchost_vps - версия адаптированная под vps хостинг макхост, ссылка на уже запущенный сайт: https://test-heat-map.mcdir.ru/ версия отличается прописанными .htaccess и адаптированными путями к файлам в контроллерах, а также ссылками на карты с get параметром
          heat_map_db - два файла импорта базы данных, одна с тестовыми данными, вторая без
          
В проекте прописаны миграции и сидер, поэтому после подключения к бд (.env файл) еть возможность не импортировать базу данных, а создать её из приложения: 
php artisan migrate / php artisan migrate:refresh / php artisan migrate:refresh --seed

более подробно о проекте можно прочитать на странице о приложении, после установки

@Газин Максим
