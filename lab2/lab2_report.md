University: ITMO University 

Faculty: FTMI

Course: Cloud platforms as the basis of technology entrepreneurship ADD link 

Year: 2023/2024 

Group: U4125 

Author: Vakhromeeva Yulia Vladimirovna

Lab: Lab1 Date of create: 03.05.2024 

Date of finished: 07.05.2024

# Лабораторная работа №2 "Исследование Cloud Run"
Создан Cloud Run из представленного дефолтного сервиса Hello с минимальным количеством ресурсов.

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/1a1b1806-0ff5-4f3c-a5a1-84fcd3c8638f)


![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/cc66585d-ae78-4291-9647-ac86ca76e95f)


Перешла по ссылке предоставленной Cloud Run, протестировала сервис.

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/3013b2dc-2e09-421f-a409-9f147d87efa8)


Перешла в разделы логи и метрики

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/b6023be4-083b-480c-a34f-4327212b11d6)

# Метрики:
Количество запросов (Request Count)- общее количество запросов, полученных вашим приложением за определенный период времени. 

Среднее время ответа (Average Response Latency) - среднее время, требуемое для обработки одного запроса вашим приложением.

Процент ошибок (Error Rate) - процент запросов, которые привели к ошибке сервера или другим неуспешным ответам. 

Использование памяти (Memory Usage) - объем памяти, используемой вашим приложением в данный момент времени. 

Процент загрузки CPU (CPU Load) - процент использования CPU вашим приложением. 

Процент успешных запросов (Success Rate) - процент успешных запросов, которые завершились без ошибок. 

Проанализировать их можно после нескольких переходов по тестовой ссылке.

# Логи
Позволяют отслеживать действия и события, происходящие в приложении.

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/423f69d9-f2e4-4b13-835e-4a09de1aca9c)

Проанализируем один из логов: 2024-05-03 23:27:37.508 MSK GET2005.44 KB3 msChrome 124 https://yvakhromeeva-lab2-syptpw5q4q-uc.a.run.app/ 
Время: 2024-05-03 23:27:37.508 MSK

Метод: GET

Код состояния: 200 (Успешно)

Размер ответа: 5.44 KB

Время ответа: 3 мс

Браузер: Chrome

Страница: https://yvakhromeeva-lab2-syptpw5q4q-uc.a.run.app/

Этот лог указывает на успешный запрос типа GET к приложению. Размер ответа составил 5.44 KB, время ответа было всего 3 мс. Пользователь (я) использовала браузер Chrome и перешла на страницу https://yvakhromeeva-lab2-syptpw5q4q-uc.a.run.app/.

Изменила Cloud Run, поменяв порт на 8090.

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/05428c46-b60a-47dc-afbc-97c8548071fd)

Добавился новый порт для передачи данных.

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/50b802fe-ba32-4585-9358-88286480dfe9)

Переключила трафик между версиями.

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/66aa490f-f8ab-4c53-a1f1-ce1a4caef045)

Изменились данные в метриках и логах (вертикальные линии показывают изменения трафика).

![image](https://github.com/Yuliagkk/2023_2024-cloud-platforms-as-the-basis-of-technology-entrepreneurship-u4125-vakhromeeva_u_v/assets/166257005/8148f672-a73d-4ed4-b962-b1589dc2302c)





