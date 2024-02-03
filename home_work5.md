1) Установить на хост redis (https://redis.io/docs/install/intall-redis/install-redis-on-linux/)
2) Проверить что сервис redis попал в автозагрузку (enable) и запущен
3) Остановить, запустить снова, проверить статус и логи (journalctl)
4) Вывести список всех юнитов; вывести только юниты со статусом inactive (ключ --stat)
5) Получить уровень, на котором запускается юнит, не заглядвая в его файл (get-default)
6) Написать свой юнит файл для второго экземпляра redis
!!! Мы НЕ собираем кластер, мы просто поднимаем еще один сервис
!!! В конфигурации как минимум должен отличаться порт, на котором слушает redis
8) Запустить consul template (https://github.com/hashicorp/consul-template?tab=readme-ov-file#installation) как systemd юнит
