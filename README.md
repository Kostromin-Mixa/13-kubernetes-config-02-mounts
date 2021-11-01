# Домашнее задание к занятию "13.2 разделы и монтирование"   
Создан NFS сервер. Вывод примера создания PVC для этого NFS сервера.   
![nfs](https://user-images.githubusercontent.com/78191008/139725720-de218ed4-cd8a-4de9-9e33-87d42d2dbfc3.png)   
__1 задание__   
- Создан POD "pod-int-volumes" с двумя контейнерами "frontend" и "backend" и общей папкой /static   
  
- В общую папку в контейнере bacend помещён файл test.txt   
- Из контейнера frontend файл test.txt так же доступен:   
![2021-11-01_23-52-04](https://user-images.githubusercontent.com/78191008/139729254-facbac01-84f3-40a0-a1db-c39aafc1875f.png)
