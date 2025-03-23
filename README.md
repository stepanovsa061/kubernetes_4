# kubernetes_4

# Задание 1. Создать Deployment и обеспечить доступ к контейнерам приложения по разным портам из другого Pod внутри кластера
1) Создать Deployment приложения, состоящего из двух контейнеров (nginx и multitool), с количеством реплик 3 шт.
2) Создать Service, который обеспечит доступ внутри кластера до контейнеров приложения из п.1 по порту 9001 — nginx 80, по 9002 — multitool 8080.
3) Создать отдельный Pod с приложением multitool и убедиться с помощью curl, что из пода есть доступ до приложения из п.1 по разным портам в разные контейнеры.
4) Продемонстрировать доступ с помощью curl по доменному имени сервиса.
5) Предоставить манифесты Deployment и Service в решении, а также скриншоты или вывод команды п.4.

Создал Deployment приложения, Service, отдельный Pod с приложением multitool 

![1 1](https://github.com/user-attachments/assets/21e94bb1-f7d0-4f8c-81b1-dc9400d2dce8)

Проверяю моандой curl доступность

![1 2 curl 1](https://github.com/user-attachments/assets/aba9817f-509d-4d68-b3e4-c3c9d2703f45)

![1 3 curl 2](https://github.com/user-attachments/assets/c42a2304-7af0-40c0-b01e-f8a6b3a3a0c2)

![1 4 curl 3](https://github.com/user-attachments/assets/3f7e7ca6-7f2c-4314-8c15-d9d3fb4255a5)

Проверяю моандой curl доступность по доменному имени сервиса

![1 5 curl dom name](https://github.com/user-attachments/assets/62458f20-b139-45eb-bab8-1bcaeefbf854)


# Задание 2. Создать Service и обеспечить доступ к приложениям снаружи кластера
1) Создать отдельный Service приложения из Задания 1 с возможностью доступа снаружи кластера к nginx, используя тип NodePort.
2) Продемонстрировать доступ с помощью браузера или curl с локального компьютера.
3) Предоставить манифест и Service в решении, а также скриншоты или вывод команды п.2.

Создал отдельный Service

![2 1 created](https://github.com/user-attachments/assets/08152f97-1412-4bbc-b897-236ab045d2b8)

Проверим доступ с помощью curl с локального компьютера

![2 1 curl](https://github.com/user-attachments/assets/4396bcd5-1e3c-4ab7-8dbf-d0ea7cc96752)




