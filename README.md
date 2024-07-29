# Домашнее задание к занятию «Микросервисы: принципы»

## Задача 1: API Gateway

Предложите решение для обеспечения реализации API Gateway. Составьте сравнительную таблицу возможностей различных программных решений. На основе таблицы сделайте выбор решения.

Решение должно соответствовать следующим требованиям:

- маршрутизация запросов к нужному сервису на основе конфигурации,

- возможность проверки аутентификационной информации в запросах,

- обеспечение терминации HTTPS.

### Ответ

Подобрал несколько популярных и мощных инструментов, некоторые имеют платную версию, но в бесплатной версии так же соответствуют нашим требованиям.

| Решение | Маршрутизация запросов | Аутентификация информации | Терминация HTTPS |
|:---:|:---:|:---:|:---:|
Kong | да | да | да |
Tyk | да | да | да |
Envoy | да | да | да |
Yandex | да | да | да |
Apigee |да | да | да |

Т.к. все сервисы обладают необходимыми функциями, то я бы выбрал популярное open source решение Kong.

## Задача 2: Брокер сообщений

Составьте таблицу возможностей различных брокеров сообщений. На основе таблицы сделайте обоснованный выбор решения.

Решение должно соответствовать следующим требованиям:

- поддержка кластеризации для обеспечения надёжности,

- хранение сообщений на диске в процессе доставки,

- высокая скорость работы,

- поддержка различных форматов сообщений,

- разделение прав доступа к различным потокам сообщений,

- простота эксплуатации.

### Ответ

Под описанные требования подходят следующие решения:

- Apache Kafka
- Rabbit MQ
- Active MQ
- Google Cloud Pub/Sub
- Yandex MQ

Исходя из финансовой составляющей и простоты управления, я бы выбрал Rabbit MQ.
