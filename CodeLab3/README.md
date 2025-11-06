# Codelab 3: Dice Roller (Lanzador de Dados)

Esta es la primera aplicación interactiva. La app muestra la imagen de un dado y un botón. Al pulsar el botón, la app "lanza" el dado y muestra una nueva cara aleatoria.

## Aspectos Interesantes y Conceptos Aprendidos

Este fue el codelab más importante conceptualmente, ya que introdujo la **interactividad** y el **estado**.

* **El Estado (`State`) en Compose:** El concepto más fundamental. Aprendí que la UI en Compose es una *función de su estado*.
* **`remember` y `mutableStateOf`:** La "magia" de Compose. Usar `mutableStateOf` para crear una variable de estado (el resultado del dado) y `remember` para que Compose "recuerde" el valor de esta variable incluso cuando la función se "recompone" (se vuelve a dibujar).
* **Recomposición:** El aspecto más interesante. Entender que al hacer clic en el botón, no "cambiamos la imagen" manualmente. Lo que hacemos es **actualizar el valor del estado** (`result.value = ...`). Compose detecta este cambio y automáticamente vuelve a ejecutar (recompone) la parte de la UI que depende de ese estado, mostrando así la nueva imagen.
* **Composable `Button` y `onClick`:** La introducción a la interactividad. Ver qué fácil es asignar lógica (generar un número aleatorio) al evento `onClick` de un botón.
* **Lógica Condicional en la UI:** Usar un `when` (el `switch` de Kotlin) para decidir qué recurso de imagen (`R.drawable.dice_1`, `R.drawable.dice_2`, etc.) mostrar en el composable `Image` basándose en el valor actual del estado. Esto demuestra lo declarativo que es Compose.
* **Estructura y "Hoisting":** Se empezó a estructurar la app en funciones composable más pequeñas y lógicas (ej. `DiceWithButtonAndImage`), pasando el estado y los eventos (`onClick`) como parámetros.