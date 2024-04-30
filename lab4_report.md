University: [ITMO University](https://itmo.ru/ru/)\
Faculty: [FTMI](https://ftmi.itmo.ru)\
Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/education/labs2023-2024/lab1/lab1/)\
Year: 2024\
Group: U4125\
Author: Gaptelganieva Guzel\
Lab: Lab4\
Date of create: 30.04.2024\
Date of finished:

## Лабораторная работа №4 "Разработка инфраструктуры MVP AI приложения."

### Описание приложения:
Телеграм-бот, который раз в несколько часов присылает пользователю приятную картинку или текст из базы данных или сгенерированный искусственным интеллектом.

### Инфраструктура (схема):
![image](https://github.com/guzel148/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-gaptelganieva_g_r/assets/156536395/71e3553a-669d-46d1-aafb-1f5debdca4fa)

### План (ресурсы)
1. Начальное состояние:
   - Веб-сервер (Google Cloud Functions) для обработки запросов от пользователей и генерации контента
   - Хранение данных в NoSQL базе данных (Google Cloud Firestore) для хранения сгенерированных текстов и ссылок на изображения
   - Облачное хранилище (Google Cloud Storage) для хранения сгенерированных изображений
   - Мониторинг и логирование (Google Cloud Monitoring и Google Cloud Logging)

2. Тестирование партнерами:
   - Увеличение вычислительных ресурсов на веб-сервере для обработки дополнительной нагрузки
   - Дополнительные инструменты мониторинга производительности (Google Cloud Profiler)

3. Продовое решение:
   - Развитие масштабируемости с помощью Google Kubernetes Engine (GKE) для управления контейнерами и автоматического масштабирования
   - Использование Cloud CDN для ускорения доставки контента пользователю
   - Резервное копирование данных с использованием Google Cloud Storage Nearline
