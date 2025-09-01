# Organización de la Carpeta Comercial

Este manual explica cómo organizar correctamente la carpeta comercial, asegurando una gestión eficiente de los productos en **Tienda Nube** y la generación automática del catálogo de productos.

### **Estructura de la Carpeta Comercial**

Dentro de la carpeta comercial, encontrarás una subcarpeta llamada **"producto"**. Esta contiene todas las categorías de productos disponibles en la tienda.

#### **1. Organización de Categorías**

* Dentro de la carpeta **"producto"**, cada categoría debe tener su propia subcarpeta.
* Estas categorías pueden **no ser idénticas** a las de Tienda Nube, pero deben mantener una estructura clara.
* **Si un producto no encaja en ninguna categoría existente**, se asignará a la categoría o carpeta **"Otros"**.

#### **2. Creación de Carpetas para Productos**

Cada producto debe tener su propia carpeta dentro de la categoría correspondiente. Sigue esta nomenclatura al crear nuevas carpetas de productos:

📌 **Formato del nombre de la carpeta del producto:**

```
[SKU] - [Nombre del Producto]
```

Ejemplo:

```
12345 - Aceite Esencial
```

<figure><img src="../../.gitbook/assets/Estructura correcta.jpg" alt=""><figcaption></figcaption></figure>

💡 **IMPORTANTE:** La descripción del producto **debe ser igual** a la que está en Tienda Nube. En caso de diferencias, se tomará la descripción de Tienda Nube.

#### **3. Agregar Imágenes de Producto**

* Es **obligatorio** incluir al menos **una imagen del producto** en su respectiva carpeta.
* **Requisito importante**: La imagen debe **tener fondo transparente**.
* **No se pueden incluir fotos que no correspondan al producto.**

### **4. Generación Automática del Catálogo**

* La carpeta de productos es clave para la generación automática del **catálogo de productos**, que posteriormente será enviado por **WhatsApp**.
* **Si un producto no tiene su carpeta con SKU y nombre correctamente configurados, no aparecerá en el catálogo.**
* Las imágenes también deben estar correctamente organizadas, ya que el catálogo solo incluirá productos bien estructurados.



### 5. Estructura de Carpetas y Descripción de Cada Categoría

A continuación, se detallan los nombres y la finalidad de las subcarpetas que deben hallarse (o crearse) dentro de la carpeta principal:

1. **000-Con Fondo**
   * **Descripción**: Aquí se colocarán todas las fotos que tengan algún tipo de fondo (cualquiera) excepto las de fondo blanco puro.
   * **Uso**: Estas imágenes pueden incluir escenarios, props, ambientes o texturas. Se utilizan, por ejemplo, para publicaciones en redes sociales donde se quiera mostrar el producto en un contexto llamativo.
2. **001-Sin Fondo**
   * **Descripción**: Solo fotos cuyo fondo sea **completamente blanco** (RGB 255,255,255).
   * **Uso**: Se emplean en el sitio web oficial o en listados donde se busque un look limpio y estandarizado (p. ej., tienda online).
3. **003-ML** (Mercado Libre)
   * **Descripción**: Dentro de esta carpeta, para cada SKU o modelo de producto, se colocarán únicamente:
     * Las fotos que **tengan fondo blanco** (idénticas a las de 001).
     * **La imagen principal** que mejor represente el producto (puede coincidir con una de las de fondo blanco).
   * **Uso**: Estas imágenes son exclusivas para la publicación en Mercado Libre. En ML es obligatorio que la foto principal tenga fondo blanco, y opcionalmente se pueden agregar variantes.
4. **004-Catalogo**
   * **Descripción**: Contendrá **una sola foto** por cada producto, seleccionada cuidadosamente para su inclusión en catálogos (digitales o impresos).
   * **Uso**: Esta imagen debe cumplir criterios de alta resolución, buena iluminación y encuadre que permita que el catálogo luzca profesional.

Para garantizar una correcta organización y evitar errores en el catálogo:

✅ **Las carpetas de productos deben seguir este formato:**\
`[SKU] - [Nombre del Producto]`

✅ **Las descripciones deben coincidir con Tienda Nube.**\
Si no coinciden, se usará la de Tienda Nube.

✅ **No se permite almacenar fotos sueltas dentro de categorías o en la carpeta general.**

* Las imágenes deben estar **dentro de la carpeta del producto correspondiente**.
* Si hay fotos sin asociar a un producto, **serán eliminadas.**

✅ **No puede haber carpetas sin SKU o sin nombre de producto.**

* Si una carpeta no sigue la estructura correcta, **el producto no será visible en el catálogo.**

### **Conclusión**

Siguiendo esta estructura, garantizamos un orden lógico y accesible para todos los productos dentro de la carpeta comercial. Esto facilita la gestión y actualización de productos en Tienda Nube y la generación automática del catálogo.

\
\


## Errores

* Hay fotos sin asignar a un productos

<figure><img src="../../.gitbook/assets/Error en la carga de fotos de productos.jpg" alt=""><figcaption></figcaption></figure>
