University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FTMI](https://ftmi.itmo.ru)
Course: [Cloud platforms as the basis of technology entrepreneurship](https://) ADD link
Year: 2024
Group: U4125
Author: Gushchina Ekaterina
Lab: Lab1
Date of create: 19.04.2023
Date of finished: 19.04.2023


# Отчет по лабораторной работе №1

1. Создала service account с названием egushchina-sa-lab1 и ролью Storage Admin
<img width="583" alt="Снимок экрана 2024-04-19 в 11 17 09 PM" src="https://github.com/digitalsun21/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-gushchina_e_a/assets/166996616/9791501e-df00-48e7-ba2a-e7fc3abe33fe">

2. Создала виртуальную машину с названием  egushchina-vm-lab1 на основе упомянутого service account
<img width="1048" alt="Снимок экрана 2024-04-19 в 11 19 12 PM" src="https://github.com/digitalsun21/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-gushchina_e_a/assets/166996616/21fb2793-2ce6-45b3-822d-fe86a2b35e83">


3. Скопировала 3 файла из lab1-bucket-itmo в созданную виртуальную машину с помощью утилиты "gsutil" и проверила нахождение файлов на виртуальной машине с помощью команды ls -lah 
<img width="927" alt="Снимок экрана 2024-04-19 в 11 05 28 PM" src="https://github.com/digitalsun21/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-gushchina_e_a/assets/166996616/a36bfe20-a540-48e3-abd1-ef1117f2f7c9">

4. Сменила права доступа service account с Storage Admin на Compute Viewer
<img width="1145" alt="Снимок экрана 2024-04-19 в 11 26 23 PM" src="https://github.com/digitalsun21/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-gushchina_e_a/assets/166996616/30829e5c-ccb0-47dd-8c6f-1b91b0d05f86">


5. После смены роли на Compute Viewer скопировать файлы в виртуальную машину не удалось, так как у service account недостаточно прав. Роль Compute Viewer предоставляет возможность просмотра и перечисления ресурсов Compute Engine с ограниченным доступом к данным, хранящимся на этих ресурсах. Это означает, что пользователь с этой ролью может видеть информацию о виртуальных машинах, сетях и других ресурсах Compute Engine, но не имеет права копировать содержимое, хранящееся на этих ресурсах.
<img width="1429" alt="Снимок экрана 2024-04-19 в 11 08 33 PM" src="https://github.com/digitalsun21/2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-gushchina_e_a/assets/166996616/04f69d03-2f9c-4b50-975a-31e7f208ed89">



## итог
В Google Cloud Storage существует разнообразие ролей, которые позволяют ограничивать и предоставлять доступ к бакетам или отдельным сервисам в облаке. 



