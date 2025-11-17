# Bitácora del Proyecto de Infraestructura Computacional
Manuel Pineda Varela-1092455543  

Santiago Solarte Trujillo-1059355828

Carlos Alonso Barahona Alvarez-1094896340

## Configuración de RAID y LVM
- Configuré tres arreglos RAID 1 usando `mdadm`.
  ![alt text](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-15%20172125.png?raw=true)
- Creé volúmenes LVM sobre cada RAID.
  ![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-15%20190654.png?raw=true)
- Monté los volúmenes en `/home/pete3000/apache`, `/home/pete3000/mysql`, `/home/pete3000/nginx`.
   ![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-15%20191512.png?raw=true)
  ![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-15%20191537.png?raw=true)

## Contenedor Apache
- Creé el Dockerfile.
  ![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-16%20104758.png?raw=true)
- Construí la imagen `nuestroapache`.
  ![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-16%20185653.png?raw=true)
- Monté el volumen LVM.
  ![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-16%20185948.png?raw=true)
- Probé acceso desde navegador.
![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-16%20185718.png?raw=true)

## Contenedor MySQL
- Creé el Dockerfile.

  ![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-16%20110008.png?raw=true)
- Creé la imagen personalizada `nuestromysql`.
![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-16%20115032.png?raw=true)
- Probé conexión y creación de bases de datos.
- comandos;
- "sudo docker exec -it mysqlito bash"
- "mysql -u root -p"
- "SHOW DATABASES;"

![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-16%20121951.png?raw=true)
![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-16%20122539.png?raw=true)

## Contenedor Nginx
- Dockerfile
  
  ![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-16%20123055.png?raw=true)
- Construí la imagen
  
  ![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-16%20124334.png?raw=true)
- Desplegué Nginx con volumen persistente.
  ![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-16%20124404.png?raw=true)

- Verifiqué contenido web.
  ![alt text.](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-16%20191006.png?raw=true)



















