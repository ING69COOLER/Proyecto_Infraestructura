# Bitácora del Proyecto de Infraestructura Computacional

## Día 1 — Configuración de RAID y LVM
- Configuré tres arreglos RAID 1 usando `mdadm`.
- ![alt text](https://github.com/ING69COOLER/Proyecto_Infraestructura/blob/main/imagenes/Captura%20de%20pantalla%202025-11-15%20172125.png?raw=true)
- Creé volúmenes LVM sobre cada RAID.
- Monté los volúmenes en `/home/pete3000/apache`, `/home/pete3000/mysql`, `/home/pete3000/nginx`.

## Día 2 — Contenedor Apache
- Creé el Dockerfile.
- Construí la imagen `apache-custom`.
- Monté el volumen LVM.
- Probé acceso desde navegador.

## Día 3 — Contenedor MySQL
- Creé la imagen personalizada `mysql-custom`.
- Probé conexión y creación de bases de datos.
- Verifiqué persistencia después del reinicio.

## Día 4 — Contenedor Nginx
- Desplegué Nginx con volumen persistente.
- Verifiqué contenido web.

## Día 5 — Pruebas finales
- Apache OK.
- Nginx OK.
- MySQL OK con persistencia.

