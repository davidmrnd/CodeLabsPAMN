# Codelab 1: Greeting Card App

Esta es la primera aplicación creada como parte de los Codelabs de Kotlin para Android. Es una aplicación muy simple que muestra un mensaje de texto en la pantalla.

## Aspectos Interesantes y Conceptos Aprendidos

Aunque es un ejercicio básico, introduce los pilares fundamentales de Jetpack Compose:

* **Funciones Composable (`@Composable`):** El concepto central de que la UI se define mediante funciones. Fue mi primera vez viendo cómo `@Composable` le dice al compilador que esta función describe una pieza de UI.
* **El Composable `Text`:** La unidad básica para mostrar texto.
* **El `Modifier`:** El aspecto más interesante fue cómo se usa `Modifier` para "decorar" o añadir comportamiento a un composable. En este caso, se usó `Modifier.padding()` para añadir espacio alrededor del texto, demostrando cómo se encadenan las modificaciones.
* **La Anotación `@Preview`:** Sin duda, la herramienta más útil. Poder ver los cambios de la UI en tiempo real en Android Studio sin tener que compilar y ejecutar la app completa en un emulador es un cambio radical en la velocidad de desarrollo.
* **Organización del Proyecto:** El primer vistazo a la estructura de un proyecto de Android (el fichero `MainActivity.kt`, `build.gradle`, etc.).