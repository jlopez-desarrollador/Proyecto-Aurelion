
# Documento del Menú en Consola

#### 1) Tema, problema y solución
👉 **Tema:** Optimización de la estrategia comercial mediante el análisis de ventas por ciudad.  
El objetivo es identificar zonas con alto y bajo rendimiento para tomar decisiones informadas que impulsen los ingresos.  

❗ **Problema:** Actualmente no contamos con una visión clara sobre qué ciudades generan más ingresos y cuáles tienen bajo rendimiento comercial.  
Esta falta de información limita la capacidad de rediseñar estrategias específicas para mejorar las ventas en zonas menos activas.  

✅ **Solución:** Utilizaremos Python y pandas para realizar un análisis de ventas por ciudad.  

---

#### 2) Dataset de referencia

##### Tabla: Ventas
| Campo          | Tipo de dato   | Escala    |
|----------------|----------------|-----------|
| id_venta       | int            | Razón     |
| fecha          | datetime.date  | Intervalo |
| id_cliente     | int            | Razón     |
| nombre_cliente | str            | Nominal   |
| email          | str            | Nominal   |
| medio_pago     | str            | Nominal   |

##### Tabla: Productos
| Campo           | Tipo de dato | Escala   |
|-----------------|--------------|----------|
| id_producto     | int          | Razón    |
| nombre_producto | str          | Nominal  |
| categoria       | str          | Nominal  |
| precio_unitario | float        | Razón    |

##### Tabla: Detalle de venta
| Campo           | Tipo de dato | Escala   |
|-----------------|--------------|----------|
| id_venta        | int          | Razón    |
| id_producto     | int          | Razón    |
| nombre_producto | str          | Nominal  |
| cantidad        | int          | Razón    |
| precio_unitario | float        | Razón    |
| importe         | float        | Razón    |

##### Tabla: Clientes
| Campo          | Tipo de dato   | Escala    |
|----------------|----------------|-----------|
| id_cliente     | int            | Razón     |
| nombre_cliente | str            | Nominal   |
| email          | str            | Nominal   |
| ciudad         | str            | Nominal   |
| fecha_alta     | datetime.date  | Intervalo |

---

#### 3) Información, pasos, pseudocódigo y diagrama

##### 3.1 Información
1. Tema, problema y solución.  
2. Dataset de referencia.  
3. Estructura por tabla.  
4. Escalas de medición.  
5. Sugerencias y mejoras.  
6. Salir.  

##### 3.2 Pasos
1. Definir el objetivo del programa.  
2. Diseñar el menú (interfaz en consola).  
3. Elegir el mecanismo de repetición.  
4. Capturar y procesar la opción elegida.  
5. Escribir las acciones de cada opción.  
6. Control de errores.  
7. Cerrar el programa correctamente.  
8. Organizar el código en funciones.  

##### 3.3 Pseudocódigo
```
INICIO

FUNCIÓN mostrar_menu:
    IMPRIMIR "=== Menú de secciones ==="
    IMPRIMIR "1) Tema, problema y solución"
    IMPRIMIR "2) Dataset de referencia"
    IMPRIMIR "3) Información, pasos pseudocódigo y diagrama"
    IMPRIMIR "4) Sugerencias y mejoras"
    IMPRIMIR "0) Salir"

FUNCIÓN main:
    DEFINIR opcion ← NULO

    MIENTRAS opcion ≠ "0" HACER:
        LLAMAR mostrar_menu
        LEER opcion

        SI opcion = "1":
            IMPRIMIR "Tema, problema y solución..."
        SI opcion = "2":
            IMPRIMIR "Dataset de referencia..."
        SI opcion = "3":
            IMPRIMIR "Información, pasos, pseudocódigo y diagrama..."
        SI opcion = "4":
            IMPRIMIR "Sugerencias y mejoras..."
        SI opcion = "0":
            IMPRIMIR "Salir"

FIN FUNCIÓN

LLAMAR main

FIN
```

##### 3.4 Diagrama de flujo
📂 (Archivo en carpeta)

---

#### 4) Sugerencias y mejoras
1. Agregar comentarios en el código.  
2. Validar entrada del usuario con manejo de excepciones.  
3. Separar la lógica en funciones.  
4. Uso de diccionario para mapear opciones a funciones.  
5. Agregar opción de volver al menú después de cada acción.  
6. Internacionalización (soporte a varios idiomas).  
7. Documentar el código con docstrings.  
8. Agregar pruebas unitarias para asegurar el correcto funcionamiento.  
