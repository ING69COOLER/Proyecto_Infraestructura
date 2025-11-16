# Bitácora del Proyecto de Infraestructura Computacional

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
- Construí la imagen `apache-custom`.
- Monté el volumen LVM.
- Probé acceso desde navegador.

## Contenedor MySQL
- Creé la imagen personalizada `mysql-custom`.
- Probé conexión y creación de bases de datos.
- Verifiqué persistencia después del reinicio.

## Contenedor Nginx
- Desplegué Nginx con volumen persistente.
- Verifiqué contenido web.

## Pruebas finales
- Apache OK.
- Nginx OK.
- MySQL OK con persistencia.





