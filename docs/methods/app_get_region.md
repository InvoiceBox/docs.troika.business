---
layout: default
nav_order: 20
title: Список регионов
parent: "Методы API"
---

# Получение доступных регионов

Для получения списка доступных регионов, необходимо вызвать следующий метод API:

- HTTP метод: `POST`
- наименование метода API: `app_get_region`

## Параметры запроса

Запрос не предполагает наличие параметров.


## Параметры ответа

| Параметр    | Обязательный | Тип                   | Описание           | Пример значения                   |
|-------------|--------------|-----------------------|--------------------|-----------------------------------|
| region      | Да           | ARRAY OF regionItem   | Массив регионов    | См. описание объекта regionItem   |


## regionItem

| Параметр     | Обязательный | Тип        | Описание                       |
|--------------|--------------|------------|--------------------------------|
| id           | Да           | STRING     | Идентификатор                  |
| name         | Да           | STRING     | Наименование                   |

[Читать далее &raquo;](/docs/methods/app_create_order/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
