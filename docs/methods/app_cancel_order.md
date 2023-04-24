---
layout: default
nav_order: 61
title: Отмена билетов в заказе
parent: "Методы API"
---

# Отмена билетов в заказе

Для отмены билетов в заказе, необходимо вызвать следующий метод API:

- HTTP метод: `POST`
- наименование метода API: `app_cancel_order`


## Параметры запроса

| Параметр  | Обязательный | Тип         | Описание                         | Пример значения                |
|-----------|--------------|-------------|----------------------------------|--------------------------------|
| orderId   | Да           | INT         | Идентификатор заказа             | 234356                         |


<details>
  <summary>Пример запроса</summary>
<section markdown="1">
``` json
{
    "message": {
        "head": {
            "type": "app_cancel_order",
            "languageId": "ru",
            "phone": "+72348544565",
            "terminalId": "bus_d23bcd26b59741a",
            "time": "2022-04-22 10:35:31 +03:00"
        },
        "body": {
            "orderId": 645896
        }
    }
}
```
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
}
```
</section>
</details>


[Читать далее &raquo;](/docs/methods/app_get_businessaccount/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
