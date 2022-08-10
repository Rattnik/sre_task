
## Описание

Репозиторий содержит API написанную на GO которая взаимодействует с БД. Основное предназначение API - управление записями находящимися в таблице `contacts`.  
Схема взаимодействия компонентов: `Nginx:443 ssl -> APP_Backend -> DB`

## Задача
Необходимо собрать приложение и развернуть его в Docker через docker-compose. Часть функционала уже написана инженером, но он не успел его закончить. В текщей версии деплоя могут возникать ошибки - **основня цель задания исправить все ошибки и запустить приложение.** Код самого приложения исправлять или дописывать не нужно.

## Условия выполнения
- Деплой должен являться идемпотентным не зависимо от состояния/наличия временных файлов и файлов данных.
- Приложение должно открываться по ссылке app.yandex.ru
- В БД по умолчанию должна быть следующая запись: `id="1", fullname="Yurij Dyatlov", address="Kazan, st.Komsomolskaya d.53 kv.22", phonenumber="312997789", email="y.dyatlov@ygoogle.com"`. Схема таблицы БД на ваше усмотрение.


## Оформление
- Создать свой репозиторий на основе текущего в GitHub
- Добавить права на чтение для следующих пользователей @Rattnik, @pashtet04, @diarworld
- Создать ветку feature/Git
- После выполнения задания отправить изменения в ветке feature/Git в Github и создать PR в ветку main
- В качестве reviewer указать пользователей @Rattnik, @pashtet04, @diarworld
- Все дополнительные действия необходимые от пользователя для запуска приложения должны сопровождаться инструкцией - создать файл DEVELOPMENT.md в корне репозитория.Но деплой должен быть максимально автоматизирован
- При желании создайте дополнительный контейнер с необходимым окружением для тестирования работы API. В качестве инструмента тестирования можно использовать любой скриптовый язык.(данный пункт не является обязательным)
- Отправить ссылку на PR через HR или контактное лицо для проверки
