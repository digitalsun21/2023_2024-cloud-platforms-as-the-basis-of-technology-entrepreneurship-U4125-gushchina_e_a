University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FTMI](https://ftmi.itmo.ru)
Course: [Cloud platforms as the basis of technology entrepreneurship](https://) ADD link
Year: 2024
Group: U4125
Author: Gushchina Ekaterina
Lab: Lab2
Date of create: 22.04.2023
Date of finished: 22.04.2023


# Отчет по лабораторной работе №2
1. Создала Cloud Run из представленного сервиса Hello
<img width="576" alt="Снимок экрана 2024-04-22 в 10 58 27 AM" src="https://github.com/digitalsun21/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-gushchina_e_a/assets/166996616/91f378af-9b45-4ab6-b9a9-163a2bf5f0d2">
<img width="1010" alt="Снимок экрана 2024-04-22 в 11 21 29 AM" src="https://github.com/digitalsun21/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-gushchina_e_a/assets/166996616/41987d9b-a068-4900-9928-596d10264fd4">
<br>
<br>
2. При переходе по ссылке предоставленной Cloud Run получили информацию об успешноо развернутом контейнере
<img width="842" alt="Снимок экрана 2024-04-22 в 10 59 14 AM" src="https://github.com/digitalsun21/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-gushchina_e_a/assets/166996616/9e4f23cb-344a-4312-960c-f1cb90772c54">
<br>
<br>
3. Изучила представленные логи, отображающие историю записей о событиях.<br>
Например, первый лог является записью аудита (audit_log) о создании сервиса (Services.CreateService) в Cloud Run.<br>
Второй лог сообщает о том, что условие готовности (Ready condition status) для ревизии hello-00001-j7p изменилось на True, то есть система проверила его готовность к обработке входящих запросов<br>
Третий лог информирует о том, что контейнер успешно запущен и готов принимать HTTP-запросы<br>
   <img width="1357" alt="Снимок экрана 2024-04-22 в 11 05 41 AM" src="https://github.com/digitalsun21/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-gushchina_e_a/assets/166996616/507f1391-50da-4733-9456-1a103039f585">
   
<br>
<br>
Ознакомилась с метриками.<br>
Например, Метрика "Request count" отображает количество запросов, поступающих к приложению в единицу времени.<br>
Метрика "Request latencies" отображает задержки при обработке запросов приложением.<br>
Метрика "Container instance count" отображает количество экземпляров контейнеров, запущенных для вашего приложения.<br>
Метрика "Billable container instance time" отображает время, в течение которого были запущены и использованы экземпляры контейнеров, за которые вам будет начислена плата. <br>
<img width="1416" alt="Снимок экрана 2024-04-22 в 11 09 35 AM" src="https://github.com/digitalsun21/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-gushchina_e_a/assets/166996616/91fb93f8-f8c8-46ff-9982-129701434e6b">
<br>
<br>
4. Изменила порт на 8090 в Cloud Run <br>
<img width="565" alt="Снимок экрана 2024-04-22 в 11 11 02 AM" src="https://github.com/digitalsun21/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-gushchina_e_a/assets/166996616/c10a4ad5-ac76-4cb2-a089-c5f01362fac4">
<br>
После смены порта, поменялось имя активной версии
<img width="974" alt="Снимок экрана 2024-04-22 в 11 12 07 AM" src="https://github.com/digitalsun21/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-gushchina_e_a/assets/166996616/fa98737b-1867-4402-8d6d-dcce81f54973">
<br>
<br>
При смене версии и нагрузки, на графиках с метриками появляются засечки, сигнализирующие об изменениях
<img width="717" alt="Снимок экрана 2024-04-22 в 12 03 30 PM" src="https://github.com/digitalsun21/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-gushchina_e_a/assets/166996616/7dfef4f8-c574-4db7-9cfa-c3a48dcae89e">

<br>
<br>
Таким образом, Сloud Run представляет собой платформу для запуска контейнеров. Она обеспечивает возможность развертывания сервиса в облаке без необходимости управления инфраструктурой. Также платформа обладает анлалитикой в виде отслеживания метрик и логов, что полезно для контроля устойчивости сервиса и поиска ошибок. 
