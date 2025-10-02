#### Actividades iniciales
**Trabajo en equipo**

1. Crea una carpeta en tu PC **“Tu nombre - Proyecto Aurelion”**.  
2. Conecta dicha carpeta a **VS Code**.  
3. Dentro, crea el archivo **DOCUMENTACION.md**.  
4. Describe el problema que quieres resolver o lo que te gustaría analizar:  
   **Ranking de ventas por Ciudad**  
5. Describe estructura, tipos y escala de la BD:

### Tabla: Ventas
| Campo          | Tipo de dato | Escala    |
|----------------|--------------|-----------|
| id_venta       | int          | Razón     |
| fecha          | datetime.date| Intervalo |
| id_cliente     | int          | Razón     |
| nombre_cliente | str          | Nominal   |
| email          | str          | Nominal   |
| medio_pago     | str          | Nominal   |

---

### Tabla: Productos
| Campo           | Tipo de dato | Escala   |
|-----------------|--------------|----------|
| id_producto     | int          | Razón    |
| nombre_producto | str          | Nominal  |
| categoria       | str          | Nominal  |
| precio_unitario | float        | Razón    |

---

### Tabla: Detalle de venta
| Campo           | Tipo de dato | Escala   |
|-----------------|--------------|----------|
| id_venta        | int          | Razón    |
| id_producto     | int          | Razón    |
| nombre_producto | str          | Nominal  |
| cantidad        | int          | Razón    |
| precio_unitario | float        | Razón    |
| importe         | float        | Razón    |

---

### Tabla: Clientes
| Campo          | Tipo de dato | Escala    |
|----------------|--------------|-----------|
| id_cliente     | int          | Razón     |
| nombre_cliente | str          | Nominal   |
| email          | str          | Nominal   |
| ciudad         | str          | Nominal   |
| fecha_alta     | datetime.date| Intervalo |