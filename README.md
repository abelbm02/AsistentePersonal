# 🤖 Mi Asistente Personal en Python

Aplicación de consola interactiva diseñada para resolver tareas cotidianas reales —gestión de compras, finanzas, conversores, agenda, inventario, utilidades matemáticas y **conteo/análisis de entrenamientos**— con **guardado automático en JSON** para conservar tus datos entre sesiones.

Proyecto desarrollado para la asignatura **Programación IA (2026/27)** de **iLERNA** (UD02: Funciones en Python).

Realizado por: Abel Blanco Muñoz

---

## ✨ Funcionalidades principales

El asistente cuenta con un menú interactivo en consola a prueba de errores y se organiza en **8 módulos**:

| #     | Módulo                            | Qué puedes hacer en el día a día                                                                                                     |
| ----- | --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **1** | **Gestión de compras**            | Calcular precios con descuento e IVA, ahorro total y comparar precio por unidad/kilo.                                                |
| **2** | **Gestión económica**             | Controlar presupuesto mensual, sumar múltiples gastos y repartir cuentas entre amigos (con propina opcional).                        |
| **3** | **Conversores**                   | Convertir temperaturas (°C, °F, K), distancias (`km ↔ millas ↔ metros` para entrenos/viajes) y tiempos (`minutos → h:min`).          |
| **4** | **Agenda de contactos**           | Añadir contactos con etiqueta (entreno, familia, trabajo), buscar por nombre o categoría y ordenar alfabéticamente.                  |
| **5** | **Gestión de productos**          | Registrar despensa, suplementación o material deportivo, consultar stock y detectar productos con existencias bajas.                 |
| **6** | **Utilidades matemáticas**        | Calcular **factorial**, serie de **Fibonacci** y **MCD** (máximo común divisor).                                                     |
| **7** | **Conteo y análisis de entrenos** | Registrar sesiones de entrenamiento, obtener estadísticas (total, media, mínimo, máximo) y filtrar sesiones que superen un objetivo. |
| **8** | **Persistencia y salida**         | Guardado automático de contactos, inventario, gastos y entrenamientos en archivos `.json` y cierre seguro del programa.              |

---

## 🛠️ Requisitos técnicos cubiertos

El código está diseñado de forma modular y reutilizable, aplicando todos los conceptos clave de funciones en Python:

- **Funciones sin parámetros:** visualización de menús y cabeceras.
- **Funciones con uno y varios parámetros:** conversores y cálculos matemáticos.
- **Parámetros opcionales (por defecto):** cálculo de IVA (`iva=0.21`), descuentos o propinas.
- **Argumentos variables (`*args` / `**kwargs`):** suma flexible de gastos y registro dinámico de atributos de productos.
- **Retorno múltiple:** devolución de tuplas con varios resultados (ej. precio final y ahorro, o estadísticas completas).
- **Recursividad:** cálculo de factorial, Fibonacci y MCD con su caso base definido.
- **Funciones `lambda`:** ordenación de listas/diccionarios y filtrado de entrenamientos o datos.
- **Validaciones:** control de entradas con `try/except`, prevención de divisiones por cero, listas vacías y valores negativos.

---

## 📁 Estructura del proyecto

```text
AsistentePersonal/
│
├── AP_SinParametros.py          # Pruebas y funciones sin parámetros
├── AP_UnParametro.py            # Pruebas y funciones con un parámetro
├── AP_VariosParametros.py       # Pruebas y funciones con varios parámetros, opcionales y *args/**kwargs
├── AP_ListasDiccionarios.py     # Pruebas de agenda, inventario y análisis de listas
├── AP_Recursividad.py           # Pruebas de funciones recursivas (factorial, Fibonacci, MCD)
├── APLambda.py                  # Pruebas de funciones lambda (ordenación y filtrado)
│
├── Proyecto_AsistentePersonal/
│   ├── main.py                  # Punto de entrada y menú interactivo
│   └── funciones.py             # Módulo unificado con toda la lógica del asistente
│
├── .gitignore
└── README.md
```

---

## 🚀 Cómo ejecutarlo

### Requisitos previos
- **Python 3.10** o superior (no requiere librerías externas; solo usa la biblioteca estándar de Python).

### Pasos
1. Clona el repositorio:
   ```bash
   git clone https://github.com/abelbm02/AsistentePersonal.git
   cd AsistentePersonal
   ```

2. Ejecuta el asistente completo:
   ```bash
   python Proyecto_AsistentePersonal/main.py
   ```

3. *(Opcional)* También puedes ejecutar de forma independiente cualquiera de los archivos `AP_*.py` para probar cada tipo de función por separado:
   ```bash
   python AP_Recursividad.py
   ```

---

## 👤 Autor

**Abel Blanco Muñoz**
- GitHub: [@abelbm02](https://github.com/abelbm02)
- Asignatura: Programación IA 2026/27 — iLERNA
