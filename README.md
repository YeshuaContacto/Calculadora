# Calculadora en PySide6 - YeshuaContacto
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white&labelColor=101010)]()
[![PySide6](https://img.shields.io/badge/PySide6-Qt-4A90E2?style=for-the-badge&logo=qt&logoColor=white&labelColor=101010)](https://wiki.qt.io/Qt_for_Python)

![[https://github.com/YeshuaContacto](https://github.com/YeshuaContacto)](./Calculadora.jpg)


Este es un programa que implementa una calculadora básica utilizando la biblioteca PySide6 para crear la interfaz gráfica. La calculadora muestra los números y las operaciones en un panel LCD y permite realizar cálculos simples.

## Clase `Calculadora`

La clase `Calculadora` hereda de `QLCDNumber` y representa el panel LCD donde se muestran los números y resultados. Tiene los siguientes métodos:

- `__init__()`: Inicializa la calculadora con una configuración por defecto y variables para el número actual, operación y reinicio.
- `escribir(caracter)`: Agrega caracteres al panel LCD, permitiendo la entrada de números y la coma decimal.
- `preparar(operacion)`: Almacena en memoria el número y la operación seleccionada para su posterior cálculo.
- `calcular()`: Realiza el cálculo utilizando la operación almacenada y el número en memoria, luego muestra el resultado en el panel LCD.
- `limpiar()`: Establece el panel LCD a cero, reiniciando la calculadora.

## Clase `Window`

La clase `Window` hereda de `QWidget` y representa la ventana de la calculadora. Tiene los siguientes métodos:

- `__init__()`: Inicializa la ventana y establece su tamaño y título. Carga estilos de una hoja de estilos externa.
- `boton_clicado(simbolo)`: Maneja el clic en los botones de la calculadora, llamando a los métodos apropiados de la calculadora según el símbolo clicado.

En el método `__main__`, se crea una instancia de `QApplication` y `Window`, y se muestra la ventana de la calculadora.

La interfaz gráfica incluye botones para los dígitos, operaciones básicas y el cálculo, y un panel LCD para mostrar los números y resultados.

La calculadora utiliza clases y métodos de PySide6 para crear la interfaz gráfica y manejar las interacciones del usuario.
