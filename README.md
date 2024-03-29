# Модуль OpenCart 2.3 для Украины

## Чеклист интеграции:
- [x] Установить модуль.
- [x] Передать тех поддержке PSP Platon  ссылку для коллбеков.
- [x] Провести оплату используя тестовые реквизиты.

## Установка:

* Распаковать архив в корень сайта.

* В админ панеле перейти Extensions → Payments → Platon.

* Нажите "Install", потом "Edit".

* В настройках указать ключ и пароль. Настройте статусы транзакций Pending для Order Status и Refunded как Refunded Order Status.

* Установить значение платежного метода в статус Enabled.

## Иностранные валюты:
Готовые CMS модули PSP Platon по умолчанию поддерживают только оплату в UAH.

Если необходимы иностранные валюты необходимо провести правки модуля вашими программистами согласно раздела [документации](https://platon.atlassian.net/wiki/spaces/docs/pages/1810235393).

## Ссылка для коллбеков:
https://ВАШ_САЙТ/index.php?route=extension/payment/platon/callback

## Тестирование:
В целях тестирования используйте наши тестовые реквизиты.

| Номер карты  | Месяц / Год | CVV2 | Описание результата |
| :---:  | :---:  | :---:  | --- |
| 4111  1111  1111  1111 | 01 / 2024 | Любые три цифры | Успешная оплата без 3DS проверки |
| 4111  1111  1111  1111 | 02 / 2024 | Любые три цифры | Не успешная оплата без 3DS проверки |
| 4111  1111  1111  1111 | 05 / 2024 | Любые три цифры | Успешная оплата с 3DS проверкой |
| 4111  1111  1111  1111 | 06 / 2024 | Любые три цифры | Не успешная оплата с 3DS проверкой |
