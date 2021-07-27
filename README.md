## Установка

### Все команды

```
npm i - загрузит все дополнительные пакеты
npm start - запустит для тестирования на локалке
npm run build - скомпилирует проект в папку /dist для выгрузки на хостинге
npm run deploy - скомпилирует и загрузит проект на GitHub Pages
```

### Выгрузка на GitHub Pages
```
npm run deploy
```
Ссылка на GitHub Pages [клик](https://skygopnik.github.io/showbox/)

## Запуск приложения
Для запуска необходимо использовать ссылку `https://vk.com/app7826637` и передать в неё параметры `token`, `userId`

> https://vk.com/app7826637#token=BAW12ZXD&userId=12345

## Ответ приложения
После завершения всех шагов приложение отправит `POST` запрос на URL который указан в `src/views/Main/Main.tsx`, функция `finishStep`

!['функция'](https://i.imgur.com/lDFYaqh.png)

Заменить `https://localhost/test/api` на адрес вашего метода

Приложение отправит в теле запроса следующие данные:
* id - id пользователя или группы ВКонтакте
* type - тип id, группа или пользователя (user или group)
* token - внутренний токен пользователя в приложении ШоуБокс
* userId - внутренний id пользователя в приложении ШоуБокс

## Вопросы или баги
В случаи возникновения вопросов, багов или доработки нового функционала, ждём в [личных сообщениях](https://vk.me/skreglis) SkyReglis Studio