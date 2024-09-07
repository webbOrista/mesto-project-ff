# Mesto - галерея путешественника

**Формат проекта**: страница с галереей фотокарточек, которые можно открывать в полный размер. На странице можно лайкать карточки других пользователей, добавлять собственные с помощью формы, удалять их, изменять аватар и редактировать свои данные. Вся обновленная информация сохраняется на сервере.

### [Посмотреть проект](https://webborista.github.io/mesto-project-ff/)

## Используемые технологии

- **HTML**
- **CSS**
- **JavaScript**

## Функциональность, реализованная мной

- **Валидация форм**: 
  - Полностью настроена валидация форм редактирования профиля, обновления аватара, создания новой карточки. 
  - Валидация основана на регулярных выражениях и включает кастомные тексты ошибок.
  - Реализована динамическая связь валидации с состоянием кнопки: если хотя бы одно из полей формы не прошло валидацию, кнопка «Сохранить» становится неактивной.
  - Производится очистка ошибок валидации при закрытии заполненной формы.

- **Интеграция с API**:
  - Получение с сервера массива начальных карточек и данных пользователя.
  - Обновление данных пользователя при редактировании профиля.
  - Отправка данных для добавления новой карточки.
  - Обновление аватара профиля.
  - Удаление карточки.
  - Добавление и снятие лайка с карточки.

- **Избирательное удаление**:
  - Удаление доступно только для своих карточек. Иконка удаления присутствует исключительно на карточках текущего пользователя.

- **Счетчик лайков**:
  - Отображение количества лайков от разных пользователей у карточек.
  - Иконка лайка меняется в зависимости от того, лайкнул ли карточку текущий пользователь.

- **Уведомление о процессе загрузки**:
  - При отправке запросов текст кнопки «Сохранить» меняется на «Сохранение...», уведомляя пользователя о процессе загрузки.

- **Закрытие модальных окон**:
  - Реализовано закрытие модальных окон по клику на крестик, нажатию клавиши `Esc` и клику на оверлей.

---

## Установка зависимостей и запуск проекта:

```bash
npm i
npm run start

```

---

**P.S.**

Вы можете попробовать пройти полный flow сервиса: заменить аватар, отредактировать данные пользователя, добавить собственную карточку с названием и изображением, лайкнуть её и затем удалить.

**P.P.S**

В данный момент на странице отображаются только мои карточки (выставлена фильтрация по id), чтобы избежать отображения неконтролируемого контента от других пользователей.
