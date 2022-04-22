---
layout: default
nav_order: 60
title: Отмена билета
parent: "Методы API"
---

# Отмена билета в заказе

Для отмены билета в заказе, необходимо вызвать следующий метод API:

- HTTP метод: `POST`
- наименование метода API: `app_cancel_ticket`


## Параметры запроса

| Параметр        | Обязательный | Тип         | Описание                         | Пример значения                |
|-----------------|--------------|-------------|----------------------------------|--------------------------------|
| orderTariffId   | Да           | INT         | Идентификатор билета             | 234356                         |


<details>
  <summary>Пример запроса</summary>
<section markdown="1">
``` json
{
    "message": {
        "head": {
            "type": "app_cancel_ticket",
            "languageId": "ru",
            "phone": "+72348544565",
            "terminalId": "bus_d23bcd26b59741a",
            "time": "2022-04-22 10:35:31 +03:00"
        },
        "body": {
            "msgType": "app_cancel_ticket",
            "orderTariffId": 645896
        }
    }
}```
</section>
</details>


## Параметры ответа

Ответ не предполагает наличие параметров.


<details>
  <summary>Пример ответа</summary>
<section markdown="1">
``` json
{
    "message": {
        "head": {
            "resultCode": 0,
            "resultMessage": "OK"
        }
    }
}}```
</section>
</details>


[Читать далее &raquo;](/docs/security/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
