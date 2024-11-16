University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: Cloud platforms as the basis of technology entrepreneurship

Year: 2024/2025

Group: U4225

Author: Volkov Vladislav Alekseevich

Lab: Lab1

Date of create: 16.11.2024

Date of finished: 16.11.2024

# Ход работы

Был создан Cloud Run из сервиса Hello
![image](https://github.com/user-attachments/assets/6e009046-cf92-41a9-896e-e580d8acce72)

Сервис успешно запушен
![image](https://github.com/user-attachments/assets/27b4bdea-14b3-431b-8745-a8c218d0f3fd)

Логи
![image](https://github.com/user-attachments/assets/f45bf44b-f642-4a75-847d-d7dd151f5970)

Метрики
![image](https://github.com/user-attachments/assets/79b3c691-a928-4b7a-b0fb-8d1c1f021157)
![image](https://github.com/user-attachments/assets/140463a5-f0d6-47d4-9292-81f77c6f260d)
![image](https://github.com/user-attachments/assets/4b2b7143-4833-4cdf-bac7-03ac390fdf8a)

Меняем порт с 8080 на 8090 и при распределении нагрузки 15% и 85% между портами
![image](https://github.com/user-attachments/assets/353825c8-da2e-44c1-b45e-ccf70239d927)

Получаем следующие показатели
![image](https://github.com/user-attachments/assets/4d53334d-6830-4b42-a83c-ec180b7ba298)
![image](https://github.com/user-attachments/assets/1224b1cc-7fd6-49ca-8368-f97bb524d8e4)
![image](https://github.com/user-attachments/assets/864e9399-c9fe-4c1b-b3af-13424805a653)
![image](https://github.com/user-attachments/assets/9c2031c1-1cff-4670-a80c-93f1bfb729fd)

При распределении поровну получаем следующее
![image](https://github.com/user-attachments/assets/fcd1e835-da18-441d-ba95-d6b6996cf4e3)
![image](https://github.com/user-attachments/assets/0bc38910-045a-43e7-a0d1-56d184abb932)
![image](https://github.com/user-attachments/assets/361caedc-feb0-4a61-83ee-c9c1ffc87890)
![image](https://github.com/user-attachments/assets/9f105306-ed1f-4a32-a466-8b2659316761)

## Вывод
Распределение нагрузки поровну является наиболее оптимальным, так как использование памяти и задержка запросов уменьшаются.
