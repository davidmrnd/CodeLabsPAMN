# Codelab 2: Happy Birthday Card

Este ejercicio expande la app "Greeting Card" para crear una tarjeta de felicitación de cumpleaños. El objetivo principal era aprender a superponer texto sobre una imagen de fondo.

## Aspectos Interesantes y Conceptos Aprendidos

Este codelab se centró en cómo organizar y superponer elementos de UI:

* **Composable `Image`:** Aprendizaje de cómo incluir y mostrar recursos de imagen (assets) dentro de la app usando `painterResource(R.drawable.nombre_imagen)`.
* **Layouts - El `Box`:** El concepto clave aquí fue el `Box`. A diferencia de `Column` o `Row`, `Box` está diseñado para apilar elementos uno encima del otro. Fue interesante ver cómo se usa para poner el texto "encima" de la imagen de fondo.
* **Manejo de Imágenes (`ContentScale`):** Un aspecto muy práctico fue el uso de `contentScale = ContentScale.Crop`. Esto asegura que la imagen de fondo llene toda la pantalla sin distorsionarse, recortando el exceso.
* **Alineación (`contentAlignment` y `Modifier.align()`):** Se exploraron dos formas de alinear. Primero, usando `contentAlignment` en el `Box` para centrar todo su contenido. Luego, usando `Modifier.align()` en los elementos `Text` individuales para anclarlos a diferentes esquinas (ej. `Alignment.TopEnd`), dándonos control total sobre la posición.
* **Estilización de `Text`:** Se introdujeron más parámetros del composable `Text`, como `fontSize`, `lineHeight` y `textAlign`, para mejorar la apariencia visual.