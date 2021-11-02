# Домашнее задание к занятию "13.2 разделы и монтирование"   
Создан NFS сервер. Вывод примера создания PVC для этого NFS сервера.   

![nfs](https://user-images.githubusercontent.com/78191008/139725720-de218ed4-cd8a-4de9-9e33-87d42d2dbfc3.png)   

## 1 задание  
- Создан POD "pod-int-volumes" с двумя контейнерами "frontend" и "backend" и общей папкой /static   
  [stage.yaml](https://github.com/Kostromin-Mixa/13-kubernetes-config-02-mounts/blob/main/stage.yaml)   
- В общую папку в контейнере backend помещён файл test.txt   
- Из контейнера frontend файл test.txt так же доступен:   

![2021-11-01_23-52-04](https://user-images.githubusercontent.com/78191008/139729254-facbac01-84f3-40a0-a1db-c39aafc1875f.png)

## 2 задание   
Созданы два POD [frontend](https://github.com/Kostromin-Mixa/13-kubernetes-config-02-mounts/blob/main/front.yaml) и [backend](https://github.com/Kostromin-Mixa/13-kubernetes-config-02-mounts/blob/main/back.yaml)   

![2021-11-02_15-46-01](https://user-images.githubusercontent.com/78191008/139832428-dc894ccf-9308-4175-81e5-7073d5d04fa8.png)

А так же [PV](https://github.com/Kostromin-Mixa/13-kubernetes-config-02-mounts/blob/main/pv.yaml) и [PVC](https://github.com/Kostromin-Mixa/13-kubernetes-config-02-mounts/blob/main/pvc.yaml)   

![pv_pvc](https://user-images.githubusercontent.com/78191008/139832270-1a8d4345-efe5-4e81-9627-6e75fd8680e8.png)

Создаём в backend файл netology.txt и проверяем его доступность в frontend, файл всезде доступен.   

![2021-11-02_15-17-50](https://user-images.githubusercontent.com/78191008/139832929-dbf0ed5e-9178-424a-b2d2-12748e4ac500.png)

