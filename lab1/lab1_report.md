University: ITMO University 

Faculty: FTMI

Course: Cloud platforms as the basis of technology entrepreneurship ADD link 

Year: 2023/2024 

Group: U4125 

Author: Vakhromeeva Yulia Vladimirovna

Lab: Lab1 Date of create: 02.05.2024 

Date of finished: 07.05.2024

# Лабораторная работа №1 "Обзор Google Cloud и исследование основных сервисов"
Во вкладке IAM был создан service account с ролью Storage Admin.

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/f69e109b-cd7b-4324-90b9-0ebcd93d8a51)

Далее был создан минимальный compute engine (виртуальная машина) с Machine type e2-micro в режиме spot.

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/cd50a493-7cd8-43a2-9e79-5f38ce31c069)

С помощью утилиты gsutils найден бакет lab1-bucket-itmo и скопированы 3 файла в локальную папку на VM. 

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/49b7687d-d7cf-4518-9eb5-c1246384481a)

Используя команду ls -lah отображены файлы, хранящиеся на VM.

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/1668e347-9d69-4150-804c-80c7a1c00ddf)

После этого мы должны видеть информацию о скопированных файлах в локальной папке на виртуальной машине.

Во вкладке IAM поменяла права доступа для service account с Storage Admin на на Compute Viewer.

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/44853f9a-ccac-4928-ba69-0a43eb85c8ef)

Повторила пункт с копированием данных, предварительно перезапустив машину

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/fe8b8e43-cd45-4f75-b651-18dcebb82901)


Вышла ошибка "AccessDeniedException: 403", потому что у service account теперь нет разрешения на доступ к бакету Storage.

# Вывод: Изменение роли service account с Storage Admin на Compute Viewer привело к потере доступа к бакету Storage, так как Compute Viewer не имеет прав на доступ к хранилищу. Это означает, что изменение прав доступа влияет на действия, которые можно выполнять с использованием данного service account.
