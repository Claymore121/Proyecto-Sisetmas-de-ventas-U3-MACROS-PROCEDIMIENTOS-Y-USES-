# ByteShop - Sistema de Ventas e Inventario (MASM x86)

Sistema de gestión de inventario y punto de venta en consola desarrollado en lenguaje ensamblador **MASM x86 (32 bits)** utilizando la biblioteca **Irvine32** para la materia de Lenguajes de Interfaz (Instituto Tecnológico de Culiacán).

## Características principales
* **Gestión de catálogo:** Registro de hasta 10 productos en memoria mediante estructuras de 44 bytes (código `ABC-123`, nombre, precio en centavos enteros y existencia).
* **Control de inventario:** Búsqueda por código, recepción de mercancía (tope de 100 unidades) y consultas de resumen con detección de desbordamiento.
* **Ventas y regla de negocio:** Descuento automático del **10 %** al vender 10 o más unidades de un mismo producto en una transacción, además de opción para cotizar sin afectar existencias.
* **Persistencia en archivo:** Guardado y carga de catálogo en archivos de texto plano (`inventario.txt`) con validación estricta de formato y prevención de corrupción de datos.
* **Arquitectura modular (Unidad 3):** Refactorizado con procedimientos reutilizables, macros parametrizadas (con etiquetas `LOCAL`) y preservación automática de registros mediante `USES`.

## Requisitos y ejecución
1. Entorno Windows con **MASM32 / Visual Studio** y la biblioteca **Irvine32** configurada.
2. Ensamblar y enlazar `VentasInventario.asm`.
3. Colocar `inventario.txt` en el mismo directorio del ejecutable para la carga automática inicial.

## Integrantes
* **Luis Angel Lopez Ibarra**
* **Jose Ramses Alvarez Hicks**
