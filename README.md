# Sistema de Gestion de Construccion de Viviendas

**Universidad Catolica del Norte - Ingenieria de Software - Entrega 1**

---

## Casos de Prueba

### Evidencias Simuladas

#### Evidencia 1 - Registro de Material

- **Fecha:** 08/06/2026
- **Accion realizada:** Registro de material "Cemento Gris"
- **Datos ingresados:**
  - Nombre: Cemento Gris
  - Cantidad: 200 unidades
  - Unidad de medida: Bultos (50 kg)
  - Costo unitario: $32.000
- **Resultado obtenido:** El sistema registro correctamente el material
- **Mensaje mostrado:** Material registrado exitosamente. ID Material: MAT-001

---

#### Evidencia 2 - Registro de Gasto

- **Fecha:** 10/06/2026
- **Accion realizada:** Registro de compra de materiales
- **Datos ingresados:**
  - Descripcion: Compra de materiales
  - Monto: $6.400.000
  - Categoria: Materiales
- **Resultado obtenido:** Registro exitoso
- **Mensaje mostrado:** Gasto registrado exitosamente. Presupuesto consumido: 9%

---

#### Evidencia 3 - Seguimiento de Avance

- **Fecha:** 15/06/2026
- **Etapa:** Cimentacion
- **Avance registrado:** 50%
- **Resultado obtenido:** Sistema actualiza avance general
- **Mensaje mostrado:** Etapa actualizada. Avance general del proyecto: 25%

---

#### Evidencia 4 - Asignacion de Tareas

- **Fecha:** 16/06/2026
- **Datos:**
  - Tarea: Instalar vigas de soporte
  - Responsable: Carlos Perez
  - Prioridad: Alta
  - Fecha limite: 20/06/2026
- **Resultado obtenido:** Tarea creada correctamente
- **Mensaje mostrado:** Tarea asignada exitosamente. Estado: Pendiente

---

#### Evidencia 5 - Prueba Negativa

- **Caso:** Registrar gasto negativo
- **Dato ingresado:** -$500.000
- **Resultado esperado:** Error: El valor del gasto debe ser mayor a cero
- **Resultado obtenido:** El sistema bloqueo el registro
- **Estado de la prueba:** Aprobada

---

## Estrategia de Pruebas Utilizada

Para comprobar que el sistema funciona correctamente, se realizaron diferentes pruebas durante el desarrollo. Estas pruebas permitieron identificar errores, verificar que las funciones cumplieran los requisitos establecidos y asegurarnos que la informacion corre adecuadamente.

### Pruebas Unitarias

Se utilizaron con el fin de revisar cada modulo por aparte verificando que ejecutara correctamente las tareas. Los modulos revisados fueron:

- Gestion de materiales
- Control de gastos
- Seguimiento de avances de las obras
- Gestion de tareas

**Proposito:** Ayuda a encontrar errores especificos de cada funcion, evitando problemas a la hora de unir los modulos.

### Pruebas de Integracion

Se realizaron con el fin de comprobar si los modulos estaban trabajando sin problemas y que se estuvieran comunicando correctamente.

**Proposito:** Garantizar que la informacion se comparta correctamente como, por ejemplo:

- Registro de compra de materiales y actualizacion de gastos
- Actualizacion del avance de obras y tareas a completar
- Consultar informacion en la base de datos

### Pruebas Funcionales

Se verificaron que todas las funcionalidades definidas cumplieran los requisitos del proyecto y que este funcionara de acuerdo con las necesidades de los usuarios.

**Proposito:** Validar las funcionalidades cumplan los requerimientos establecidos como:

- Crear materiales
- Consultar gastos
- Asignar tareas
- Visualizar avances

### Pruebas de Validacion de Datos

Se utilizaron el ingreso de datos incorrectos o incompletos para verificar las reglas de validacion. Por ejemplo:

- Registrar material sin nombre
- Registrar un gasto con valor negativo
- Ingresar un avance superior al 100%
- Crear una tarea sin responsable asignado

**Proposito:** Evitar errores de captura de datos garantizando su integridad.

### Pruebas de Estres

Se realizaron simulaciones con grandes cargas de datos para observar como se comportaba el sistema.

**Proposito:** Comprobar si la aplicacion seguia funcionando correctamente despues de recibir tanta informacion.

### Pruebas de Aceptacion

Se realizaron al final del desarrollo para revisar que las funcionalidades principales estuvieran funcionando bien.

**Proposito:** Verificar que el sistema cumple los objetivos y esta lista para su entrega.

### Resultados Finales

Despues de haber realizado las pruebas, podemos determinar que las funcionalidades principales operaban correctamente y el sistema respondia a los requisitos establecidos.

---

## Justificacion Tecnica de las Tecnologias Utilizadas

### Trello

Se utilizo como herramienta de gestion de tareas debido a que permite organizar las actividades del equipo mediante tableros, listas y tarjetas. Gracias a esta herramienta fue posible asignar responsabilidades, realizar seguimiento al avance del proyecto y mantener una mejor comunicacion entre los integrantes.

### GitHub

Se empleo como repositorio para almacenar tanto el codigo como la documentacion del proyecto. GitHub facilita el control de versiones, permitiendo registrar los cambios realizados y mantener un historial organizado del desarrollo. Ademas, favorece el trabajo colaborativo y la centralizacion de la informacion del proyecto.

### Figma

Se utilizo para la elaboracion de los disenos y prototipos de la interfaz del sistema antes de iniciar la etapa de programacion. Esto permitio visualizar la estructura de la aplicacion, identificar posibles mejoras y validar el diseno antes de su implementacion.

---

## Gestion Post-Proyecto

### Estrategia de Seguimiento

Despues de entregar el sistema, se realizara un seguimiento para verificar que todas las funciones operen correctamente y que los usuarios puedan utilizar la plataforma sin inconvenientes.

### Soporte Tecnico

Se brindara apoyo a los usuarios para resolver dudas, reportar errores o inconvenientes relacionados con el funcionamiento del sistema.

### Mantenimiento

Se realizaran revisiones periodicas para:

- Corregir errores detectados
- Mejorar el rendimiento del sistema
- Actualizar funcionalidades cuando sea necesario

### Respaldo de Informacion

Se recomienda realizar copias de seguridad periodicas para proteger la informacion registrada en el sistema y evitar perdidas de datos.

### Mejoras Futuras

Como futuras versiones del sistema se podrian incorporar:

- Gestion de multiples obras simultaneamente
- Integracion con proveedores
- Modulo de facturacion
- Sistema de mensajeria interna

---

## Manual de Usuario

### Introduccion al Sistema

BuildTrack es un sistema de gestion de construccion de viviendas que facilita la organizacion, control y seguimiento del proceso constructivo. Permite administrar materiales, gastos, avances de obra y tareas desde una unica plataforma.

### Requisitos Previos

- Navegador web actualizado (Chrome, Firefox, Edge o Safari)
- Credenciales de acceso proporcionadas por el administrador segun el rol asignado
- Conexion a internet estable

---

### Modulo de Materiales

#### Registrar un nuevo material

1. Desde el menu principal, seleccionar **Materiales** en la barra de navegacion lateral
2. Hacer clic en el boton **+ Agregar Material**
3. Completar el formulario con los datos del material (nombre, cantidad, unidad de medida, costo unitario)
4. Presionar **Guardar** para registrar el material en el sistema

**Ejemplo:**

| Campo | Valor |
|---|---|
| Nombre | Cemento Gris |
| Cantidad | 200 unidades |
| Unidad de medida | Bultos (50 kg) |
| Costo unitario | $32.000 |

**Resultado:** Material registrado exitosamente. ID Material: MAT-001

#### Editar un material existente

1. En la lista de materiales, buscar el material que se desea modificar
2. Hacer clic en el icono de edicion (lapiz) junto al material
3. Modificar los campos necesarios y presionar **Actualizar**

#### Consultar materiales

La pantalla principal del modulo muestra una tabla con todos los materiales registrados. Se puede ordenar por nombre, cantidad o costo, y utilizar filtros para encontrar materiales especificos.

> **Importante:** No se permite registrar un material sin nombre. El sistema mostrara un error de validacion si se intenta guardar con campos obligatorios vacios.

---

### Modulo de Control de Gastos

#### Registrar un gasto

1. Desde el menu principal, seleccionar **Gastos** en la barra de navegacion
2. Hacer clic en **+ Registrar Gasto**
3. Ingresar la descripcion del gasto, el monto, la categoria y la fecha correspondiente
4. Presionar **Guardar**. El sistema actualizara automaticamente el porcentaje de presupuesto consumido

**Ejemplo:**

| Campo | Valor |
|---|---|
| Descripcion | Compra de materiales |
| Monto | $6.400.000 |
| Categoria | Materiales |
| Fecha | 10/06/2026 |

**Resultado:** Gasto registrado exitosamente. Presupuesto consumido: 9%

#### Consultar gastos

El panel de gastos muestra un resumen con el presupuesto total, el monto gastado, el porcentaje consumido y un desglose por categoria. Se puede filtrar gastos por rango de fechas y categoria.

> **Validacion:** No se permite registrar gastos con valores negativos. Si se ingresa un monto como -$500.000, el sistema mostrara: "Error: El valor del gasto debe ser mayor a cero."

---

### Modulo de Avances de Obra

#### Registrar avance de una etapa

1. Seleccionar **Avances** en el menu de navegacion
2. Elegir la etapa de la obra que se desea actualizar (ej: Cimentacion, Estructura, Acabados)
3. Ingresar el porcentaje de avance actual de la etapa (valor entre 0% y 100%)
4. Presionar **Actualizar Avance**. El sistema recalculara el avance general del proyecto

**Ejemplo:**

| Campo | Valor |
|---|---|
| Etapa | Cimentacion |
| Avance registrado | 50% |
| Fecha | 15/06/2026 |

**Resultado:** Etapa actualizada. Avance general del proyecto: 25%

#### Visualizar avance general

El panel de avances presenta una barra de progreso general y el desglose por etapa. Cada etapa muestra su porcentaje individual, lo que permite identificar rapidamente cuales requieren atencion.

> **Validacion:** No se permite ingresar un avance superior al 100%. El sistema rechazara valores fuera del rango 0-100.

---

### Modulo de Gestion de Tareas

#### Crear y asignar una tarea

1. Seleccionar **Tareas** en el menu de navegacion
2. Hacer clic en **+ Crear Tarea**
3. Ingresar el nombre de la tarea, seleccionar al trabajador responsable, establecer la prioridad y la fecha limite
4. Presionar **Guardar**. La tarea se creara con estado "Pendiente" y sera visible para el trabajador asignado

**Ejemplo:**

| Campo | Valor |
|---|---|
| Tarea | Instalar vigas de soporte |
| Responsable | Carlos Perez |
| Prioridad | Alta |
| Fecha limite | 20/06/2026 |

**Resultado:** Tarea asignada exitosamente. Estado: Pendiente

#### Estados de una tarea

Las tareas pasan por los siguientes estados durante su ciclo de vida:

**Pendiente** → **En Progreso** → **Completada**

> **Validacion:** No se permite crear una tarea sin responsable asignado. El sistema requiere que se seleccione un trabajador antes de guardar.

---

### Validaciones del Sistema

| Error | Dato ingresado | Mensaje del sistema | Solucion |
|---|---|---|---|
| Gasto con valor negativo | -$500.000 | "Error: El valor del gasto debe ser mayor a cero." | Ingresar un valor positivo |
| Material sin nombre | Campo vacio | "Error: El nombre del material es obligatorio." | Completar el campo de nombre |
| Avance superior al 100% | 150% | "Error: El avance debe estar entre 0% y 100%." | Ingresar valor entre 0 y 100 |
| Tarea sin responsable | Sin seleccionar | "Error: Debe asignar un responsable a la tarea." | Seleccionar un trabajador de la lista |

---

### Roles de Usuario

#### Cliente

- Ver avances de obra
- Consultar gastos
- No puede editar registros

#### Arquitecto / Ingeniero

- Ver y actualizar avances
- Consultar materiales
- Acceder a reportes tecnicos

#### Trabajador

- Ver tareas asignadas
- Actualizar estado de tareas
- No puede crear nuevas tareas

#### Dueno del Proyecto

- Acceso total al sistema
- Crear y editar registros
- Gestionar usuarios

---

### Recomendaciones Generales

- No compartir credenciales de acceso con otras personas. Cada usuario tiene un perfil individual
- Verificar periodicamente que la informacion registrada este actualizada para mantener la precision de los reportes
- Ante cualquier error inesperado, tomar una captura de pantalla y reportarlo al equipo de soporte
- Mantener el navegador actualizado para garantizar la compatibilidad y seguridad del sistema

---

**Universidad Catolica del Norte - Ingenieria de Software - 2026**

**Equipo de desarrollo:**

| Integrante | Rol |
|---|---|
| Laura Valentina Arango Bedoya | Lider del Proyecto |
| Deison Mora Mira | Disenador |
| Jose Manuel Rojas Metaute | Programador |
| Nelson Estiven Lopera Mosquera | Tester |
