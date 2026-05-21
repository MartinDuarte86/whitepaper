# Manual de Uso — MyAnandaTool

> **Acceso a la herramienta:** [https://martinduarte86.github.io/MyanandaTool/](https://martinduarte86.github.io/MyanandaTool/)

MyAnandaTool es la plataforma centralizada de operaciones de MyAnanda. Desde un solo lugar podés consultar el catálogo, cotizar precios, buscar productos, generar listas de precios y seguir los movimientos del negocio.

---

## Inicio diario — Paso a paso

Cada día, antes de usar cualquier módulo, el sistema verifica que la base de datos esté actualizada. Si no encuentra el archivo del día, aparece la pantalla de bloqueo.

### ¿Qué hacer si aparece "Sistema Bloqueado"?

1. Ingresá a **Tiendanube** → Productos → Exportar catálogo (CSV)
2. Descargá el archivo (se llama algo como `tiendanube-XXXXX.csv`)
3. En la pantalla de bloqueo, **arrastrá el archivo** al área punteada, o hacé clic para explorarlo
4. Esperá el mensaje ✅ **"Sistema Desbloqueado | Archivo de hoy verificado"**
5. Ya podés usar todos los módulos

> 💡 **Importante:** el archivo sube automáticamente a Google Drive. No necesitás hacer nada más.

---

## Módulos disponibles

Una vez desbloqueado, el Hub Principal muestra los cuatro módulos del sistema.

---

## 1. Cotizador de Promociones

**¿Para qué sirve?** Para armar escalas de precios con descuentos y generar etiquetas para imprimir.

### Cómo usar el Cotizador

**Paso 1 — Configurar el producto**

1. En el campo **"Nombre del Producto o Combo"**, empezá a escribir el nombre
2. Seleccioná el producto del listado que aparece abajo (el precio se carga solo)
3. Si querés cambiar el precio, editá el campo **"Precio Unitario Base ($)"**

**Paso 2 — Configurar escalas de descuento**

La tabla tiene filas con **CANT.** y **% DESC.**

| CANT. | % DESC. | Resultado |
|-------|---------|-----------|
| 1 | 0 | Precio normal, sin descuento |
| 5 | 10 | Comprando 5 unidades → 10% de descuento |
| 10 | 15 | Comprando 10 unidades → 15% de descuento |

- Podés agregar más filas con el botón **"+ Añadir escala (máx. 4)"**
- Podés eliminar una fila con el botón **✕** a la derecha
- Máximo 4 escalas por etiqueta

**Paso 3 — Indicar cantidad de copias**

En el campo **"× Copias"** indicá cuántas veces querés que aparezca esta etiqueta en la hoja impresa (máximo 20).

**Paso 4 — Agregar a la hoja**

Hacé clic en **"➕ Agregar a la Hoja"**. La etiqueta aparece en la sección inferior y el formulario se limpia para configurar el próximo producto.

**Paso 5 — Imprimir**

Una vez que agregaste todas las etiquetas:

- Revisá el preview en **"2. Hoja de Impresión"**
- Usá el botón **"✕"** en cada card para quitar una etiqueta si te equivocaste
- Hacé clic en **"🖨️ Imprimir Hoja"** → se abre el diálogo de impresión
- El layout es de **4 etiquetas por hoja A4** (2 columnas × 2 filas)
- Si tenés más de 4 etiquetas, se genera automáticamente la segunda página

> 💡 **Tip:** si querés empezar de cero, usá el botón **"🗑️ Limpiar todo"**.

---

## 2. Buscador Avanzado

**¿Para qué sirve?** Para consultar el catálogo completo con stock, precios y variantes en tiempo real.

### Cómo buscar

Tenés dos campos de búsqueda:

- **BUSCAR POR PRODUCTO** → escribí el nombre del producto (ej: "Sahumerio", "Vela", "Fuente")
- **BUSCAR POR AROMA** → escribí el aroma (ej: "Lavanda", "Palo Santo", "Rosas")

Podés usar los dos campos al mismo tiempo para afinar la búsqueda.

### ¿Qué muestra la tabla?

| Columna | Descripción |
|---------|-------------|
| Nombre del Producto | Nombre clickeable para ver todos los detalles |
| Aroma (Variante) | El aroma o variante específica |
| Stock Acumulado | Stock total de todas las variantes del producto |
| Stock Aroma | Stock de esa variante en particular |
| Precio | Precio de venta (tachado si hay promo activa) |

**Colores del stock:**
- 🟢 Verde → stock normal (10 o más unidades)
- 🟡 Amarillo → stock crítico (menos de 10)
- 🔴 Rojo → sin stock (0 unidades)

### Ver el detalle completo de un producto

Hacé clic en el **nombre del producto** (aparece subrayado con línea punteada) para abrir un popup con:

- **Badge Vigente / No vigente** → indica si el producto está activo en la tienda
- **Stock total acumulado** de todas las variantes
- **Costo** interno del producto
- **Dimensiones** (Alto × Ancho × Profundidad en cm)
- **Categorías** del producto
- **Descripción** del producto (hacé clic en "Ver más" para expandir)
- **Tabla de variantes** con: Aroma, SKU, Mostrar en tienda, Stock, Precio, Precio promo

Las filas de variantes aparecen en **rojo** cuando el stock de ese aroma es 0.

> 💡 Si buscaste por aroma antes de abrir el popup, la tabla de variantes ya viene filtrada por ese aroma.

### Ir directamente al Cotizador

Desde el popup del producto, el botón **"🏷️ Ir al Cotizador con este producto"** te lleva al Cotizador con el nombre y precio ya pre-cargados.

---

## 3. Lista de Precios

**¿Para qué sirve?** Para generar listas de precios en formato PDF para distribución.

### Generar Lista Mayorista

1. La barra superior confirma el archivo Tiendanube del día verificado
2. Hacé clic en **"Generar Lista Mayorista"**
3. El sistema procesa los datos y descarga un PDF con todos los productos activos, ordenados alfabéticamente
4. Los productos con precio promocional aparecen con el precio original tachado y el precio promo destacado en rojo

> 📌 Los botones "Generar lista de precios sugeridos" y "Generar lista myananda emprende" se activan con los datos enviados desde el sistema de automatización n8n.

---

## 4. Movimientos

**¿Para qué sirve?** Para llevar el seguimiento de la liquidez, inversiones y presupuesto mensual.

### Panel principal

El dashboard muestra tres indicadores clave:

- **Liquidez Disponible** → efectivo/disponible actual
- **Inversiones Activas** → inversiones en curso con rendimiento estimado
- **Presupuesto Mensual** → cuánto queda del presupuesto del mes con barra de progreso

### Registrar un movimiento

1. Hacé clic en **"+ Nuevo Movimiento"**
2. Completá: fecha, descripción, categoría (Ingreso / Gasto / Inversión) y monto
3. El movimiento aparece en la lista "Últimas Transacciones"

### Gestión Rápida

La sección lateral permite:

- **Ajustar Presupuesto** → modificar el presupuesto mensual
- **Sincronizar Datos** → actualizar con los últimos datos del sistema

---

## Actualizar el catálogo en cualquier momento

Si durante el día necesitás actualizar la base de datos sin cerrar la sesión:

1. Hacé clic en el botón **"🔄 Actualizar Catálogo"** (esquina superior derecha, visible en todos los módulos)
2. Arrastrá o seleccioná el nuevo archivo CSV de Tiendanube
3. El sistema procesa y confirma la actualización con el mensaje de conexión activa

---

## Preguntas frecuentes

**¿Por qué aparece "Sistema Bloqueado" si ya subí el archivo ayer?**\
El sistema verifica el archivo del día actual. Cada día hay que subir el CSV actualizado de Tiendanube para desbloquear.

**¿El archivo que subo se guarda en algún lado?**\
Sí. El archivo se guarda automáticamente en una carpeta de Google Drive del sistema. No necesitás guardarlo manualmente.

**¿Por qué un producto aparece con stock 0?**\
Puede ser que el producto esté sin stock en Tiendanube, o que el campo "Mostrar en tienda" esté en NO. El buscador muestra todos los productos, incluso los que no están activos en la tienda.

**¿Los precios que veo son los de Tiendanube?**\
Sí. Los precios se leen directamente del archivo CSV exportado desde Tiendanube. Si hay un precio desactualizado, hay que exportar el catálogo actualizado desde Tiendanube y subirlo.

**¿Puedo usar la herramienta desde el celular?**\
Sí, la herramienta es responsive. Para mejor experiencia se recomienda usar desde computadora, especialmente para el módulo de Cotizador y la impresión de etiquetas.

**¿Qué pasa si cierro el navegador con etiquetas en la Hoja de Impresión?**\
Las etiquetas se pierden al cerrar el navegador. El Cotizador no guarda el estado de la hoja entre sesiones. Conviene armar e imprimir en la misma sesión.

**¿Cuántas escalas puede tener una etiqueta?**\
Máximo 4 escalas de precio por etiqueta.

**¿Cuántas etiquetas entran en una hoja A4?**\
4 etiquetas por página (2 columnas × 2 filas de 9cm × 9cm). Si tenés más de 4, se imprimen automáticamente en páginas adicionales.

---

## Acceso rápido

| Módulo | URL |
|--------|-----|
| Hub Principal | [/](https://martinduarte86.github.io/MyanandaTool/) |
| Cotizador | [/cotizador.html](https://martinduarte86.github.io/MyanandaTool/cotizador.html) |
| Buscador Avanzado | [/buscador-avanzado.html](https://martinduarte86.github.io/MyanandaTool/buscador-avanzado.html) |
| Lista de Precios | [/generador-pdf.html](https://martinduarte86.github.io/MyanandaTool/generador-pdf.html) |
| Movimientos | [/movimientos.html](https://martinduarte86.github.io/MyanandaTool/movimientos.html) |
