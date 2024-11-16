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

В разделе IAM создан service account с ролью Storage Admin.

![1](https://github.com/user-attachments/assets/b605bf9e-d621-4f71-9838-59929172e149)

Создана виртуальная машина - Machine type e2-micro в режиме spot
![image](https://github.com/user-attachments/assets/15d15a99-1840-4b2c-93c1-46e84e68d0bb)

С помощью утилиты gsutils найден бакет lab1-bucket-itmo и скопированы 3 файла в локальную папку на VM
![image](https://github.com/user-attachments/assets/c9c6f8c5-83ac-4cc9-9589-021962f48092)

Затем роль Service Account была изменена на Compute Viewer
![image](https://github.com/user-attachments/assets/c4e348ad-0457-40d0-9d1f-731ec42b5541)

Это привело к тому, что файлы стали недоступны для копирования
![image](https://github.com/user-attachments/assets/e2d5f019-6709-4d6a-91bb-22f9f987d21f)

Вывод:
Роль Storage Admin предоставляет полный контроль над контейнерами, папками, управляемыми папками и объектами. Compute Viewer дает доступ только для чтения и для получения и просмотра информации обо всех ресурсах Compute Engine, включая экземпляры, диски и брандмауэры. Роль Compute Viewer позволяет получать и просматривать информацию о дисках, образах и снимках, но не позволяет читать хранящиеся на них данные.
